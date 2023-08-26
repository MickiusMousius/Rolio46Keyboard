# Introduction
I made this project mostly as a way to refresh some skills that I'd not had a chance to use in many years (or simply never had to begin with).

Currently the project is only at a pre-release level, but I felt it was already nice enough to share.

![CNC 0.1 Chassis](images/cnc/main.png?raw=true "CNC 0.1 Chassis")

Version 1.0 is well underway and I believe much closer to achieving my desired goals. Here's a preview:

![Version 1.0 Preview Render](images/preview_v1.png?raw=true "Version 1.0 Preview Render")

The version 1.0 release improves:
- The power switch is easier to operate
- It's much prettier (to me anyway)
- The PCB can have most parts soldered using a hot plate or oven
  - This is important as it makes pre-soldered boards cheaper to produce
  - It simplifies at home production for those with an oven or hotplate
- A set of test points for the backlight has been added to test things before the controller is added
- The CNC chassis has been improved by:
   - Reducing the number of tool changes required to produce it and simplifying tool paths
   - Simplified the production of the damping membranes
   - Simplified end user assembly

### Goals
The primary goal of this project is to provide a compact open source consumer grade backlit split wireless keyboard.

There are a few other secondary reuirements:
- It needs to be able to be assembled at home without highly specialised tools.
- The parts need to be accessible to hobbyists.
- It needs to be easy to modify and fork.
- Ideally it should be easy for "keyboard hobby stores" to sell to hobbyists should there be interest in this keyboard.
- A few price-point options should be available (currently with/without a backlight and FDM or CNC chassis options).


### Inspiration
Inspiration for this project came from the Corne and Sofle keyboards, these are both excellent projects. I have attempted to combine what I believe are the best aspects of both of these keyboards into a single project.

### Features

