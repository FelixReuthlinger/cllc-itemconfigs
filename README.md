# Create Level and Loot Control (CLLC) item config

This mod contains a set of ItemConfig*.yml files that can be used with 
[CLLC](https://valheim.thunderstore.io/package/Smoothbrain/CreatureLevelAndLootControl/). 
The config contains all new items for Heart and Home, groups them into more detailed groups. 
Also for some other mods I created item lists for some specific versions.

## How to create such item configs

I was using [VNEI](https://valheim.thunderstore.io/package/MSchmoecker/VNEI/) mod, where I 
especially added a new feature to export the indexed items into a CLLC like YAML file.
Using VNEI you don't need to do all the tedious steps of manually editing the item names
(which btw might be localized and by that using displayed names won't work sufficiently),
the mod can create a list of all maybe relevant items, but some things you might want to 
manually still delete, like create attacks (mostly having item type of a one-handed weapon).

## Additional features

The item config file also does contain the settings required to:
* not let you loose equipment and foods on death
* increase stack sizes of all stackable items to double the default size
* decrease the weight of all item to 70% of the original weight
* Epic Loot materials (if the mod is also used) stack sizes are 500% as big as original
* Dragon Eggs can be teleported

## Additional mods supported

* Vanilla (the base game) -> supported version 0.205.5
* EpicLoot -> supported version 0.8.7
* Terraheim -> supported version 2.2.0
* ChaosArmor -> supported version 7.1.0
* DoOrDieMonsters (all the items this mod includes) -> supported version 0.4.1
* Epic Valheim Additions -> supported version 1.2.7
* Sage Robes -> deprecated, will be replaced soon

## Installation

For using the ItemConfig.yaml file, you will need to set the mod to 
use the config file, which is turned off by default.

Search and replace this section below:

```
## Reads the ItemConfig.yml file if present. Configuration done via the YAML file will override the same settings done via the default configuration file. For everything not configured in the YAML file, the default configuration file will still be used.
# Setting type: Toggle
# Default value: Off
# Acceptable values: Off, On
Use item configuration yaml = On
```

## Changelog

* 1.2.2 -> updated vanilla list to valheim version 0.205.5
* 1.2.1 -> using the fixed version for game update on 25th Nov
* 1.2.0 -> added more support to other new mods
* 1.1.0 -> split the item configs into config per mod that added the items; starting to add support for other mods
* 1.0.0 -> first version

## Contact

* https://github.com/FelixReuthlinger/cllc-itemconfigs
* Discord: Flux#0062 (you can find me around some of the Valheim modding discords, too)
