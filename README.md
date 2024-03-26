# EnvyAndSpite
**ENVY LEADS TO SPITE**
**SPITE LEADS TO MOTIVATION**
**MOTIVATION LEADS TO ART**

An attempt at making an open source ultrakill level loader and editor...

**Important** 
 8. THE MOD IS A DEAD PROJECT! This means i wont work on it or anything, by releasing the work here on github i wish someone could make a fork continuing my project and seeing how it thrives, The entire idea of this mod is to allow people to get creative in ultrakill, it doesnt matter if im the one who publishes it but i want the project to  be always open source
 1. [Please get this version of unity](https://unity.com/releases/editor/whats-new/2019.4.40)
 1.5 This mod works only in sandbox.
 2. Every enemy by default is set to inactive in the runtime
 2.5 Due to importing prefabs in the sandbox scene, You need to place an enemy on any box collider on the "map" and then rebuild navmesh for all enemies to work
 3. This uses names of gameobjects instead of prefabs (side note: enjoy having to manually select every enemy to see where they are)
 4. Almost every ultrakill enemy spawns from their feet (aka their point of origin IS their feet) so dont place the empty gameobjects in the middle of the air 
 5. Blockers, Powerups, PlayerStart are the only exception to above
 6. For Height references use a default unity cube with the sizes of 4 4 4, that is v1's height in unity or a capsule with 2 2 2
 7. AND MOST OF ALL, BE CREATIVE :D
 
    

# HOW IT WORKS

The mod uses a prefab instead of scenes, so you dont have to manually set every value in the scene itself

basically you need to make a prefab STRICTLY named "MapBase" and then parent every room you want in the map as a child of it you can work on rooms or whatever you can use blender but make sure to use boxes as colliders, anyways once you make your make make sure every walkable surface is a box collider because thats the only one enemies can walk on in ultrakill, anyways to start click on "SPITE" on the toolbar then proceed to make a triggerzone and make sure to set the boxcollider component to the size you actual want, then put the enemies as children of these trigger zones, so they will get activated once the player walks in, Then for waves simpily put it as a child of trigger wave and include enemies AND you can daisy chain this meaning setting another wave as a child of that wave works to make it so the enemies of that child wave get activated when the parent wave ends/ has enemies all dead

# CREDITS 

me, this was a solo project for the most part
eternalunion, the creator of rude of which inspired me to make the project after i got denied access, and also he provided the terminal bundle for me.
