# FRR2 Audio Lag skips

## About
Author: themathgenius

Last updated: 30 July 2024

This document describes outlines the audio lag skips performed in the FireRed Elite 4 Round 2 speedrun.

## What is audio lag?
In the overworld, the game sometimes takes a bit of time to switch between audio tracks (e.g., overworld music to bike music).
This lag will stack if entering a new area while tracks are mid-transition.

As an arbitrary example to try:
1. Start in front of the warden's house [while dismounted] in Fuschia City. 
1. Mount the bike, then immediately enter the warden's house.

Comparing this to just entering the house without mounting, mounting first will be over 0.5s slower.
This can be attributed to the game taking a set amount of time to load the bike track, then another set amount of time to load the Fuschia city track again.
We call this delay "audio lag".

To work around this behavior, we take advantage of track switches that are instant (for example, dismounting the bike).
So before entering a new area or a building, we may perform dismounts or "bike flashes" (where the runner mounts, then immediately
dismounts the bike) to ensure a track is already playing as the new area is supposed to be loaded.
The timesave is maximized in cases where the tracks before and after the transition are the same.

## List of audio lags
No pics yet, I can post them if enough people ask. But runners who have done a few playthroughs of the run should have a good idea of where these are.
 
Unless there's a specific setup listed, assume to just dismount before each listed location/action.
Listed in the approximate order they're done. 

Note: * = also done in any% glitchless
* Rock Tunnel
  * if RTB'ing after Dudley (last hiker), dismount before entering the ladder* 
  * dismount before Dana (last RT trainer) and remount after the fight*
* Route 7-8 Underground tunnel:
  * going up western stairs
* Celadon 1 (Rocket hideout)
  * entering coin case building (if you pick up Eevee)
  * entering the game corner prize shop
  * entering tea building
* Fuschia
  * entering the safari entrance building
* Pewter 2 (old amber, Diglett)
  * entering old amber building
* Cinnabar 1 (Mansion)
  * Bike flash before entering mansion*
  * RTB into the gym (run DR, bike the rest of the way)*. ONLY DO IF NO REPEL UP, OR YOU KNOW THE REPEL WILL WEAR OUT IN THE GYM. 
		THIS SETUP DOES NOT WORK IF THE REPEL WEARS OUT OUTSIDE THE GYM.
* Sevii 1 (Lostelle)
  * Basically every time you re-enter the dock house (same applies for postgame)
  * if you're biking in Pony grass, dismount before teleporting
* Cinnabar 2 (Cinnabar lab)
  * entering Cinnabar lab
* Celadon 2 (Erika)
  * Eevee house if no early Eevee
* Kindle Road (for Mt Ember/Ruby)
  * line up 1 tile left of the last girl swimmer, then take the LHS entrance into Mt ember (biking 1 right + a bunch up).
* Icefall Cave
  * There are a lot of different ones. Here's a [video example](https://youtu.be/Jntyb2hIgs8?t=10677) from pokeguy's 3:27:20.
* Dotted Hole (Six island)
  * Every tile drop (NOT including the initial drop to start the puzzle, since dotted hole music is already loaded)
  * Entering the ladder back up after Gideon takes the Sapphire
* Cerulean Cave
  * bike flash before entering the cave.
 
