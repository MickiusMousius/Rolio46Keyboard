# Introduction

The controller provides the "brains" for the Rolio 46 keyboard. All of the tested controllers provide the bluetooth connectivity as well as battery charging and USB functionality. 

# Controllers

There are three different controllers that have been tested with this project.


| Nice!Nano  | SuperMini 52840 | SuperMini NRF52840 |
| ------------- | ------------- | ------------- |
| ![Nice!Nano](../images/controllers/nice_nano.jpg)  | ![SuperMini NRF52840](../images/controllers/supermini_52840.jpg)  | ![52840Nano](../images/controllers/52840Nano.jpg)  |

Details for each controller are summarized below.

### Nice!Nano  V2

This is the most common of the available controllers and arguably the best. Documentation for this controller can be found on [nice keyboards](https://nicekeyboards.com/nice-nano/).


The most standout features are summarized below:
 * Deep sleep consumption of only 20uA
    * This could provide a theoretical standby time (if not used) of more than 12 months for a Rolio 46
 * High manufacturing standards
 * Well established & widely used so its behavior is very well understood

This is by far the best all round controller. It has an excellent power consumption profile, has good support for all required features and is readily available from many distributors.

### SuperMini NRF52840

This is essentially a Nice!Nano clone, testing shows that it is almost 100% compatible with the Nice!Nano. Further documentation on this controller can be found on [ICBuy](http://wiki.icbbuy.com/doku.php?id=developmentboard:nrf52840).

Testing has shown that the deep sleep power consumption when turning off the external peripherals is as high as 700uA, this would provide very poor deep sleep durations. However this can be worked around by disabling peripheral power control this will decrease deep sleep power consumption to 128uA.

Key details are summarized below:
 * Deep sleep consumption of 128 uA
    * This could provide a theoretical standby time (if not used) of roughly 80 days for a Rolio 46
 * Poor support for peripheral power control
 * Much cheaper than the Nice!Nano

 This controller is a good choice for those that type for several hours a day that are more price conscious. The Rolio 46 can provide a little over a month of use between charges with this controller (depending on backlight usage etc). For a high usage scenario this controller's power profile is roughly comparable to the Nice!Nano.

### 52840Nano

Another Nice!Nano Clone, as with the SuperMini 58240 testing shows that it is almost fully compatible with the Nice!Nano.

There is one key issue with the controller, it can not power the Rolio 46's back light circuit. There are no work arounds for this except to disable the backlight in firmware.

Key details are summarized below:
 * Not compatible with the Rolio 46.1 backlight circuit, requiring the backlight to be disabled in firmware.
 * Standby power consumption of just 2.5uA
 * Requires a modification to the ZMK firmware to get accurate battery readings
 * Much cheaper than the Nice!Nano

If you have no need for a backlight then this is possibly the most energy efficient controller of the three options.
