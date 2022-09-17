# liquidctl-aqc - fork for Aquacomputer devices

This repository is a fork of the [liquidctl](https://github.com/liquidctl/liquidctl) project with the intent of supporting various Aquacomputer devices. The end goal is for this fork to cease to exist once all new code and docs end up being merged into the main project. Until that happens, this repo serves as a faster way to iterate and to provide support for Aquacomputer devices earlier.

Main reverse engineering efforts and discussions about the devices are carried out at the [aquacomputer_d5next-hwmon](https://github.com/aleksamagicka/aquacomputer_d5next-hwmon) repository, which holds the hwmon Linux driver for supporting the devices. It's much more likely that any new devices will end up being supported there first, and when their supported features stabilize, they end up being implemented here as well.

## Current level of support

Here is what the is currently supported (roughly), per device:

|        Device/Feature         | Reading sensors | Setting fixed fan speeds | RGB support | Reading/writing fan/sensor labels | Reading/setting fan curves | Setting advanced fan settings (start boost, etc.) | Setting temp offsets for sensors | Support for alarms |
| :---------------------------: | :-------------: | :----------------------: | :---------: | :-------------------------------: | :------------------------: | :-----------------------------------------------: | :------------------------------: | :----------------: |
|  D5 Next (watercooling pump)  |     **Yes**     |         **Yes**          |     No      |                No                 |             No             |                        No                         |                No                |         No         |
| Farbwerk 360 (RGB controller) |     **Yes**     |            /             |     No      |                No                 |             /              |                         /                         |                No                |         No         |
|     Octo (fan controller)     |     **Yes**     |         **Yes**          |     No      |                No                 |             No             |                        No                         |                No                |         No         |
|    Quadro (fan controller)    |     **Yes**     |            No            |     No      |                No                 |             /              |                        No                         |                No                |         No         |

