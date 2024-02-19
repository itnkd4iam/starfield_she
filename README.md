![That Troublesome Tarsier](https://i.ibb.co/4f9k0WS/tarsier256x.png)


## STARFIELD SHOPPING HELPER (BETA)

[![Practical use of the Starfield Shopping Helper app](https://img.youtube.com/vi/FIWfARY3gVo/0.jpg)](https://youtu.be/FIWfARY3gVo)

The Starfield Shopping Helper is a Windows PC app that allows you to create a shopping list of any necessary Starfield resources to help build your items/mods and by setting the quantity, you can manage your inventory better as you explore.

Additionally, if you don't have the time to get the resources, the app can generate the necessary console commands for you. This feature can be especially useful if you want to save time and focus on other aspects of the game.

As a bonus, the app can also generate console commands for credits, digipicks, med packs, advanced or legendary (advanced) weapons, superior spacesuits, boost packs and helmets.


### Installation
[![Starfield Shopping Helper app installation](https://img.youtube.com/vi/L5e7R5WUSZk/0.jpg)](https://youtu.be/L5e7R5WUSZk)

Download the ZIPPed source code and supporting files > unzip > create a virtual environment for this app (recommended) and install the required modules:
```
    pip install -r requirements.txt
```

Start the script by typing:
```
    python starfield_she.py
```

A windows binary is also available for download and was compiled using Nuitka. But since the binary is unsigned, some antivirus apps will likely mark the exe as a virus/trojan.


### JSON Data
The app reads the categories and items off the JSON files. To edit the general categories listed by the app, edit the starfield_she_support.ini and look for the "data" key and add/remove the filenames of the JSON that you wish the app to use.

Here's a short description of the available JSON data:
* outpostitems.json - Lists all the equipments/items that can be built in an outpost.
* research.json - Lists all the research projects.
* resources.json - Lists all the resources used in the previous files. This file is necessary for the app to properly display the items and generate the console commands.


### Other JSON Data
* Industrial Workbench (industrialworkbench.json)
    Lists the items produced from the Industrial Workbench. This can help you plan the fabricators you may need in producing certain parts.

* The Goodies (goodies.json)

[![Starfield Shopping Helper app generating weapons and spacesuit](https://img.youtube.com/vi/p9ZGU9-JQpE/0.jpg)](https://youtu.be/p9ZGU9-JQpE)

This will likely appeal to most people 😜 Among other things, this will help you add credits, digipicks, med packs, and create weapons and spacesuit sets. Please note that it's best to run the console commands in a batch file as running all the commands from the console will likely FREEZE/CRASH your game.

The mods for the legendary items are randomized. If you wish to use specific mods (legendary or otherwise), edit the file, look for the weapon/spacesuit you wish to modify and look for the following string pattern: 00AA11BB|22CC33DD|44EE55FF
The "|" is a separator for the set of mods for the app to select from.

For an extensive list of items/mods, refer to spreadsheet created by [TiffanyGaming](https://www.reddit.com/user/TiffanyGaming/):
[https://www.reddit.com/r/Starfield/comments/16fqhac/i_made_a_sheet_with_all_the_legendary_weapon_ids/](https://www.reddit.com/r/Starfield/comments/16fqhac/i_made_a_sheet_with_all_the_legendary_weapon_ids/)


### Known issue
* Creating modded items of similar type (ie Advanced Magshear and Legendary Advanced Magshear) will result in the 1st item not being modded properly. To fix this problem, separate the console commands in 2 different batch files and run them separately.


### Donate
If you'd like to leave a tip, you can follow this [PayPal link](https://www.paypal.com/paypalme/ehalos/1?country.x=PH&locale.x=en_US) or buy one of [my NFTs](https://linktr.ee/iamai_nft) 🙃🙏
