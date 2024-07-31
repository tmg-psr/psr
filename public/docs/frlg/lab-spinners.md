# Probability analysis for FRLG lab spinners

## About
Author: themathgenius

Last updated: 20 March 2023

This analysis is restricted to determining how often the spinners can advance RNG without actually spinning. 
For background information on spinner mechanics, feel free to read [this writeup](https://pastebin.com/VxTjrnzz) by Exarion.

## Background
There are two NPC's in the lab that can choose to spin every 32 frames. When this happens (1/4 chance), the spinner will choose a new direction at random to face. [Much to the frustration of FRLG speedrunners everywhere,] This also includes the direction the spinner is already facing (1/4 chance). 

Each time the spinner chooses to spin, the RNG advances 2 states (in addition to the default one state per frame advancement rate). Assuming that these cycles are independent events (i.e., what happens in cycle 1 does not influence what happens in cycle 2),[^1]
we can break down the lab movement into 6 spin cycles for the normal lab movement to Squirtle:[^2]

```
[(2 tiles down + 3 tiles right) * (16f per tile walked)] + (2 turnframes * 8f per turnframe) = 96 frames of movement
96 frames elapsed / (32 frames per cycle per spinner) = 3 cycles per spinner
3 cycles per spinner * 2 spinners = 6 total cyles
```

## The mathy part
Let's set some definitions first:

| Event | Definition |
| --- | --- |
|	P()   |	The probability of an outcome occurring. |
| S     |	The event that a spinner chose to spin. P(S) = 1/4, calculated independently every 32 frames. |
|	~S	  |	The complement of S (read "not S"); i.e., the event that a spinner chose NOT to spin. P(~S) = 1-P(S) = 3/4. |
| B	    |	The event that a spinner chose to spin in its original direction. P(B) = P(S) * 1/4 = 1/16, calculated independently every 32 frames. |
| E     |	The event that a spinner chose not to spin GIVEN that it did NOT change direction. P(E) = 1/13[^3] |
| (n,k)	|	The binominal coefficient, commonly known as "n choose k" in combinatorics. = n!/[k! * (n-k)!] |

The probability distribution[^4] for 0-6 E's, given that the spinners stay frozen, are as follows (rounded to the nearest hundredth of a percent, or 1/10,000):

```
0: 61.86%
1: 30.93%
2: 6.44%
3: 0.71%
4: 0.04%
5-6: < 0.01%
```

## Analysis (includes some opinions so discretion is advised)
This tells us that, while at least 1 E (i.e, RNG advanced extra) is likely, the spinners staying frozen alone might not be enough to warrant assuming RNG advanced extra. However, runners can combine this probability with other independent situations (such as the fence guy being stuck against a fence or not bagging outside when going left out of your house) to give them a higher likelihood of correctly predicting unverifiable RNG advancements.


## Footnotes
[^1] These spin cycles are not independent events technically if we already knew the exact RNG seed/stream beforehand, but because we don't, we can't predict what the spinners will do, so we can treat the spins as effectively independent events.
  
[^2] The last tile up to Squirtle does not affect spin cycles; this is intentionally set up so that the npc's can't advance RNG while they are off screen.
   
[^3] The probability that a spinner does the frustrating thing (i.e, advance rng given they didn't spin) is calculated as follows:
```	
P(E) = P(B | spinner did not change direction) = P(B)/[P(B or ~S)] = P(B)/[P(B) + P(~S) - P(B and ~S)]
```
Since B and ~S are mutually exclusive events (i.e, a spinner can't advance RNG AND choose not to spin), P(B and ~S) = 0. So:
```
P(E) = P(B)/[P(B) + P(~S) - P(B and ~S)] = P(B)/[P(B) + P(~S)] = (1/16)/(12/16 + 1/16) = 1/13.
```

[^4] The calculations for the following table are as follows:
```
P(E happening k times in 6 cycles) = (6,k) * [P(~E)]^(6-k) * P(E)^k = (6,k) * (12/13)^(6-k) * (1/13)^k
```
