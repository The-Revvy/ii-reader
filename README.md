# ii-Reader
A Wii Homebrew app to inject vpk data into your e-Reader save file.

Requires vpk data named "vpk.bin" in "SD://iireader"

Modify "title.bin" in a hex editor to change the name of the program (maximum 35 characters).

# To obtain vpk.bin

* Obtain a .raw dump of your desired e-Reader card
* Download [nedcenc](https://www.caitsith2.com/ereader/tools/nedcenc.rar) from [caitsith2.com E-Reader Development Tools](https://www.caitsith2.com/ereader/devtools.htm)
* Run the following command 
```
nedcenc.exe -i <input>.raw -o vpk.bin -d
```

Based on GBA Link Cable Dumper v1.6 by FIX94

# Special Shoutouts to:
FIX94

Chishm

Dark Fader

Caitsith2

The e-Reader Crew

# todo
-Add suport for more than just z80 data, should be p easy


# Original README.md
# GBA Link Cable Dumper
A GC and Wii Homebrew App to get GBA BIOS, ROMs and saves via the GC GBA Link Cable.  
Save Support based on SendSave by Chishm.  
GBA BIOS Dumper by Dark Fader.  

# Usage
Grab the release from the "releases" tab above and start up the correct dol file on your GC/Wii.  
Make sure to plug in a GC Controller into Port 1 of your console and the GBA Link Cable into Port 2.  
Now Boot your GBA without a cart inserted, it should automatically boot into the dumper when connected. From there you can just follow the instructions on screen.  
If your GBA resets when you get to the step of inserting a cart, try to boot your GBA with the cart already inserted and holding down start+select on the GBA bootup, this aborts the game launch and should allow the dumper to boot up from there.  
The bin, gba and sav files dumped will be placed in a folder called "dumps" on your main device (SD Gecko on gamecube and SD/USB on Wii). Please note that dumping GBA ROMs can take a long time (32mb takes about 48 minutes) because of the cable protocol limitations, an estimation will be displayed on screen before you dump it as a reference.
