# Path Of Exile's Conqueror Influence Tracker

This is a fork of Starloop's PoE-Region-Searcher found here: https://github.com/starloop-miguelferradans/PoE-Region-Searcher
Which was a fork from Fall's Region Search Overlay found here: https://github.com/Fallstreak6/PoE-Region-Searcher
This is a AutoHotKey script to add map tab QoL and save time with atlas progression, and to track influenced
regions automatically, by parsing Path Of Exile's client log.

![picture alt](https://i.imgur.com/LxxPwbT.png)

# Updated Features

* Semi Transparent UI
* Smaller UI with simple corner placement
* Maps in the same order as in game
* Auto loading saved state

# Custom Search

I took this idea from another tool Mappy which can be found here: https://github.com/Nekolike/Mappy

Basically you can set a list of custom searchs at the bottom of the Config.ini file and then use the drop down in the top right to search them.

* Great for cleaning up Quad tabs
* Great for remembering mods you cannot run
* Great for listing the Maps you like best

Just create a list separated by | and they will all be loaded into the dropdown

It's all in a single drop down now but I may add more if this takes off, right now this is just a knock off tool to do what I want


# Automatic Influence Tracking

Every time you encounter a Conqueror in a map, the script UI will update automatically to reflect the new status.

There are five levels of influence status:

* 0: no influence in this region
* 1: Conqueror encountered once
* 2: Conqueror encountered twice
* 3: Conqueror encountered thrice, and his/her Citadel is opened
* 4: Conqueror was defeated and his/her influence cannot be spawned again in this Sirus spawn cycle

When you defeat every Conqueror, the script UI will reset, ready for the new Sirus spawn cycle

## Initial Setup:

The first time you use the script, you will have to modify the Config.ini file, found in the main folder.

Here you will have to update the path to your client log, and the status of your current influenced regions
for each conqueror, follow the explanation from above to set each Conqueror correctly.

After this is done, there is nothing else to do, the script will automatically update the influences when you encounter
the Conquerors in maps.

![picture alt](https://i.imgur.com/bgVsGxk.png)

# Features:

* Click to search your map tab by region. Works in any stash tab with a search bar. (Make sure your stash is open when you do this or nothing will happen, it can check if the game is open but not what you are doing ingame)
* Tracks your influenced regions automatically by parsing Path Of Exile's client log
* Automatic always on top while you play.
* F2 to any Hotkey show/hide interface.