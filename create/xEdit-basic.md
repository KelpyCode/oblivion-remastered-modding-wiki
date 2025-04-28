---
title: Basic edits in xEdit
description: 
published: true
date: 2025-04-28T13:13:39.803Z
tags: 
editor: markdown
dateCreated: 2025-04-28T13:13:39.803Z
---

This is a note on basic property changes for the remaster. Might be useful if you just need to do small changes like weight/cost/enchantments. Don't change names using this method, as AltarESPMain.esp changes all the names in the game to be localization strings that are managed by UE5 side.

# Instructions
1. Install the latest xEdit (4.1.5n as of this guide) from [their Discord server](https://discord.com/invite/5t8RnNQ). Installation folder does not matter, as long as you don't lose it.
2. Boot up xEdit with next arguments:
   `xEdit.exe -TES4R -D:"C:\path\to\OblivionRemastered\Content\Dev\ObvData\Data\" -I:"C:\path\to\OblivionRemastered\Content\Dev\ObvData\Oblivion.ini"`
   -D is the location of Data folder, -I is the location of Oblivion.ini, -TES4R - makes xEdit aware it's remaster.
3. Load Oblivion.esm and all the DLC files.
   ![Screenshot 1](/screenshots/guide1.png)
4. Wait for all the files to load through.
   ![Screenshot 2](/screenshots/guide2.png)
5. Open up the AltarESPMain.esp (on the left) and find the item you want to change. In our case it's an iron shield. Right click the item you want to change and select "Copy as new record into..."
   ![Screenshot 3](/screenshots/guide3.png)
6. Confirm that you know what you're doing.
   ![Screenshot 4](/screenshots/guide4.png)
7. Change the EditorID of the item so it wouldn't conflict. 
   ![Screenshot 5](/screenshots/guide5.png)
8. Select a new .esp file here - we don't want to change the original files.
   ![Screenshot 6](/screenshots/guide6.png)
9. Pick a new name for your mod.
   ![Screenshot 7](/screenshots/guide7.png)
10.  Find your new item and do all the changes you need in DATA section.
    ![Screenshot 8](/screenshots/guide8.png)
11. Return to AltarESPMain.esp records and go to Container section. Find a container you'll find easily. (for example, the Arena chest). Right click the chest and select "Copy as override into..."
    ![Screenshot 9](/screenshots/guide9.png)
12. Select your new .esp file as the destination.
    ![Screenshot 10](/screenshots/guide10.png)
13. Confirm.
    
    ![Screenshot 11](/screenshots/guide11.png)
14. Navigate to your container in your .esp file. Pick Items tab and right click, pick "Add item".
    ![Screenshot 12](/screenshots/guide12.png)
15. Find your item you just updated.
    ![Screenshot 13](/screenshots/guide13.png)
    ![Screenshot 14](/screenshots/guide14.png)
16. Save your file.
    
    ![Screenshot 15](/screenshots/guide15.png)
17. Enable your plugin in ObvData/Data/plugins.txt.
18. Test.

# Credits
silvist for screenshots