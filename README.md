# VOID40
*A 40% handwired ortholinear keyboard*

![VOID40](https://i.imgur.com/WZ8EVJY.jpg)

The VOID40 is a 3d printed, handwired, 40% ortholinear keyboard running QMK Firmware on a Pro Micro controller. The case is designed to fit the bed of a stock Ender 3 when the parts are rotated 45 degrees and the skirt/brim is disabled in the slicers settings.

I suggest printing the case using a 0.4 mm nozzle, supports are not needed for any of the parts.

You might want/need to use small dabs of hot glue to secure the switches in the plate depending on how well calibrated your printer is (if you're generous with it, it will add to the weight of the keyboard and it might change the feel of it).

Dont overtighten the screws as the posts could break off and the threads might get stripped.

# Handwiring guide

I've also put together a pretty visual handwiring guide for the VOID9, that you can browse over [here](https://victorlucachi.ro/journal/void9-wiring-guide/).

| ![](https://i.imgur.com/01WknB5.jpg) 	| ![](https://i.imgur.com/GMMczAH.jpg) 	| ![](https://i.imgur.com/5NyUoJY.jpg) 	|
|---------------------------------------|---------------------------------------|---------------------------------------|

# Bill Of Materials

* 48 x diodes ([tme.eu](https://www.tme.eu/ro/en/details/1n4148-dio/tht-universal-diodes/diotec-semiconductor/1n4148/)/[aliexpress](https://www.aliexpress.com/item/32729204179.html))
* 48 x Cherry MX style mechanical switches
* 48 x keycaps of choice
* 1 x Pro Micro ([aliexpress](https://www.aliexpress.com/item/32902569443.html))
* 1 x EC11 Rotary Encoder ([aliexpress](https://www.aliexpress.com/item/32872039030.html)/mounted to the plate using [this adapter](https://www.thingiverse.com/thing:3770166))
* 24 AWG (0.2 mm2) wire
* 4 x 8mm bumpons

### Redux
* 10 x M2x3x3.5 OD heat inserts ([aliexpress](https://www.aliexpress.com/item/4000585933306.html?spm=a2g0o.order_list.order_list_main.33.21ef1802vdSNrS))
* 4 x M2x10 Allen head screws ([aliexpress](https://www.aliexpress.com/item/32966941844.html?spm=a2g0o.order_detail.order_detail_item.9.722ff19cyjrixq))
* 6 x M2x6 Countersunk screws ([aliexpress](https://www.aliexpress.com/item/32968097507.html?spm=a2g0o.order_list.order_list_main.32.21ef1802vdSNrS))

### V1
* 4 x M3x10 countersunk screws that go through the top case ([tme.eu](https://www.tme.eu/ro/en/details/b3x10_bn661/bolts/bossard/1250752/)/[aliexpress](https://www.aliexpress.com/item/32968097507.html))
* 4 x M3x10 allen head screws ([tme.eu](https://www.tme.eu/ro/en/details/m3x10_d912-a2/bolts/kraftberg/)/[aliexpress](https://www.aliexpress.com/item/32966941844.html))
* hotglue

# Pin assignment

    ROW0    ROW1    ROW2    ROW3
    D3      D2      D1      D0
    
    
    COL0    COL1    COL2    COL3    COL4    COL5    COL6    COL7    COL8    COL9    COL10   COL11
    D4      C6      D7      E6      B4      B5      F4      F5      F6      F7      B1      B3


    Encoder Pad A           Encoder Pad B
    B6                      B2

# QMK Vial Fork

A QMK Vial fork can be found [here](https://github.com/victorlucachi/vial-qmk/tree/dev_void/keyboards/handwired/void40).

Most features are disabled in order for the firmware to fit on the atmega32u4 present on the Pro Micro controllers, but if you want to tinker around with different features or if you're using a different MCU you can enable/disable them to suit your own needs by editing the rules.mk file in the vial keymap folder.

The web version of Vial is available at [vial.rocks](https://vial.rocks/); it runs in supported browsers (Chrome, Edge and Opera) without requiring an installation.

![VOID40 Vial](https://user-images.githubusercontent.com/2669084/198690935-4e657756-582a-4827-8257-93ca3e1ee1a2.png)

# QMK Fork

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/dev_void/keyboards/handwired/void40). Edit them to suit your own needs and build the firmware following the QMK docs.

If you plan on using the VIA configurator dont forget to download the json definitions file linked in this repository.

[![License: CC BY-NC-SA 4.0](https://img.shields.io/badge/License-CC%20BY--NC--SA%204.0-blue)](https://creativecommons.org/licenses/by-nc-sa/4.0/)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).
