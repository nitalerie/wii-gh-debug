# Wii Guitar Hero Debug Menu

## Note: Warriors of Rock is absent. This is because there is currently no known way to access the debug menu in any way on this game on Wii. If a way is found, janky or not, the files will be added.

You will need a Wii ISO manipulation tool such as WiiScrubber (old and kinda sucks but has a GUI) or Wiimms ISO Tools (command line only but works very well)
You can get it here: https://wit.wiimm.de/
I will only be covering how to use the QBs with WIT

1. Get the game's qb.pak.ngc file from this folder

2. Dump your legally acquired copy of the game you want or acquire a totally legal copy from a fellow named John "Arby" https://bit.ly/ArbysHasTheMeats (yes that is his last name) (yes we hate piracy here)

3. Open a terminal in the folder where your game dump is located, and run this command:
  wit extract "CHANGE ME THIS IS THE FILE NAME OF YOUR GAME ISO" "CHANGE ME TOO THIS WILL BE THE NAME OF THE FOLDER WHERE YOUR EXTRACED ISO'S FILES WILL BE"

Once that's done running, you will have a folder with your game files.

4. Open said folder, go in files/pak/ and drag in the qb.pak.ngc file you downloaded in there

5. Open Dolphin Emulator, click Open, navigate to your folder with your extracted files, go in sys/ and double click on main.dol to run the game

Enjoy!
If you want an ISO you can use on real hardware, there are some more steps you need to take:

6. Navigate where your folder with your ISOs is located

7. Open a terminal in that folder, and run this command:
  wit copy "CHANGE ME THIS IS THE NAME OF THE FOLDER WHERE YOUR EXTRACED ISO'S FILES ARE" "CHANGE ME TOO THIS IS THE NAME OF YOUR ISO WITH THE NEWLY ADDED DEBUG FUNCTIONALITIES.iso"

Once that's done running, you will have an ISO file that can be added to your hard drive with your other Wii games.

7.5. If you wanna have both the stock and debug ISOs, you can change the name and and disc ID of your debug ISO by adding these arguments to the command above:
  --name="change me" --id="CHNGME"

Disc IDs are usually formatted like ABCD12, I don't know if this works if it's formatted in any other way. Honestly just get the original disc ID and change the last two characters to 01 or something lol
Also since the menu that appears when you press select doesn't exist on Wii it's not that big of a deal to not have a stock copy on your hard drive.

All done!
