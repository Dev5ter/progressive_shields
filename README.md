### Changes made from Original

1: The Hero's Shield, Wind Waker, Ballad of Gales, Wind's Requiem, and Song of Passing have the option to be randomized.
2: The Hero's Shield and the Mirror shield are progressive exaclty like the bow, swords, picto etc.
3: The Wind Waker can NEVER be in a location that HAS to be recevied in the day, or a mail letter that requires time to pass.
4: Orca - Hit 500 Times (Misc) & Beedles Gold + Silver memberships letters (Expensive Purchases) can hold progressive items.

### About

This is a randomizer for The Legend of Zelda: The Wind Waker.  
It randomizes all the items in the game so that each playthrough is unique and you never know where a particular item will be.  
It also makes the game completely open world from the start, removes most cutscenes from the game, and increases sailing speed and text speed.

**You can download the randomizer here: https://github.com/LagoLunatic/wwrando/releases/latest**

### Information

The randomizer only supports the North American GameCube version of Wind Waker. (MD5: d8e4d45af2032a081a0f446384e9261b)  
The European and Japanese versions of Wind Waker won't work, and neither will Wind Waker HD.

The randomizer guarantees that every playthrough will be completable, and that you don't need to use any glitches or tricks to beat it.

All items are randomized, but because Wind Waker is such a large game, a single run of it would take a very long time if you had to check every single location. Therefore the randomizer has options to limit where progress items can appear based on the type of the location.  
For example, you can limit progress items to appearing in dungeons and secret caves only, or secret caves sidequests and mail, or any other combination you want.  
Location types that you don't select will only have unimportant items that you don't need to beat the game - like rupees, heart pieces, bomb bag upgrades, etc. So you can skip checking them entirely, unless you want some of those optional items.

If you seem to be stuck and can't find anywhere to progress, you should first consult the spoiler log. The spoiler log is generated at the same time as the randomized ISO, and is put in the same folder. It contains information on everything that was randomized in this seed, and lists the order you can get progress items in as well.

If you've consulted the spoiler log and you're still stuck, it's possible you've encountered a bug in the randomizer.  
Please report bugs like that here: https://github.com/LagoLunatic/wwrando/issues  
In the bug report be sure to include the permalink for the seed you encountered the bug on.

If you're going to play on emulator, you should use the latest development version of Dolphin which can be found at the top of this page: https://dolphin-emu.org/download/  
Note that the GameCube boot up animation in Dolphin doesn't work with the randomizer and will cause the game to crash before reaching the main menu. If you have previously set Dolphin up to play that animation you will need to disable it before launching the randomized game by going to Config -> GameCube in Dolphin and checking "Skip Main Menu".  

### Discord Server

If you have any questions or are looking for people to play/race with, why not join the official Wind Waker Randomizer Discord server?  
https://discord.gg/r2963mt

### Credits

The randomizer was created and programmed by LagoLunatic, with help from:  
CryZe (event flag documentation)  
Gamma / SageOfMirrors (custom model conversion, file format documentation)  
Hypatia (textures)  
JarheadHME (additional programming)  
LordNed (file format documentation)  
MelonSpeedruns (game design suggestions, graphic design)  
TrogWW (additional programming)  
nbouteme (additional programming)  
wooferzfg (additional programming)  

### Running the randomizer from source

If you want to run the latest development/beta version of the randomizer from source, follow the instructions below.

Download and install git from here: https://git-scm.com/downloads  
Then clone this repository with git by running this in a command prompt:  
`git clone https://github.com/LagoLunatic/wwrando.git`  

Download and install Python 3.8.2 from here: https://www.python.org/downloads/release/python-382/  
"Windows x86-64 executable installer" is the one you want if you're on Windows, "macOS 64-bit installer" if you're on Mac.  
If you're on Linux, run this command instead: `sudo apt-get install python3.8`  

Open the wwrando folder in a command prompt and install dependencies by running:  
`py -3.8 -m pip install -r requirements.txt` (on Windows)  
`python3 -m pip install -r requirements.txt` (on Mac)  
`python3 -m pip install $(cat requirements.txt) --user` (on Linux)  

Then run the randomizer with:  
`py -3.8 wwrando.py` (on Windows)  
`python3 wwrando.py` (on Mac)  
`python3 wwrando.py` (on Linux)  

Optionally, you can also install `requirements_full.txt` with the same process you used for `requirements.txt` above.  
`requirements_full.txt` will install additional libraries that speed up texture recoloring, as well as for building a distributable version of the randomizer. You can still run the randomizer from source without these.  
