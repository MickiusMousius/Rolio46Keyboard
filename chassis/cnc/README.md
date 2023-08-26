# Introduction

This is a chassis that can be manufactured using CNC.

It has been tested using JLCPCBs CNC Manufacturing service using:
 * 6061 Aliminium
 * Finish
   * Bead Blasting - 100 mesh
   * Matte Anodising - Dark Grey
 * Tolerance ISO 2768 medium

The STEP files are the original CAD files, these are made available so that modifications can easily be made. If the STEP files from the Electronics folder are imported too it will be possible to see the clearances for various parts.

# Examples

Backlight on and at a lowish setting.

![CNC 0.1 Example](../../images/cnc/main.png?raw=true "CNC 0.1 Example")

The USB port has a small printable surround that makes the charge and Bluetooth indicator LEDs visible.

![CNC 0.1 Example](../../images/cnc/indicators.jpeg?raw=true "CNC 0.1 Example")

![CNC 0.1 Example](../../images/cnc/rear.jpeg?raw=true "CNC 0.1 Example")

The CNC version of the chassis has a few more parts than the FDM version, assembly is illustrated below:

![CNC 0.1 Example](../../images/cnc/assembly.png?raw=true "CNC 0.1 Example")


# The Chassis

The STEP files in "CNC Parts" must be uploaded to provide the design itself.

When preparing the order use the following settings:
 * Material 6061 Aliminium
 * Finish
   * Bead Blasting - 100 mesh
   * Matte Anodising - Dark Grey
 * Tolerance ISO 2768 medium
 * Threads "Yes"
   * Upload the "Thread and Machine Spec.pdf" to provide thread details

You will need to request a manual quote from JLCPCB before youu can proceed to place your order.

# Other Parts

In addition to the CNC parts some components need to be printed using FDM (SLA may also work). The required STL files can be found in the "FDM PLA Parts" and "FDM TPU Parts" folders.

When printing the "FDM PLA parts" the "LCD Bracket", "Reset Button" and "USB Diffuser" should be printed on a smooth build plate with very fine layer lines (tested at 0.12mm).

You will need to print two "USB Diffuser" and "Reset Buttons", since they are very small it may be wise to print three in total (depending on the printer).

The "USB Diffuser" is optional, if it is printed it should ideally be printed in clear filament so that light from the LED indicators can shine through.

The "FDM TPU Parts" should be printed on a smooth build plate using 0.1mm layer lines (including the first layer).

You will also require 10x M2x4 screws & 8x 9mm non-slip silicone feet.
