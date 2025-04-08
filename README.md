# Widescreen-ShadowTH


Modified files for proper widescreen support in Shadow The Hedgehog.


Provides widescreen without any UI stretching weirdness or incorrect overlays.


Please note this is already integrated with Shadow The Hedgehog: Reloaded and Shadow SX. This is a standalone widescreen feature if you want to integrate it with your own mod or the original game.

### ROM Validation

Please verify the ROM you are attempting to patch is a 1:1 Shadow The Hedgehog NTSC-U or PAL GameCube ISO.

GCZ/WIA/RVZ or any other format than ISO is not supported. Please convert to ISO, then compare your game to the table below.

You can get your hashes of your ISO by right clicking your game in Dolphin's game list -> `Properties` -> `Verify` tab.

| ROM    | CRC32 Hash    | SHA-1 Hash                               |
| ------ | ------------- | ---------------------------------------- |
| NTSC-U | f582cf1e      | 5dc81ad9c97549394e30bedc252bfa37d4db1de0 |
|  PAL   | db7d8cd9      | 05b34c82c0fe8aa504539e4dfbba89957c7fc788 |


### Patched ROM Output Validation

Below is the expected outputs after patching your original rom to the widescreen version.

| ROM    | CRC32 Hash    | SHA-1 Hash                               |
| ------ | ------------- | ---------------------------------------- |
| NTSC-U | e7bba31d      | 77bf39a056f9ad0fd06d1d8fbc588d1d6ba14aa5 |
|  PAL   | d213e6a0      | 14ba52934be08fc8d49cddd57a0b1ad0ddb16930 |


## Usage / How to Setup

If you are making your own mod...

1. Merge & overwrite files from 'files' with extracted game's 'files'. (See "Extraction of Game" below for how to if you are not familiar)
2. Use the all-in-one (singleplayer only) code below. Do NOT use the xdelta.

If you are just patching the original game and won't be making further dol edits...

1. Download the patch for the region you are using.


[shadow-widescreen-ntsc-u.xdelta](https://raw.githubusercontent.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH/main/shadow-widescreen-ntsc-u.xdelta)


[shadow-widescreen-pal.xdelta](https://raw.githubusercontent.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH/main/shadow-widescreen-pal.xdelta)

2. Use any xdelta3 patcher on your .ISO format game - you're done! No Gecko Codes required, as its embedded in the dol.

### PC
1. Visit https://shadowthehedgehoghacking.github.io/xdelta-wasm/ or any other xdelta3 patcher of your choice.
2. Specify your original ISO as the `Source file`.
3. Specify the `shadow-widescreen.xdelta` file you downloaded as the `Patch file`.
4. Click `Apply Patch`: It will then 'download' the patched file as `ISO NAME-patched.iso` (nothing is actually uploaded/downloaded, it is all done on-device).
5. If you run into errors, likely the ISO is the wrong hash. Double check your original game in `Dolphin Verify` tab.

### Android
1. Download and install the [ROM Patcher](https://github.com/btimofeev/UniPatcher/releases/latest)
2. Place your original ShadowTheHedgehog NTSC-U ROM in ISO format into an accessible folder
3. Download and place the `shadow-widescreen-[region].xdelta` somewhere UniPatcher will be able to access it.
4. Specify the output file & click the pink floating action button.
5. `ISO NAME [PATCHED].iso` should be created successfully. If you run into errors, likely the ISO is wrong hash, double check your original game.

### Gecko (Not required if you use the xdelta)

#### NTSC-U
```
$Advanced Full Widescreen v5 with UI/GNCP Code for NTSC-U [dreamsyntax, Dolphin Wiki]
045F67A0 C1700000
045F67A8 44250000
045F67E0 442F0000
045F67D0 C2600000
045F67F0 C2780000
04343228 4E800020
044AB5CC 42F00000
045F7D4C 40300000
06519F60 00000034
3DC08057 3DE03F40
91EEE098 3DE0BF40
91EEE084 7E0802A6
4E800421 7E0803A6
3DE03F80 91EEE098
3DE0BF80 91EEE084
4E800020 00000000
04036764 484E37FD
0436328C 481B6CD5
04363180 481B6DE1
040BCA54 4845D50D
04345D98 481D41C9
C20BC8D8 00000008
C3629918 81E10094
3E00800B 6210C4B0
7C0F8000 40820028
3DE08057 61EF5F1C
81EF0000 2C0F0002
3DE0804A 61EFB5CC
C36F0000 41820008
FF60D850 00000000
040622A8 484B7CB9
04062300 484B7C61
C249475C 00000003
3DC03F40 91C22000
C2222000 EC110032
D0030004 00000000
C2484334 00000002
3DC04000 91C22000
C0822000 00000000
*Requires .gncp patches from:
*https://github.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH
```

#### PAL Version
```
$Advanced Full Widescreen v5 with UI/GNCP Code for PAL [dreamsyntax, Dolphin Wiki]
C24957AC 00000003
3DC03F40 91C22000
C2222000 EC110032
D0030004 00000000
C2485384 00000002
3DC04000 91C22000
C0822000 00000000
C2306564 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
C2036764 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
C23640D4 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
C2363FC8 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
C20BCE3C 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
C2346BA0 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
04344030 4E800020
045F7828 C1700000
045F7830 44250000
045F7858 C2600000
045F7868 442F0000
045F7878 C2780000
044AC62C 42F00000
045F8DD4 40300000
C20BCCC0 00000008
C3629918 81E10094
3E00800B 6210C898
7C0F8000 40820028
3DE08057 61EF6FDC
81EF0000 2C0F0002
3DE0804A 61EFC62C
C36F0000 41820008
FF60D850 00000000
C2062428 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
C20623D0 00000006
3DC08057 3DE03F40
91EEF158 3DE0BF40
91EEF144 4E800421
3DE03F80 91EEF158
3DE0BF80 91EEF144
60000000 00000000
*Requires .gncp patches from:
*https://github.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH
```


Example of using the common widescreen code (or this one) without the patched csdFiles

## Bad
<img src="https://raw.githubusercontent.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH/main/workspace/res/bad.jpg" align="center" />


Example of using my version of the widescreen code WITH the files:

## Good
<img src="https://raw.githubusercontent.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH/main/workspace/res/good.jpg" align="center" />


### Extraction of Game
1. Get the latest release or dev Dolphin - [Dolphin 2503 or newer recommended](https://dolphin-emu.org/download/)
2. Open Dolphin
3. Set game path to your Shadow the Hedgehog ISO
4. Right-click `Shadow The Hedgehog` in the game list
5. Select `Properties`
6. Select `Filesystem` Tab
7. Right-click `Disc`
9. Select `Extract Entire Disc...`
10. Select a new folder where you will store the game content and modify its files


### Playing the Extracted Game
1. Open Dolphin
2. Open `Config`
3. Select `Paths` Tab
5. Select `Add` for Game Folders
6. Navigate to the folder where you extracted the game
7. Open the `sys` folder, and select "Select Folder"
8. Close the `Config` window. Now your games list should have a new 0 filesize game of Shadow The Hedgehog. The 0 filesize entry is the Extracted game
9. You can now launch the game here if you wish to play in Extracted format


### Converting Extracted Game to ISO (OPTIONAL)
1. Right click the Extracted format game (0 filesize entry) and pick `Convert File...`
2. The Convert window will appear, click "Convert..." and name it `game.iso` for Nintendont, or `Shadow-Widescreen.iso` for Dolphin
3. Move/Save the ISO to the Path Dolphin detects your games. A new full-size entry should appear in your Dolphin game list. Use this when playing the game.
