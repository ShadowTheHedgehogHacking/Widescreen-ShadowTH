# Widescreen-ShadowTH
Modified files for widescreen support in Shadow The Hedgehog. Mainly modifications to GNCPs

## Usage
1. Merge & Overwrite files from 'csdFiles' with extracted game's csdFiles
2. Use relevant gecko-codes-widescreen-patches.txt codes or use the all-in-one (singleplayer only) code here:

```
$Advanced Full Widescreen v3 with UI/GNCP Code [dreamsyntax, Dolphin Wiki]
045f67a0 c1700000
045f67a8 44250000
045f67e0 442f0000
045f67d0 c2600000
045f67f0 c2780000
c20622a8 00000006
3dc08057 3de03f40
91eee098 3de0bf40
91eee084 4e800421
3de03f80 91eee098
3de0bf80 91eee084
60000000 00000000
c2062300 00000006
3dc08057 3de03f40
91eee098 3de0bf40
91eee084 4e800421
3de03f80 91eee098
3de0bf80 91eee084
60000000 00000000
c249475c 00000003
3dc03f40 91c22000
c2222000 ec110032
d0030004 00000000
c2484334 00000002
3dc04000 91c22000
c0822000 00000000
c2036764 00000006
3dc08057 3de03f40
91eee098 3de0bf40
91eee084 4e800421
3de03f80 91eee098
3de0bf80 91eee084
60000000 00000000
c236328c 00000006
3dc08057 3de03f40
91eee098 3de0bf40
91eee084 4e800421
3de03f80 91eee098
3de0bf80 91eee084
60000000 00000000
c2363180 00000006
3dc08057 3de03f40
91eee098 3de0bf40
91eee084 4e800421
3de03f80 91eee098
3de0bf80 91eee084
60000000 00000000
c20bca54 00000006
3dc08057 3de03f40
91eee098 3de0bf40
91eee084 4e800421
3de03f80 91eee098
3de0bf80 91eee084
60000000 00000000
c2345d98 00000006
3dc08057 3de03f40
91eee098 3de0bf40
91eee084 4e800421
3de03f80 91eee098
3de0bf80 91eee084
60000000 00000000
*Disable Simple Widescreen by LimblessVector if you use this.
*Requires .gncp patches from:
*https://github.com/ShadowTheHedgehogHacking/Widescreen-ShadowTH
*All inclusive code for Single Player only!
```

# Reloaded II Mod Loader
This mod has compatibility with Realoded II, the universal mod loader created by Sewer56/Sewer56lol. To use this port you first need to follow the instructions below.

1. Go to your Dolphin Emulator and right-click in your Shadow The Hedgehog game:
![image](https://user-images.githubusercontent.com/50070802/181631182-7da7fe3e-61f8-47b2-9eec-0eb39249c686.png)

2. Go to the Filesystem, right-click in the Disk icon/"Disc - GUPE8P" and then click in "Extract Entire Disk...":
![image](https://user-images.githubusercontent.com/50070802/181631536-f6e22e30-a5de-460c-9d9d-7e3c5e8325b8.png)

3. After that, you'll have to create a folder called "SHADOWTHEHEDGEHOG". Make sure the new folder is next to your Dolphin.exe:
![image](https://user-images.githubusercontent.com/50070802/181631957-d657cfbd-52dc-48a4-b852-bb881fffe050.png)
![image](https://user-images.githubusercontent.com/50070802/181632036-fa6501ad-5448-4291-a179-2f5e695dea12.png)

4. Wait until the process is finished:

![image](https://user-images.githubusercontent.com/50070802/181632175-7566283e-6254-4ffc-b02e-a4ac6e991e7f.png)

5. Open Reloaded II and add your "Dolphin.exe" to the mod loader:
![image](https://user-images.githubusercontent.com/50070802/181632500-9e49515a-83bf-47b9-a827-28ab7ee9d6da.png)
![image](https://user-images.githubusercontent.com/50070802/181632731-5e1f85c3-e15b-4718-acf8-f2c0fdd6c242.png)

6. Click on "Edit Application" and add the following Argument Command:

<b>-b -e "Your Dolphin Emulator folder loaction\SHADOWTHEHEDGEHOG\sys\main.dol"</b>
![image](https://user-images.githubusercontent.com/50070802/181632991-b842a465-ade5-4042-b50e-0bfa550b6377.png)
![image](https://user-images.githubusercontent.com/50070802/181633143-bf4222e3-cc1b-4e09-865e-8f97436e5ac2.png)

7. Download "shadowthehedgehog.guis.widescreenrevamp" and extract with the same name as in the zip file in Reloaded's "mods" folder:
![image](https://user-images.githubusercontent.com/50070802/181634398-c702f2ca-cd4e-4716-a198-844a46f46c0d.png)

8. If the mod is not in the game's list, go to the Manage Mods tab on Reloaded II, serach for the mod and enable the option for "dolphin.exe" or in this case for Shadow The Hedgehog:
![image](https://user-images.githubusercontent.com/50070802/181634660-4524d65f-de03-433c-b2f8-d38d3b80d50c.png)

9. Enable the mod by going to your game tab on R-II and check the box:
![image](https://user-images.githubusercontent.com/50070802/181636292-f41666b9-7404-42e5-8df4-8555149bbdcb.png)

10. Go back to Reloaded II's "mods" folder and go to the extracted folder (named shadowthehedgehog.guis.widescreenrevamp). Inside you'll see a text file with Gecko Codes, you need to put those in your game's Gecko Codes tab on Dolphin Emulator:
![image](https://user-images.githubusercontent.com/50070802/181635814-8bc4528b-ced8-4354-ac4a-c90ccf66b22d.png)

11. Save everything and have fun playing Shadow The Hedgehog with Reloaded II support!
