# Installation Instructions
***[DOWNLOADS IN THE RELEASES SECTION](https://github.com/threethan/XCX-Cut-Content-Mod/releases/tag/v1.0)***

On Wii U there are two possible methods (thanks to Abarax!) Both require softmodding your wii u, though file replacement only requires you to boot into homebrew once.
### File Replacement (Cemu or real wii u)
- File replacement will persist unless you manually uninstall the mod
 
     Replacement file size is 34MiB (smaller than the original due to better compression)
### XCXgecko Code (Real wii u only)
 - The gecko code must be applied every time the game is opened, but does not modify any files (Changes to your save will persist, but shouldn't cause any issues even without the mod enabled)
 
     Gecko code doesn't have Full Burst and Air Slash, as they store to your save and don't work properly without the mod. Gecko code is also missing some time trial descriptions, as they don't matter and would be difficult to port. Everything else should work identical to file replacement.
     
     Code file is only 10KiB!

On the Cemu emulator, only file replacement can be used.

## Cemu Method
1. Navigate to your cemu folder (wherever Cemu.exe is)
2. Then go to `mlc01\usr\title\0005000e\`
3. Open `101c4d00`, `10116100` or 101c4c00` ( If none of these exist, either update your game or navigate to the game's folder instead )
4. Open content. There should be a file named `bdat.cpk`
5. Rename this file to `bdat.backup` (optional)
6. Move the modded `bdat.cpk` into this folder, replacing the old one

## Wii U Method 1 - File Replacement
1. Softmod your console. ( I would recommend using the mocha method from [WiiU.hacks.guide](https://wiiu.hacks.guide/#/) )
2. Use a tool like [FTPpii U(https://gbatemp.net/threads/ftpiiu.416907/) to browse your Wii U's storage
3. Open `mlc` (it might be names `storagemlc` or something similar)
4. Navigate to `usr\title\0005000e\`
5. Open `101c4d00`, `10116100` or 101c4c00` (If none of these exist, update your game)
6. Open content. There should be a file named `bdat.cpk`
7. Rename this file to `bdat.backup` (optional)
8. Move the modded `bdat.cpk` into this folder, replacing the old one (the file is fairly small, and shouldn't take long to copy over FTP)

## Wii U Method 2 - Gecko Code
1. Softmod your console. ( [WiiU.hacks.guide](https://wiiu.hacks.guide/#/) )
2. Set up [XCX Gecko](https://github.com/mimicax/XCXGecko/) to modify the game
3. Open Xenoblade X on the WiiU to the title screen
4. Copy the contents of `XCXGeckoCode.txt` into XCXGecko as a custom code and apply it

*Steps 3 & 4 must be repeated every time the game is closed*

**There is a bug where, when using the gecko code, the boss in Chimeric Abomination will be far too big, preventing you from targeting appendages. To fix this use the code `2110A31D 00640064` and restart the time trial**
**The gecko code is missing a few lines of text. Missions will not have descritions and you may see a few placeholder strings. The only fix for this is using the file version, but it does not effect gameplay whatsoever**
