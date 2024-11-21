# Wii Guitar Hero Debug Menu

### Note: Warriors of Rock is absent. This is because there is currently no known way to access the debug menu in any way on that game on Wii. If a way is found, janky or not, the files will be added.

You will need a Wii ISO manipulation tool such as Wiimms ISO Tools. You might have to overcome your commandlinephobia for this one.

You can get it here: https://wit.wiimm.de/

Don't forget to change any of the strings in quotes. For this example, we will use the best game in the series Guitar Hero Smash Hits.


* Get the game's qb.pak.ngc file from this repository

* Dump your legally acquired copy of the game you want or acquire a totally legal copy from a fellow named John "Arby" https://bit.ly/ArbysHasTheMeats (yes that is his last name) (yes we hate piracy here)

* Open a terminal in the folder where your game dump is located, and run this command:
```
  wit extract "Guitar Hero - Smash Hits (USA) (En,Fr).wbfs" "hits_ext/"
```

Once that's done running, you will have a folder with your game files.

* Open said folder, go in files/pak/ and drag in the qb.pak.ngc file you downloaded in there

* Open Dolphin Emulator, click Open, navigate to your folder with your extracted files, go in sys/ and double click on main.dol to run the game

Enjoy!

## Any issues running the game (aerosmith probably) or you want to run this on real hardware?

Try building it into an ISO with the steps below:

* Navigate where your folder with your ISO is located

* Open a terminal in that folder, and run this command:
```
  wit copy "hits_ext/" "smash_hits_debug.iso"
```

Once that's done running, you will have an ISO file that can be added to your hard drive with your other Wii games.

* **(OPTIONAL)** If you wanna have both the stock and debug ISOs, you can change the name and and disc ID of your debug ISO by adding these arguments to the command above:
```
  --name="Guitar Hero Smash Hits Debug" --id="SXCE01"
```

Disc IDs are usually formatted like ABCD12, I don't know if this works if it's formatted in any other way. Using the original disc ID but changing the last two characters to 01 works totally fine.
You are also free to only have a debug copy on your hard drive as you don't lose much playability compared to stock GH.

All done!