The keyboard itself:
- Fully wireless thanks to the Nice!Nano controllers and awesome [ZMK firmware](https://zmk.dev)
- Compact portable form factor that is similar to the Corne
- Additional "Sometimes" buttons on the bottom row like the Sofle
- Choc spacing
- Low profile
- A backlight that is efficient enough to be used on battery
- Horizontal rotary encoders
- A robust chassis so that it can be treated like a normal keyboard
  - An FDM version for at home low cost production
  - A CNC option for a slick look and very premium feel
- A travel case that can easily be made using FDM (will be in v1.0)

ZMK Keymap & Custom keycaps:
- The keycaps are fully customised and match the ZMK keymap thanks to fkcaps
- MacOS and Windows modes
- All of the symbols and special behaviours can be accessed using at most two keys
- The settings keys and different modes are more or less documented in the key caps themselves (easy to learn).
- The keymap can be easily customised thanks to ZMK, the keycaps can also be customised to suit you needs
   - Here is a starting point for making your own key caps: [FKCaps](https://fkcaps.com/custom/MKA4FX)

![Version 1.0 Key Caps](images/key_legend.jpeg?raw=true "Version 1.0 Key Caps")


# Making Your Own Rolio

### Electrical Parts

I've provided the links below to the suppliers I purchased my parts from. You can get all of these parts from other suppliers too. I have no affiliation with any of these suppliers.

<ins>PCB</ins>

The PCB for this board can be ordered from JLCPCB or just about any other PCB manufacturer. I have provided pre-prepared zip files for JLCPB.

More information about the PCB can be found in [PCB section](pcb/README.md).

<ins>Required Components</ins>

All of the components in th below table are required to build this keyboard.

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 2    | LiPo Battery, Protected, 801230 (alternatives: 601230, 701230)   | BATT1 | 701230    | [Aliexpress 1](https://www.aliexpress.com/item/1005003667851773.html?spm=a2g0o.order_list.order_list_main.109.675e1802ITKJQ5 ), [Aliexpress 2](  https://www.aliexpress.com/item/1005005386757680.html?spm=a2g0o.order_list.order_list_main.73.675e1802ITKJQ5 )   |
| 48    | 75V 0.15A Fast Switching Diode, SOD-123    | D1-D29    | 1N4148W    | [Aliexpress](https://www.aliexpress.com/item/1005003102614335.html?spm=a2g0o.order_list.order_list_main.13.675e1802ITKJQ5 )    |
| 2  | Nice!Nano Controller  | -    | -    | [Typeractive](https://typeractive.xyz/products/nice-nano)   |
| 2  | Machine sockets and pins | -    | -   | [Typeractive](https://typeractive.xyz/products/machine-sockets-and-pins?_pos=1&_sid=3c03709e0&_ss=r)   |
| 2    | Nice!View Sharp Memory display module  | -  | -  | [Typeractive](https://typeractive.xyz/products/nice-view )  |
| 2    | Surface mount push button switch, generic, two pins    | RESET1   | -   | [Aliexpress](https://www.aliexpress.com/item/1005004297433455.html?spm=a2g0o.order_list.order_list_main.136.675e1802ITKJQ5 ) (I used "Option 4")  |
| 2  | Surface mount DIP Switch, Single Pole Single Throw (SPST) switch, small symbol   | SW4  | -   | [Aliexpress](https://www.aliexpress.com/item/4000685483225.html?spm=a2g0o.order_list.order_list_main.177.675e1802ITKJQ5) |
| 2  | EVQWGD001 Rotary encoder, dual channel, incremental quadrate outputs, with switch  | RE_1  | EVQWGD001  | [Aliexpress](https://www.aliexpress.com/item/32990950196.html?spm=a2g0o.detail.0.0.d848ibGnibGnWq&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=a7670640-8b96-4c08-a45e-ac785f25eb7d&_t=gps-id:pcDetailTopMoreOtherSeller,scm-url:1007.40050.354490.0,pvid:a7670640-8b96-4c08-a45e-ac785f25eb7d,tpp_buckets:668%232846%238114%231999&pdp_npi=4%40dis%21AUD%2110.27%218.31%21%21%216.46%21%21%40210321dc16943086866475019e3a72%2112000016374535112%21rec%21AU%21192529469%21S ) |
| 46  | Kailh Choc hot swap sockets PG1350 | - | -  | [Aliexpress](https://www.aliexpress.com/item/1005003916481415.html?spm=a2g0o.store_pc_allProduct.8148356.63.1a497474I4Gojr&pdp_npi=3%40dis%21AUD%21AU%20%245.45%21AU%20%243.77%21%21%21%21%21%40210318b916943096379284692e935a%2112000027459452033%21sh%21AU%21192529469) |
| 46 | Kailh Choc Switches  | -  | -  | [Aliexpress](https://www.aliexpress.com/item/1005005446722280.html?spm=a2g0o.order_list.order_list_main.97.675e1802ITKJQ5 )  |

<ins>Optional Backlight Components</ins>

The parts in the below table are only needed for the backlight, if you do not want a backlight they can be ommitted from you build to save some money.

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 2   | 30V Vds, 5.7A Id, N-Channel MOSFET, SOT-23  | Q1   | AO3400A   | [Aliexpress](https://www.aliexpress.com/item/4000338838713.html?spm=a2g0o.order_list.order_list_main.131.675e1802ITKJQ5)  |
| 2 | 0805 Surface mount resistor  | R1  | 470Ω  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 2 | 0805 Surface mount resistor  | R2  | 10kΩ  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 2 | 0805 Surface mount resistor  | R3-R25 | 680Ω  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 46  | 0805 Surface mount LED  | LED1 - LED23  | - | [Aliexpress](https://www.aliexpress.com/item/1005004341345794.html?spm=a2g0o.order_list.order_list_main.25.675e1802ITKJQ5 )  |


### Other Parts

<ins>Chassis</ins>

The chassis can be made using either FDM or CNC.

Further information about making (or ordering) your own chassis can be found in the [Chassis Section](chassis/README.md).

<ins>Keycaps</ins>

This keyboard has been designed to use MBK caps. You should however be able to use any Choc compatible (including choc spacing) compatible caps.

You can order a set of custom keycaps from a number of possible suppliers too.

I have a design at FKCaps that has the keymap of this board integrated into the keys. The link for this key cap set can be found [HERE](https://fkcaps.com/custom/MKA4FX).

<ins>General Hardware</ins>

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 8  | 9mm Silicone Feet | -  | - | [Aliexpress](https://www.aliexpress.com/item/1005005504977168.html?spm=a2g0o.order_list.order_list_main.67.675e1802ITKJQ5 )  |
| 10 | M2x4mm Screws | -  | -  | [Aliexpress](https://www.aliexpress.com/item/32810872544.html?spm=a2g0o.productlist.main.1.764965e5UFrGqL&algo_pvid=c5686b2b-d8dd-403c-b107-a5b601dd8758&algo_exp_id=c5686b2b-d8dd-403c-b107-a5b601dd8758-0&pdp_npi=4%40dis%21AUD%212.42%211.67%21%21%211.52%21%21%402103209516943107919815919eb511%2112000026955302078%21sea%21AU%21192529469%21S&curPageLogUid=TCVQaWi3Sbah)  |



### Firmware

You can download the latest firmware from here: 

Fork the following repository: [RolioFirmware](https://github.com/MickiusMousius/RolioFirmware)

When you push a change to your fork a GitHub action will create a new firmware build for you.


### Assembly

TODO: Make some assembly instructions.

Assembly notes (pre-release version):
 - Solder the top resistors first, then the LED's, then the pther surface mount parts
 - The height of the controller and display are very important to fitting everything nicely into the chassis, make sure everything is flush and seated all the way.
 - Be sure to trim the legs of any through hole components after soldering, as above, the clearances are very important.


