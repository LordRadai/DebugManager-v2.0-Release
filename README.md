# DebugManager v2.0
This mod has a Discord server dedicated to it!
https://discord.gg/WvEt3eb7uN

NexusMod link:
https://www.nexusmods.com/darksouls2/mods/1241

# Installation
* Unpack the game with [UXM](https://www.nexusmods.com/eldenring/mods/1651)
* Pick the right version of DebugManager, DebugManager.rar if you don't use DS2LightingEngine, or if you use a version up to v0.8.10, pick DebugManager_LE.rar otherwise
* Create a backup of DarkSoulsII.exe

If you don't want to use other DLL mods:
* Rename DebugManager_v2.0.dll to DINPUT8.dll, drag and drop both the DLL, the DebugManager folder, userconfig.properties and the font folder inside the Game folder (where DarkSoulsII.exe is located)

If you use other DLL mods:
* Download [Lazy Loader](https://www.nexusmods.com/darksouls3/mods/677) by ChurchGuard and install by following the mod page instructions
* Drag and drop the DebugManager folder, userconfig.properties and the font folder inside the Game folder (where DarkSoulsII.exe is located)
* Drag and drop DebugManager_v2.0.dll inside the dllMods folder

# Basic Usage
* Press L3 + Start or F10 (can be changed in DebugManager.ini) to toggle the Debug GUI
* Press L3 + R3 to enable Debug Dash. While Debug Dash is active, the player character with move at triple the game's speed and have its gravity entirely disabled
* When any Debug GUI is open, right click in the main game window (outside of GUI windows) to bring up a PopUp menu with some extra actions (such as FPS cap, FPS display)

# Debug Camera
Press L3 + Square to cycle Debug Camera mode. The avaiable modes are:
  * Time stop free cam. Game is paused, you can move the camera.
  * Free cam. Game is running, you can move the camera.
  * Fixed camera. Camera is fixed, game is running and you can control the player character.
While the game is frozen, press Square to advance by one frame.

# Enemy Control Guide
**Attacks**:
DebugManager will map up to 6 of the available inputs for each attack cateogry, which are:
1) Action set 1 (EnemyBehavourFirst)
2) Action set 2 (EnemyBehaviourSecond)
3) Special combat actions, such as ranged attacks (EnemyBehaviourThird)
4) Combo attacks (EnemyComboBehaviour)

Attack sets are bound to the A, B, Y, X, R1/RB, R2/RT, DPAD buttons. The second set is the default set.
Holding down L2/LT will switch over to the third action set (special attacks).
Holding down L1/LB will switch over to the first action set (Action set 1)
Holding down both L1/LB and L2/LT will switch over to the fourth action set (combo attacks)
Releasing any of the above combinations will switch back to the default set.

**Dodge**:
If available, dodges are bound to the directional arrows (DPAD) while the B button is held. One arrow for each direction.
If the character does not perform any dodge actions it's because it doesn't have any.

**Block**:
Holding down L1/LB will put the character in a blocking stance. Letting go of the key will make it so that the character stops blocking.

**Dash**:
Hold B to sprint while NOT holding L1/LB and L2/LT. 

**Jump**:
Press Right Stick (R3) to jump. Contrary to the player character, this works even if the enemy is not moving (it will play a slightly different animation)

**Lock On/Unlock**:
Press Left Stick (L3) to toggle target lock. The character will look for the nearest target it can attack (taking team type into consideration) and use that as a lock on target.
Right now, no kind of visibility tests are performed to determine the lock target, so it will lock on through walls.

**Alt Stance**:
Some enemies have an alternative stance. You can access it by pressing START.

**Weapon Switch**:
You can cycle through the weapons an enemy has available by pressing BACK.

# IMPORTANT NOTES:
* If you move too far away from the player, the controlled enemy will deload
* Some enemies could deal reduced damage if you make them fight against other enemies. This can be changed in CHR_PARAM, through external tools (such as Cheat Engine)

![20240310182413_1](https://github.com/LordRadai/DebugManager-v2.0-Release/assets/22768664/48e8b7eb-c8a4-4ddf-abe9-80c8186f27de)
![20240310182428_1](https://github.com/LordRadai/DebugManager-v2.0-Release/assets/22768664/5ee02245-a576-4250-9f33-3036be299760)
