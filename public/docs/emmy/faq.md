# Pokémon Emerald Any% Glitchless FAQ
## About
Author: themathgenius

Last updated: 12 October 2024

The aim of this speedrun is to play the game from pressing "New Game" to entering the HOF without using glitches. RNG manipulation is allowed.

This will ultimately involve collecting all eight gym badges and defeating the Pokemon League.

## What is the WR?
2:29:51 by WaveWarrior. [VOD](https://youtu.be/AmSH2s-RYoA)

## Which Pokemon are used for battles?
Mudkip line, then Rayquaza. Both have their nature and IV's manipulated.

Mudkip: 21/23/28/30/29/29 Naughty

Rayquaza: See [below](https://github.com/tmg-psr/psr/new/main/public/docs/emmy/faq.md#rayquaza)

Mudkip's final moveset: Surf, Mud shot -> Dive, Strength, Rock Smash (yes, four HM's by the end of the game)
Rayquaza's final moveset: Fly, Waterfall, Extremespeed -> Aerial Ace, Outrage

More information on all the RNG manipulations will come later.

## Are there any other Pokemon we catch?
We ultimately collect three additional Pokemon outside of our primary battlers:
- **Taillow** - for Fly.
- **Abra** - for Teleport. The ability to Fly outside of battle only comes after the sixth badge, which is nearly 90 minutes into the run (over halfway timewise), so Teleport allows for faster travel until then.
- **Castform** - it's useful for a few required double battles.

There are no stat requirements for any of these Pokemon. For Castform, though, we prefer strong [HP +] Sp. Def., at least average Sp Atk., and not horrible Speed.

## Why are you picking May?
On the second Rival fight [on Route 110], May will lead with Wingull, whereas Brendan leads with Slugma. Wingull is much more difficult to set up [X-attacks] on since it knows Growl.

## Why are you skipping Brawly?
The Brawly fight is essentially unwinnable on our first trip to Dewford[^1]. So, after Flannery, we take Briney's ship back to Petalburg and just fight Brawly at the Dewford pit stop.

## Why don't you perform Wingull manip?[^2]
In Sapphire, all double battles are "optional", whereas in Emerald, all double battles are mandatory trainers if you have multiple Pokemon in your party that can battle. So, catching Wingull early in Emerald would introduce an extra battle
on the Route 104 bridge.

## RNG Manipulations
All RNG manipulations are done with a Save and Quit manip. On a soft reset, the RNG seed is set the save value (the one associated with trainer ID 0). This allows for predictable (and thus manipulable) outcomes.

### Mudkip [+ No encounter to rival 1]
Since IV's and natures are re-generated for the starter Pokemon each frame, Mudkip manip is a frame-perfect (at ~60fps) trick. The best runners will only succesfully perform this manip ~40% of the time.
We extend this manip to avoid encounters on the walk from Littleroot to Route 103 to fight Brendan. The "no encoutner" window is much larger-- 14 frames, or about 0.25 seconds. 

### Chain [Taillow into Abra]
After Roxanne, we "chain" Taillow into Abra on Route 116. This also allows us to skip a Repel, since we can ensure no [other] encounters for all the grass tiles on the way to Rusturf Tunnel.

### Rayquaza
We manipulate both the stats and the Poke Ball throw. This, if executed successfully, saves ~45s to 1 min over grabbing the Master Ball in Aqua Hideout.

The Rayquazas are listed in order of RNG frame, but numbered in terms of quality.

```
1b. 3/30/30/25/12/13 Brave		
1a. 13/25/12/29/28/28 Adamant
4. 28/29/28/23/13/20 Quiet  
3. 20/23/13/11/9/17 Adamant
```

## Footnotes
[^1]: In Pokemon Sapphire, Brawly is actually fought on the first trip. The Brawly fight is more difficult in Emerald because Brawly has an extra Meditite and Makuhita holds a Sitrus Berry, which heals back over half his HP.

[^2]: The Sapphire route catches Wingull before the first Aqua grunt fight in Petalburg Forest as the Fly-er. Wingull is then used on the first Rustboro gym trainer (since it knows Water Gun) and saves over 30 seconds over using Mudkip alone.
