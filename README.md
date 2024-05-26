# CraftingFilter

Patched for Valheim v0.217.46+

A fork of [aedenthorn/CraftingFilter](https://github.com/aedenthorn/ValheimMods/tree/master/CraftingFilter) 

[ThunderStore](https://thunderstore.io/c/valheim/p/cjayride/CraftingFilter) | [GitHub](https://github.com/cjayride/CraftingFilter_Fork)

## This mod adds a filter to the crafting tab

To filter items, you can use one of three methods: 

1.  Hover over the Craft button and a drop down menu will be shown with item types for available recipes that you can click on to switch filters.
2.  Use the scroll wheel while hovering over the Craft button to switch filters.
3.  Set hot keys or buttons to switch to next or prev filter.

These methods can each be disabled or enabled in the config.  

Individual item types are taken from items themselves so don't blame me if an item has the wrong type.  
  
## Item Categories
  
By default, the mod uses the built in item types to create categories, but you can set up custom categories to group item types together or change the display name of a category. 

To do this, edit the file **BepInEx/plugins/CraftingFilter/categories.json** using the following syntax for each entry:  
  
**\<name>:\<type1>,\<type2>[...]**  
  
Here's an example custom categories.json file:  
  
{  
"categories": [  
"All:None",  
"Resources:Material,Consumable",  
"Weapons:OneHandedWeapon,Bow,Ammo,Hands,TwoHandedWeapon",  
"Armor:Shield,Helmet,Chest,Legs,Shoulder",  
"Misc:Customization,Trophy,Misc,Attach_Atgeir",  
"Tools:Torch,Utility,Tool"  
]  
}  

Any category which has the **None** type in it will show all items.  

Categories are sorted alphabetically with the category with **None** in it at the top.

## Known Issues

Menu items are spaced incorrectly if game is in window mode and not fully expanded. Menu items DO space correctly if the game is in window mode fully expanded, and full-screen mode.

## Configuration

- A config file **BepInEx/config/cjayride.CraftingFilter.cfg** is created after running the game once with this mod.  
- Categories file **BepInEx/plugins/CraftingFilter/categories.json**