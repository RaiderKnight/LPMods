NPC Manager ReadMe, Change Log and TODO List
=============================================

ReadMe
********
Thanks for downloading the NPC manager! Read this or be doomed!

Let me first explain how NPCs work in LifePlay so you know what you are doing:

LifePlay distincts between normal NPCs and relatives. 
Later are part of your family and have other attributes / relations 
to you as normal NPCs. For example relatives can live with you, normal 
NPCs can't. (True for LP 3.17, may change in the future.)

This is why relatives are handeled different from normal NPCs in the manager. 
They have their own menu.

A "normal" NPC on the other hand can either be temporary or permanent. 
Temporary means it was created in a scene (like "Call hooker") and will not 
exist any longer after the scene exists.

Q: So, the NPC manager cannot deal with temporary NPCs, right?
A: Yep. You got it!


What is this?
~~~~~~~~~~~~~

This little tool can help you to
- Set relationships between NPCs, relatives and/or the player (MC)
- Find 'lost' NPCs and add them to your contacts
- Delete all NPCs not in your contacts (To increase game performance)
- Delete ALL NPCs (even your contacts)
- Delete ALL Relatives


Usage
~~~~~

You can find the manager in the "PC" menu, if the mod is enabled. Look for 
"Open NN NPC Manager" item.

For most actions you need to specify at least one NPC target. (Usally target1)
The second target slot will automatically set to the player, but you may
change this.

Please ensure to always use Player as "target2".
This tool does not contain any sanity checks. So if you set inapropriate 
targets and your game breaks... good work!

Find by Name
~~~~~~~~~~~~

The find by name function can look for a specific NPC by its name.
The name must be correctly spelled. The search is case insensitive.
If you do not know the name you may use * as a placeholder. 
You can also do first name = "*", last name = "Smith" for example.

The NPC Manager will then list each NPC it finds.
It will print a message every 15 NPCs so you know its still working.


WARNING
~~~~~~~

*None* of the changes the NPC Manager does can be undone.
So... guess what: Save before using it!

Some tasks run a little longer, depending on the amount of NPCs 
in your savegame and your computers performance.

F A Q
~~~~~

Q: How do I know how many NPCs are in the game but not my contacts?
A: You can use the COUNT NPCs action of the batch processing feature.
A2: If you want to know them all search for name = "*". This will spit out any NPC in your savegame.

Q: I did something I want undone. How?
A: You did not read this readme right? Go up 18 lines and read again. 

Change Log
************

Version 1.6 (15.01.2021):
- Added "had sex with" filter to batch processing
- Build and checked using Rizean's lp-builder https://github.com/Rizean/lp-builder 
    -> Thanks mate!

Version 1.5 (05.01.2021):
- First F95 version
- Added batch processing (list, delete, tag, untag, add to contacts, impregnate, stop pregnancy) for NPCs matching certain criteria
    - Tagging will add the fixed tag 'NPCMGR' to the NPCs. 
    (As tagging API does not accept string parameters as of LP 3.17.)
    
    You could change that tag in the nn_npc_mgr.lpscene file.
    (Search for the tag name 'NPCMGR' and replace it with whatever you want. 
    Leave the tag_ prefix intact!)
- Increased status counter from 'every 15' to 'every 30' so you won't get spammed... :)

Version 1.4 (03.01.2021):
- Added sugar babe support (base game)
- Added option to make relatives live with player (or not)
- Removed living with player option for normal NPCs as it is not working in LP atm.

Version 1.3 (02.01.2021):
- Added last name search
- Added status update in name search and total count. 
 - The stauts update triggers every 15 searched NPCs and is required to make LP not terminate the script.
 
Version 1.2 (30.12.2020):
- Allow selection of Players related NPCs as targets (like land lord, PT, Boss, ...)
- Changes some item texts
- Added "RETURN" option to NPC-NPC relations menu

Version 1.1 (22.12.2020):
- Added option to delete ALL NPCs from game
- Fix: Menu was not working correctly

Version 1.0 (19.12.2020):
- First public release

TODOs (Planned features by NickNo)
************************************
- Support adding new relatives to the player

Feature Requests (Requested by others)
****************************************
- Support poly relationships https://f95zone.to/threads/lifeplay-v3-18-vinfamy.11321/post-4873438

Developer & Tester Notes
**************************

Thanks to AlexWolfTheBest for the feedback and feature requests ;)
