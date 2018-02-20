# Description #
**A combinator that can set the recipe of an assembler (or other machine) based on signal inputs for any and all of your automation needs. There's also a combinator to get recipe ingredients.**

-------------

# How to #

## Crafting Combinator ##
1. Place it facing the machine you want it to work with
2. Configure it in the menu which you can open by clicking on the combinator
3. Connect it to you network
4. Build a [super awesome circuit](https://forums.factorio.com/viewtopic.php?f=193&t=42964) that can craft anything in one assembler :P

The recipes can be signaled in two ways:

1. The resulting item (or fluid) of the recipe, if its name matches the recipes' name
2. A virtual signal generated by this mod found under the 'Crafting combinator recipes' tab

The signal with highest count will be selected.

## Recipe Combinator ##
You can connect your network to it and it will select a recipe (the same way crafting combinator does) from it. Then it will output the recipes ingredients or products, based on the current setting.  
A good way of wiring the recipe combinator is to use one of the red and green connectors for input and the other one for output.

**You can discuss and ask questions on the [forum](https://forums.factorio.com/viewtopic.php?f=93&t=34405)!**

# Localisation #
Thanks to [Nexela](https://mods.factorio.com/mods/Nexela) it is no longer necessary to use the locale mod and everything should have proper locale.

# Credits #
**[LuziferSenpai](https://mods.factorio.com/mods/LuziferSenpai) for the original idea and some of the code.**  
[me](https://mods.factorio.com/mods/theRustyKnife) for the rest of the code.  

-------------

# Changelog #
## 0.9.8 ##
### Changes ###
 - Added compatibility for base game version 0.16

## 0.9.7 ##
### Features ###
 - Added Quarry compatibility ([quarry](https://mods.factorio.com/mods/FuzzCat927/quarry))

## 0.9.6 ##
### Bugfixes ###
 - Fixed a crash with Bottleneck

## 0.9.5 ##
### Features ###
 - Added Omnicompression and Compressed Materials compatibility ([compressor](https://mods.factorio.com/mods/Nexela/compressor), [omnimatter_compression](https://mods.factorio.com/mods/EmperorZelos/omnimatter_compression), [18161](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/18161))
 - Added New Game+ compatibility ([NewGamePlus](https://mods.factorio.com/mods/Bilka/NewGamePlus))
### Bugfixes ###
 - Removed the flashing logistic network warning ([17387](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/17387))

## 0.9.4 ##
### Bugfixes ###
 - Fixed that Bottleneck read mode would get disabled when not appropriate ([34](https://github.com/theRustyKnife/CraftingCombinator/issues/34))

## 0.9.3 ##
### Bugfixes ###
 - Fixed settings being lost when reviving combinators using Picker Extended ([PickerExtended](https://mods.factorio.com/mods/Nexela/PickerExtended))
 - Fixed that the data entities could get placed in large numbers when dragging a blueprint while placing it ([31](https://github.com/theRustyKnife/CraftingCombinator/issues/31))

## 0.9.2 ##
### Bugfixes ###
 - Fixed a crash in the migration script

## 0.9.1 ##
### Features ###
 - Added Omnimatter compatibility ([omnimatter](https://mods.factorio.com/mods/EmperorZelos/omnimatter), [14039](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/14039))
### Bugfixes ###
 - Fixed crash when loading without Bottleneck installe ([14118](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/14118), [28](https://github.com/theRustyKnife/CraftingCombinator/issues/28))

## 0.9.0 ##
### Features ###
 - Crafting combinator can read Bottleneck status ([Bottleneck](https://mods.factorio.com/mods/trold/Bottleneck))

## 0.8.1 ##
### Changes ###
 - Multiply by input count can now be used with find recipes
### Bugfixes ###
 - Negative values are handled properly (not ignored as before)

## 0.8.0 ##
### Features ###
 - Added an option to read crafting speed to crafting combinator
 - Added an option to multiply results by input count to recipe combinator
 - Added a mode to recipe combinator for finding recipes that produce a given item
### Bugfixes ###
 - Fixed modules being carried back to storage in certain cases

## 0.7.2 ##
### Changes ###
 - Moved the refresh rate configuration to mod settings

## 0.7.1 ##
### Bugfixes ###
 - Fixed wrong icon scale for virtual recipe group
 - Fixed recipes that defined complexities would get a virtual signal even if not necessary ([11640](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/11640))
 - Fixed broken localization
 - Enabled sorting virtual recipes into groups

## 0.7.0 ##
### Changes ###
 - Updated for Factorio 0.15

## 0.6.2 ##
### Bugfixes ###
 - Fixed a crash when the root GUI element was clicked ([9454](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/9454))

## 0.6.1 ##
### Bugfixes ###
 - Fixed recipes not being enabled again ([4438](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/4438))

## 0.6.0 ##
### Features ###
 - Settings are saved in blueprints
 - Modules that have been removed due to recipe change can now be requested back into the assembler
 - The multiplier for time in recipe combinator can now be changed to any number
 - Refresh rate is now configurable from in-game, individually for crafting and recipe combinators

## 0.5.2 ##
### Bugfixes ###
 - Removed rocket part signal and made the rocket part item not hidden to prevent flickering issues ([251643](https://forums.factorio.com/viewtopic.php?f=93&t=34405&start=40#p251643))

## 0.5.1 ##
### Bugfixes ###
 - Fixed that module would be moved even when not necessary which caused duplication ([251542](https://forums.factorio.com/viewtopic.php?f=93&t=34405&start=20#p251542))

## 0.5.0 ##
### Changes ###
 - Modules are now moved to overflow if they can't be used with the new recipe
 - Half-finished crafting should now return the ingredients into overflow
 - Crafting and recipe combinators now have seperate refresh rates specifiable in config (GUI coming later)
 - Many minor changes
### Features ###
 - Added configuration GUIs for combinators
 - Added product mode to recipe combinator
 - Added an option to crafting combinator to read recipes from assemblers
 - Added settings copy/paste
 - Added an option to crafting combinator to empty inserters' hands to prevent jamming
 - Added a way to specify what type of chest to use for overflow items and modules

## 0.4.2 ##
### Features ###
 - Added Recycling Machines compatibility ([ZRecycling](https://mods.factorio.com/mods/DRY411S/ZRecycling))

## 0.4.1 ##
### Bugfixes ###
 - Fixed a crash when loading with AAI Programmable Vehicles
 - Fixed some virtual recipes would get the default icon when not necessary

## 0.4.0 ##
### Changes ###
 - Changed the way virtual recipes are generated which should increase compatibilty (by [Nexela](Changed the way virtual recipes are generated which should increase compatibilty))
 - Combinators are color coded now (by [Nexela](Changed the way virtual recipes are generated which should increase compatibilty))
### Features ###
 - Added automatic locale generation (by [Nexela](Changed the way virtual recipes are generated which should increase compatibilty))
 - Added a subgroup for virtual recipes (by [Nexela](Changed the way virtual recipes are generated which should increase compatibilty))

## 0.3.3 ##
### Bugfixes ###
 - Fixed a crash caused by a rounding error in recipe combinator

## 0.3.2 ##
### Bugfixes ###
 - Fixed crash when placing a combinator after reloading a game ([5908](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/5908))

## 0.3.1 ##
### Bugfixes ###
 - Fixed wrong path for no-icon icon and an error in migration script ([5869](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/5869))

## 0.3.0 ##
### Changes ###
 - Completely rewritten code
 - Moved special cases to the locale mod
### Features ###
 - Added support for external special case and icon definitions
 - Added an invisible active provider chest where the items from the assembler are put when recipe changes

## 0.2.2 ##
### Features ###
 - Added crafting time to recipe combinator output (thanks to [LuziferSenpai](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/4654))

## 0.2.1 ##
### Bugfixes ###
 - Fixed a crash when removing a recipe combinator in a new game ([4644](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/4644))

## 0.2.0 ##
### Changes ###
 - Moved localisation into another mod
### Features ###
 - Added recipe combinator (thanks to [Igie](https://mods.factorio.com/mods/theRustyKnife/crafting_combinator/discussion/4421))

## 0.1.4 ##
### Changes ###
 - Changed to work with any and all (hopefully) crafting machine (chemplants, refineries too)
### Features ###
 - Added locale for some mods

## 0.1.3 ##
### Bugfixes ###
 - Recipe for combinator is enabled when the mod is added to the game

## 0.1.2 ##
### Features ###
 - Added a special case system to solve a recipe naming problem
 - Translations for vanilla virtual recipes

## 0.1.1 ##
 - Initial release
