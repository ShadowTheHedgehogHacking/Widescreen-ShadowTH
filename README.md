# Widescreen-ShadowTH
Modified files for proper widescreen support in Shadow The Hedgehog (USA GameCube version GUPE8P). 
Provides widescreen without any UI stretching weirdness
Please note this is already integrated with Reloaded. This is just standalone widescreen if you want to integrate it with your own mod or the original game.

## Usage
1. Merge & overwrite files from 'files' with extracted game's 'files'. [You can read how to extract and play/rebuild the game by clicking here.](https://github.com/ShadowTheHedgehogHacking/ShdTH-Reloaded#extraction-of-game--fst-format)
2. Use the all-in-one (singleplayer only) code below.

```
$Advanced Full Widescreen v5 with UI/GNCP Code [dreamsyntax, Dolphin Wiki]
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
*Do not use with Dolphin Widescreen Hack
*Requires .gncp patches from:
*https://github.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH
```


Example of using the common widescreen code (or this one) without the patched csdFiles

## Bad
<img src="https://raw.githubusercontent.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH/main/workspace/res/bad.jpg" align="center" />


Example of using my version of the widescreen code WITH the files:

## Good
<img src="https://raw.githubusercontent.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH/main/workspace/res/good.jpg" align="center" />
