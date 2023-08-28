# Introduction

This is a chassis that can be manufactured using CNC.

It has been tested using JLCPCBs CNC Manufacturing service using:
 * 6061 Aliminium
 * Finish
   * Bead Blasting - 150 Grid
   * Matte Anodising - Natural
 * Tolerance ISO 2768 medium

The STEP files are the original CAD files, these are made available so that modifications can easily be made. If the STEP files from the Electronics folder are imported too it will be possible to see the clearances for various parts.

# The Chassis

The files found in the "CNC Parts" folder must be uploaded to JLCPCB (or another) manufacturer.

The STEP file must be uploaded to provide the design itself.

When preparing the order use the following settings:
 * Material 6061 Aliminium
 * Finish
   * Bead Blasting - 150 Grid
   * Matte Anodising - Natural
 * Tolerance ISO 2768 medium
 * Threads "Yes"
   * Upload the "Thread and Machine Spec" to provide thread details

# Other Parts

In addition to the MJF/SLA parts some components need to be printed using FDM (SLA may also work). The required STL files can be found in the "FDM Parts" folder.

When printing the FDM parts the "LCD Bracket", "Reset Button" and "USB Diffuser" should be printed on a smooth build plate with very fine layer lines (tested at 0.12mm).

You will need to print two "USB Diffuser" and "Reset Buttons", since they are very small it may be wise to print three in total (depending on the printer).

The "USB Diffuser" is optional, if it is printed it should ideally be printed in clear filament so that light from the LED indicators can shine through.

You will also require 5x M2x4 screws & 4x 9mm non-slip silicone feet.
