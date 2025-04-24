# Introduction

This folder contains the KiCad 7 PCB design files for the left and right shield boards of the Rolio 46.

# Ordering The PCBs from JLCPCB

Inside the "Left" and "Right" folders there are "Gerbers" zips. These are gerber files that have been prepared for use with JLCPCB.

The following settings were used when ordering:
* Base Material:	FR-4
* Layers:	2
* Delivery Format:	Single PCB
* PCB Thickness:	1.6
* Impedance Control:	No	
* PCB Color:	Black
* Silkscreen:	White
* Via Covering:	Tented
* Surface Finish:	HASL(with lead)
* Deburring/Edge rounding:	No
* Outer Copper Weight:	1 oz
* Gold Fingers:	No
* Flying Probe Test:	Fully Test
* Castellated Holes:	No
* Remove Order Number:	No
* 4-Wire Kelvin Test:	No
* Paper between PCBs:	No
* Appearance Quality:	IPC Class 2 Standard
* Silkscreen Technology:	Ink-jet/Screen Printing Silkscreen
* Board Outline Tolerance:	±0.2mm(Regular)

Ordering is possible with other suppliers, however you should regenerate the Gerber files according to the manufacturer's requirements.

<br/>

# Required Components

All of the components in the below table are required to build the shield assembly.

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 48    | 75V 0.15A Fast Switching Diode, SOD-123    | D1-D29    | 1N4148W    | [Aliexpress](https://www.aliexpress.com/item/4000685043735.html?spm=a2g0o.productlist.main.1.4fdc3d00DqAdPM&algo_pvid=b3d5a5ae-e50d-4501-af77-be2bdf4c63d0&algo_exp_id=b3d5a5ae-e50d-4501-af77-be2bdf4c63d0-0&pdp_npi=4%40dis%21AUD%211.58%211.18%21%21%211.00%21%21%402101ea7116971111863577912e12a5%2110000006015575494%21sea%21AU%21192529469%21&curPageLogUid=XZjBpJ8fx53X )    |
| 2  | Machine sockets and pins | -    | -   | [Typeractive](https://typeractive.xyz/products/machine-sockets-and-pins?_pos=1&_sid=3c03709e0&_ss=r)   |
| 2    | Surface mount push button switch, generic, two pins    | RESET1   | -   | [Aliexpress](https://www.aliexpress.com/item/1005004297433455.html?spm=a2g0o.order_list.order_list_main.136.675e1802ITKJQ5 ) (I used "Option 4")  |
| 2  | Surface mount DIP Switch, Single Pole Single Throw (SPST) switch, small symbol   | SW4  | -   | [Aliexpress](https://www.aliexpress.com/item/4000685483225.html?spm=a2g0o.order_list.order_list_main.177.675e1802ITKJQ5) |
| 2  | EVQWGD001 Rotary encoder, dual channel, incremental quadrate outputs, with switch  | RE_1  | EVQWGD001  | [Aliexpress](https://www.aliexpress.com/item/1005004320540116.html?spm=a2g0o.productlist.main.23.17631feeTpOfW8&algo_pvid=cfaa226d-1b56-4653-bf93-8ca20c1d1662&algo_exp_id=cfaa226d-1b56-4653-bf93-8ca20c1d1662-11&pdp_npi=4%40dis%21AUD%2117.39%2111.31%21%21%2111.01%21%21%402103011716971110881116110e900c%2112000028743285676%21sea%21AU%21192529469%21&curPageLogUid=qpQkvoiHmsxz ) |
| 4  | 0805 Surface mount capacitors  | C1, C2  | 100nF  | [Aliexpress](https://www.aliexpress.com/item/32888863725.html?spm=a2g0o.productlist.main.1.421ed7d7TDWEJj&algo_pvid=64889c03-7048-4b0c-b35b-564d9069f833&algo_exp_id=64889c03-7048-4b0c-b35b-564d9069f833-0&pdp_npi=4%40dis%21AUD%215.93%215.34%21%21%213.72%21%21%402101e9d116966657566622481e9c98%2110000000070124058%21sea%21AU%21192529469%21&curPageLogUid=FUlprN51Ouc7) |
| 46  | Kailh Choc hot swap sockets PG1350 | - | -  | [Aliexpress](https://www.aliexpress.com/item/1005003908487064.html?spm=a2g0o.productlist.main.3.49fd54f1tOHVAG&algo_pvid=229d47f1-057c-4c60-910a-70a8406ef798&algo_exp_id=229d47f1-057c-4c60-910a-70a8406ef798-1&pdp_npi=4%40dis%21AUD%212.18%211.49%21%21%211.38%21%21%402103242516971112370436660e1166%2112000027440505201%21sea%21AU%21192529469%21&curPageLogUid=gowJDuxybhSp) |

<br/>

# Optional Backlight Components

The parts in the below table are only needed for the backlight, if you do not want a backlight they can be omitted from your build to save some money.

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 2   | 30V Vds, 5.7A Id, N-Channel MOSFET, SOT-23  | Q1   | AO3400A   | [Aliexpress](https://www.aliexpress.com/item/33013971929.html?spm=a2g0o.productlist.main.3.4ccb430f1veGO2&algo_pvid=7ba1cd19-de8e-4e99-83f5-80068013a117&algo_exp_id=7ba1cd19-de8e-4e99-83f5-80068013a117-1&pdp_npi=4%40dis%21AUD%211.33%211.17%21%21%210.84%21%21%40210313e916971112882668959e17f6%2167112817842%21sea%21AU%21192529469%21&curPageLogUid=XIKDhCd7tq6N)  |
| 2 | 0805 Surface mount resistor  | R1  | 470Ω  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 2 | 0805 Surface mount resistor  | R2  | 10kΩ  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 46 | 0805 Surface mount resistor  | R3-R25 | 680Ω  | [Aliexpress](https://www.aliexpress.com/item/1005001794062302.html?spm=a2g0o.productlist.main.1.2bbc4d8fZh4OMh&algo_pvid=cd85416e-f214-4653-8231-9cafb078d750&algo_exp_id=cd85416e-f214-4653-8231-9cafb078d750-0&pdp_npi=4%40dis%21AUD%210.87%210.74%21%21%214.04%21%21%402101e9cf16943107335705048ea1b0%2112000017594821225%21sea%21AU%21192529469%21S&curPageLogUid=wKZhmIBeFMXc) |
| 46  | 0805 Surface mount LED  | LED1 - LED23  | - | [Aliexpress](https://www.aliexpress.com/item/1005004341345794.html?spm=a2g0o.order_list.order_list_main.25.675e1802ITKJQ5 )  |
