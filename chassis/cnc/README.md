# Introduction

This section contains all of the files and information that is needed to manufacture a CNC Rolio46.1 chassis.

The STEP files are the original CAD files, these are made available so that modifications can easily be made. If the STEP files from the Electronics folder are imported too it will be possible to see the clearances for various parts.

TODO: Provide a set of models for an FDM bottom plate as this will allow for significant cost savings.

# Examples


Backlight on in full daylight.

![CNC 1.0 Example](../../images/cnc/backlight_on_above.png?raw=true "CNC 1.0 Example")

The USB port has a small printable surround that makes the charge and Bluetooth indicator LEDs visible.

![CNC 1.0 Example](../../images/cnc/from_rear.png?raw=true "CNC 1.0 Example")

# Main Chassis

The STEP files in "CNC Parts" must be uploaded to provide the design itself.

When preparing the order use the following settings:
 * Material 6061 Aluminum
 * Finish
   * Bead Blasting - 120 mesh
   * Glossy Anodizing - Natural
 * Tolerance ISO 2768 medium
 * Threads "Yes"
   * Upload the "Thread and Machine Spec.pdf" to provide thread details

You will need to request a manual quote from JLCPCB before you can proceed to place your order.

# Other Parts

In addition to the CNC parts some components need to be printed using FDM (SLA may also work). The required STL files can be found in the "FDM Parts" folder.

## FDM PLA Parts

When printing the FDM parts the "Reset Button" and "USB Diffuser" should be printed on a smooth build plate with very fine layer lines (tested at 0.12mm).

The "Power Switch" should be printed with a raft and very fine layer lines too. When printing a multicolor switch I found that a 0.2mm nozzle yielded best results, however, a 0.4mm nozzle does also work.

The "USB Diffuser" is optional, if it is printed it should ideally be printed in clear filament so that light from the LED indicators can shine through.

## FDM TPU Parts

The FDM TPU parts must be printed with 0.16 or 0.1mm layers. They are intended to absorb some vibrations, improve the sound profile, offer electrical insulation and protect the PCB from the hard aluminium chassis.

## General Hardware

| Quantity  | Description  | Ref  | Value  | Supplier  |
|:----------|:----------|:----------|:----------|:----------|
| 8  | 9mm Silicone Feet | -  | - | [Aliexpress](https://www.aliexpress.com/item/1005005504977168.html?spm=a2g0o.order_list.order_list_main.67.675e1802ITKJQ5 )  |
| 10 | M2x4mm Screws | -  | -  | [Aliexpress](https://www.aliexpress.com/item/32810872544.html?spm=a2g0o.productlist.main.1.764965e5UFrGqL&algo_pvid=c5686b2b-d8dd-403c-b107-a5b601dd8758&algo_exp_id=c5686b2b-d8dd-403c-b107-a5b601dd8758-0&pdp_npi=4%40dis%21AUD%212.42%211.67%21%21%211.52%21%21%402103209516943107919815919eb511%2112000026955302078%21sea%21AU%21192529469%21S&curPageLogUid=TCVQaWi3Sbah)  |
