# Introduction

This folder contains a designs and manufacturing files for the Rolio keyboard chassis.

The folders within here are described below.

## Electronics

This contains STEP file models with the electronics and PCB. These can be used when creating new chassis or modifying the existing models. These files should be helpful for validating component clearances.

## FDM

Contains design files for a FDM 3D printed chassis.

This is the most accessible manufacturing option and the cheapest.

The largest drawback of this manufacturing technique is that layer lines may be visible. Additionally the chassis may not be as rigid as desired depending on the filament used.

The CNC design is based on this one as it is the cheapest for prototyping.

More information and preview images can be found in the [FDM Section](fdm/README.md).


## CNC

This is by far the most expensive of the two options (anecdotally 6 times the cost of MJF or 12 times that of SLA).

It will produce the most aesthetically pleasing, rigid and durable result when using aluminium.

It does have the drawback of being the heaviest. There is also likely some Bluetooth signal attenuation, however in my testing so far this has not proven to be an issue. I will however include RF windows in the V 1.0 release.

More information and preview images can be found in the [CNC Section](cnc/README.md).
