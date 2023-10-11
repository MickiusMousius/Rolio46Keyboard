# Introduction

This is a chassis that can be manufactured using CNC.

It has been tested using JLCPCBs CNC Manufacturing service using:
 * 6061 Aluminum
 * Finish
   * Bead Blasting - 100 mesh
   * Matte Anodizing - natural (I think a non matte anodizing may yield better results)
 * Tolerance ISO 2768 medium

The STEP files are the original CAD files, these are made available so that modifications can easily be made. If the STEP files from the Electronics folder are imported too it will be possible to see the clearances for various parts.

# Examples


Backlight on and at a lowish setting, the backlight is a bit yellow as I'm using choc sunset switches.

![CNC 0.9 Example](../../images/cnc/cnc_2.jpg?raw=true "CNC 0.9 Example")
![CNC 0.9 Example](../../images/cnc/cnc_3.jpg?raw=true "CNC 0.9 Example")

The USB port has a small printable surround that makes the charge and Bluetooth indicator LEDs visible.

![CNC 0.9 Example](../../images/cnc/cnc_4.jpg?raw=true "CNC 0.9 Example")


In normal daylight conditions.

![CNC 0.9 Example](../../images/cnc/cnc_1.jpg?raw=true "CNC 0.9 Example")

# The Chassis

The STEP files in "CNC Parts" must be uploaded to provide the design itself.

When preparing the order use the following settings:
 * Material 6061 Aluminum
 * Finish
   * Bead Blasting - 100 mesh
   * Matte Anodizing - Natural
 * Tolerance ISO 2768 medium
 * Threads "Yes"
   * Upload the "Thread and Machine Spec.pdf" to provide thread details

You will need to request a manual quote from JLCPCB before you can proceed to place your order.

# Other Parts

In addition to the CNC parts some components need to be printed using FDM (SLA may also work). The required STL files can be found in the "FDM Parts" folder.

## FDM PLA Parts

When printing the FDM parts the "LCD Bracket", "Reset Button" and "USB Diffuser" should be printed on a smooth build plate with very fine layer lines (tested at 0.12mm).

The "LCD Bracket", "Reset Button" and "USB Diffuser" should be printed on a smooth build plate with very fine layer lines (tested at 0.12mm).

The "Power Switch" should be printed with a raft and very fine layer lines too. When printing a multicolor switch I found that a 0.2mm nozzle yielded best results, however, a 0.4mm nozzle does also work.

The "USB Diffuser" is optional, if it is printed it should ideally be printed in clear filament so that light from the LED indicators can shine through.

## FDM TPU Parts

The FDM TPU parts must be printed to the actual design thickness (0.3mm), a fraction more is acceptable. They are intended to absorb some vibrations, offer electrical insulation and protect the PCB from the hard aluminium chassis.

## Other Parts

You will also require 10x M2x4 screws & 8x 9mm non-slip silicone feet.
