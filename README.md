# Introduction
Currently the project is still at a pre-release level, this is the second update, putting it at 0.9, once again I felt it was nice enough to share.

![CNC 0.9 Example](images/cnc/cnc_2.jpg?raw=true "CNC 0.9 Example")
![FDM 0.9 Chassis](images/fdm/fdm_3.jpg?raw=true "FDM 0.9 Chassis")

Version 1.0 is well underway, the PCBs are already in the mail and the CAD models are ready for me to print and test.

Inspiration for this project came from the [Corne](https://github.com/foostan/crkbd) and [Sofle](https://github.com/josefadamcik/SofleKeyboard) keyboards, these are both excellent projects. I have attempted to combine what I believe are the best aspects of both of these keyboards into a single project.

I've had several people ask if I would be willing to sell them one of the prototype boards. Whilst I don't think the prototypes are good enough, I feel that the 1.0 version very probably will be good enough. With that in mind I am considering opening an online store to sell some of these, though this will likely be at quite low volumes.

### Features
The keyboard itself:
- Fully wireless thanks to the Nice!Nano controllers and awesome [ZMK firmware](https://zmk.dev)
- Excellent battery life, I've personally been getting 2+ weeks before it gets to 60%
- A low profile, compact choc spaced form factor that is similar to the Corne
- Additional "Sometimes" buttons on the bottom row just like the Sofle
- Horizontal roller encoders on both halves
- A backlight that is efficient enough to be used on battery
- A robust chassis so that it can be treated like a normal keyboard
  - An FDM version for at home low cost production
  - A CNC option for a slick look and very premium feel
- A travel case that can easily be made using any FDM printer

ZMK Keymap & Custom keycaps:
- Up to five memorized bluetooth profiles and a USB mode
- The keycaps are fully customized and match the ZMK keymap thanks to [FKCaps](https://fkcaps.com/custom/FGE2DW)
- MacOS and Windows modes as part of the keymap to keep the "same" handy macros in both OSs
- All of the symbols and special behaviors can be accessed using at most two keys
- The settings keys and different modes are documented in the key caps themselves (easy to learn).
- The keymap can be easily customized thanks to ZMK, the keycaps can also be customized to suit your needs
   - Here is a starting point for making your own key caps: [FKCaps](https://fkcaps.com/custom/FGE2DW)

[![Version 1.0 Key Caps](images/key_legend.png?raw=true "Version 1.0 Key Caps")](https://fkcaps.com/custom/FGE2DW)


### Goals
The primary goal of this project is to provide a compact open source backlit split wireless keyboard.

There are a few other secondary requirements:
- It needs to be able to be assembled at home without highly specialized tools.
- The parts need to be accessible to hobbyists.
- It needs to be easy to modify and fork.
- Ideally it should be easy for "keyboard hobby stores" to sell to hobbyists should there be interest in this keyboard.
- A few price-point options should be available.

<br/>
<br/>


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
| 2  | Nice!Nano Controller  | -    | -    | [Typeractive](https://typeractive.xyz/products/nice-nano) |
| 2  | Machine sockets and pins | -    | -   | [Typeractive](https://typeractive.xyz/products/machine-sockets-and-pins?_pos=1&_sid=3c03709e0&_ss=r)   |
| 2    | Nice!View Sharp Memory display module  | -  | -  | [Typeractive](https://typeractive.xyz/products/nice-view )  |
| 2    | Surface mount push button switch, generic, two pins    | RESET1   | -   | [Aliexpress](https://www.aliexpress.com/item/1005004297433455.html?spm=a2g0o.order_list.order_list_main.136.675e1802ITKJQ5 ) (I used "Option 4")  |
| 2  | Surface mount DIP Switch, Single Pole Single Throw (SPST) switch, small symbol   | SW4  | -   | [Aliexpress](https://www.aliexpress.com/item/4000685483225.html?spm=a2g0o.order_list.order_list_main.177.675e1802ITKJQ5) |
| 2  | EVQWGD001 Rotary encoder, dual channel, incremental quadrate outputs, with switch  | RE_1  | EVQWGD001  | [Aliexpress](https://www.aliexpress.com/item/32990950196.html?spm=a2g0o.detail.0.0.d848ibGnibGnWq&gps-id=pcDetailTopMoreOtherSeller&scm=1007.40050.354490.0&scm_id=1007.40050.354490.0&scm-url=1007.40050.354490.0&pvid=a7670640-8b96-4c08-a45e-ac785f25eb7d&_t=gps-id:pcDetailTopMoreOtherSeller,scm-url:1007.40050.354490.0,pvid:a7670640-8b96-4c08-a45e-ac785f25eb7d,tpp_buckets:668%232846%238114%231999&pdp_npi=4%40dis%21AUD%2110.27%218.31%21%21%216.46%21%21%40210321dc16943086866475019e3a72%2112000016374535112%21rec%21AU%21192529469%21S ) |
| 4  | 0805 Surface mount capacitors  | C1, C2  | 100nF  | [Aliexpress](https://www.aliexpress.com/item/32888863725.html?spm=a2g0o.productlist.main.1.421ed7d7TDWEJj&algo_pvid=64889c03-7048-4b0c-b35b-564d9069f833&algo_exp_id=64889c03-7048-4b0c-b35b-564d9069f833-0&pdp_npi=4%40dis%21AUD%215.93%215.34%21%21%213.72%21%21%402101e9d116966657566622481e9c98%2110000000070124058%21sea%21AU%21192529469%21&curPageLogUid=FUlprN51Ouc7) |
| 46  | Kailh Choc hot swap sockets PG1350 | - | -  | [Aliexpress](https://www.aliexpress.com/item/1005003916481415.html?spm=a2g0o.store_pc_allProduct.8148356.63.1a497474I4Gojr&pdp_npi=3%40dis%21AUD%21AU%20%245.45%21AU%20%243.77%21%21%21%21%21%40210318b916943096379284692e935a%2112000027459452033%21sh%21AU%21192529469) |
| 46 | Kailh Choc Switches  | -  | -  | [Aliexpress](https://www.aliexpress.com/item/1005005446722280.html?spm=a2g0o.order_list.order_list_main.97.675e1802ITKJQ5 )  |

<ins>Optional Backlight Components</ins>

The parts in the below table are only needed for the backlight, if you do not want a backlight they can be omitted from your build to save some money.

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 2   | 30V Vds, 5.7A Id, N-Channel MOSFET, SOT-23  | Q1   | AO3400A   | [Aliexpress](https://www.aliexpress.com/item/4000338838713.html?spm=a2g0o.order_list.order_list_main.131.675e1802ITKJQ5)  |
| 2 | 0805 Surface mount resistor  | R1  | 470Ω  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 2 | 0805 Surface mount resistor  | R2  | 10kΩ  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 46 | 0805 Surface mount resistor  | R3-R25 | 680Ω  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 46  | 0805 Surface mount LED  | LED1 - LED23  | - | [Aliexpress](https://www.aliexpress.com/item/1005004341345794.html?spm=a2g0o.order_list.order_list_main.25.675e1802ITKJQ5 )  |


### Other Parts

<ins>Chassis</ins>

The chassis can be made using either FDM or CNC.

Further information about making (or ordering) your own chassis can be found in the [Chassis Section](chassis/README.md).

<ins>Keycaps</ins>

This keyboard has been designed to use MBK caps. You should however be able to use any Choc compatible (including choc spacing) compatible caps.

You can order a set of custom keycaps from a number of possible suppliers too.

I have a design at FKCaps that has the keymap of this board integrated into the keys. The link for this key cap set can be found [HERE](https://fkcaps.com/custom/FGE2DW).

<ins>General Hardware</ins>

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 8  | 9mm Silicone Feet | -  | - | [Aliexpress](https://www.aliexpress.com/item/1005005504977168.html?spm=a2g0o.order_list.order_list_main.67.675e1802ITKJQ5 )  |
| 10 | M2x4mm Screws | -  | -  | [Aliexpress](https://www.aliexpress.com/item/32810872544.html?spm=a2g0o.productlist.main.1.764965e5UFrGqL&algo_pvid=c5686b2b-d8dd-403c-b107-a5b601dd8758&algo_exp_id=c5686b2b-d8dd-403c-b107-a5b601dd8758-0&pdp_npi=4%40dis%21AUD%212.42%211.67%21%21%211.52%21%21%402103209516943107919815919eb511%2112000026955302078%21sea%21AU%21192529469%21S&curPageLogUid=TCVQaWi3Sbah)  |



### Firmware

You can download the latest firmware from here: [releases](https://github.com/MickiusMousius/RolioKeyboard/releases)

If you want to customise the firmware (or your keymap) fork the following repository: [RolioFirmware](https://github.com/MickiusMousius/RolioFirmware)

When you push a change to your fork a GitHub action will create a new firmware build for you.


### Assembly

TODO: Make some assembly instructions.

Assembly notes (pre-release version):
 - Solder the top resistors first, then the LED's, then the other surface mount parts
 - The height of the controller and display are very important to fitting everything nicely into the chassis, make sure everything is flush and seated all the way.
 - Be sure to trim the legs of any through hole components after soldering, as above, the clearances are very important.


