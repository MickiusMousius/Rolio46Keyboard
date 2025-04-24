# Introduction
The Rolio46 is now at the version 1.1 release! This repo contains all the design files so you can build your own Rolio46.1 or 46.2.

![Rolio46.3](images/main.jpg?raw=true "Rolio46.3")

I will be [opening a store](https://keydio.io) to make it easier for people to make their own Rolio46.1, all of the required parts and sub assemblies will be available for purchase. The main PCBs (AKA shield boards) will be sold with all of the surface mount components pre-soldered.

# Features
The keyboard itself:
- Fully wireless thanks to the awesome [ZMK Project](https://zmk.dev)
- Support for [ZMK Studio](https://zmk.studio/download)
- Excellent battery life, I've personally been getting 4+ weeks before it needs charging
- A low profile, compact choc spaced form factor that is similar to the Corne
- Additional "Sometimes" buttons on the bottom row just like the Sofle
- Horizontal roller encoders on both halves
- A backlight that is efficient enough to be used on battery
- A robust chassis so that it can be treated like a normal keyboard
  - An FDM version for at home low cost at home production
  - A CNC option for a slick look and very premium feel
- A travel case that can easily be made using any FDM printer

ZMK Key map & Custom key caps:
- Up to five memorized bluetooth profiles and a wired mode
- MacOS and Windows layouts as part of the key map to keep the "same" handy behaviors in both OSs
- Able to memorize a specific OS layout for each profile, when you change bluetooth profiles it'll remember whether to use a Windows or MacOS layout
- All of the symbols and special behaviors can be accessed using at most two keys.
- The key caps are fully customized and match the ZMK key map thanks to [FKCaps](https://fkcaps.com/custom/UCR89J?a=KeydioDiscount)
- The settings keys and different modes are documented in the key caps themselves (easy to learn).

  [![Version 1.1 Key Caps](images/key_legend.png?raw=true "Version 1.1 Key Caps")](https://fkcaps.com/custom/UCR89J?a=KeydioDiscount)


# Build Resources
In order to build a Rolio46.1 you will need 5 main sub assemblies, the links below provide information about the different sub assemblies:
 * [The controller](doc/controller.md)
 * [The display](doc/display.md)
 * [The battery](doc/battery.md)
 * [The shield](pcb/README.md)
 * [The chassis](chassis/README.md)

The shield and chassis are the sub assemblies that are most unique to this project, all of the other sub assemblies are fungible.


# Firmware

You can download the latest firmware from here: [Rolio Firmware](https://github.com/MickiusMousius/RolioFirmware)

When you push a change to your fork a GitHub action will create a new firmware build for you.

If you want to do basic layout customization then [ZMK Studio](https://zmk.studio/download) should be all you need.

# Other Components

<ins>Keycaps</ins>

This keyboard has been designed to use MBK caps. You should however be able to use any Choc compatible compatible caps.

You can order a set of custom key caps from a number of possible suppliers too.

I have a design at FKCaps that has the key map of this board integrated into the keys. The link for this key cap set can be found [HERE](https://fkcaps.com/custom/UCR89J?a=KeydioDiscount).


<ins>Switches</ins>

The Rolio46 is designed for use with Choc V1 switches, these can be purchased from many different vendors. My personal favorite switch is the "Choc Sunset" switch.

# Gallery

![](images/case.png)

![](images/all_three.png)
