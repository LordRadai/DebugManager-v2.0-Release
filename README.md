# DebugManager-v2.0-Release
Public release of DebugManager v2.0

# Installation
* Create a backup of DarkSoulsII.exe
* Download PatchOnClick (https://www.2brightsparks.com/onclick/) and install it
* Open PatchOnClick.exe, select Patch a file. Select the game's executable (DarkSoulsII.exe), click Open, then select debug_patch.poc. If done correctly, a new exe file should be created. Replace DarkSoulsII.exe with the new .exe just created

If you don't want to use other DLL mods:
* Rename DebugManager_v2.0.dll to DINPUT8.dll, drag and drop both the DLL and the DebugManager folder inside the Game folder (where DarkSoulsII.exe is located)

If you use other DLL mods:
* Download Lazy Loader by ChurchGuard (https://www.nexusmods.com/darksouls3/mods/677) and install by following the mod page instructions
* Drag and drop the DebugManager folder inside the Game folder, where DarkSoulsII.exe is
* Drag and drop DebugManager_v2.0.dll inside the dllMods folder

If done correctly, when you open the game you should see a watermark in the top right corner of the game's window (DebugManager vX.X by Radai)

# Enemy Control Guide
When you take control of an enemy, it will switch its movement type to side walk. This is done because turn logic is jank and I have other priorities right now.

Attacks:
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

Dodge:
If available, dodges are bound to the directional arrows (DPAD) while the B button is held. One arrow for each direction.
If the character does not perform any dodge actions it's because it doesn't have any.

Block:
Holding down L1/LB will put the character in a blocking stance. Letting go of the key will make it so that the character stops blocking.

Dash:
Hold B to sprint while NOT holding L1/LB and L2/LT. 

Jump:
Press Right Stick (R3) to jump. Contrary to the player character, this works even if the enemy is not moving (it will play a slightly different animation)

Lock On/Unlock:
Press Left Stick (L3) to toggle target lock. The character will look for the nearest target it can attack (taking team type into consideration) and use that as a lock on target.
Right now, no kind of visibility tests are performed to determine the lock target, so it will lock on through walls.

Alt Stance:
Some enemies have an alternative stance. You can access it by pressing START.

Weapon Switch:
You can cycle through the weapons an enemy has available by pressing BACK.

IMPORTANT NOTES:
* If you move too far away from the player, the controlled enemy will deload
* Some enemies could deal reduced damage if you make them fight against other enemies. 
