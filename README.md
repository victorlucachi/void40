# VOID40
*A 40% handwired ortholinear keyboard*

The VOID40 is a 3d printed, handwired, 40% ortholinear keyboard running QMK Firmware on a Pro Micro controller. The case is designed to fit the bed of a stock Ender 3 when the parts are rotated 45 degrees and the skirt/brim is disabled in the slicers settings.


I suggest printing the case using a 0.4 mm nozzle, supports are not needed for any of the parts.

You might want/need to use small dabs of hot glue to secure the switches in the plate depending on how well calibrated your printer is(if you're generous with it, it will add to the weight of the keyboard and it might change the feel of it).

Dont overtighten the screws as the posts could break off and the threads might get stripped.


*BOM*

* 47/48 diodes (1N4148)
* 47/48 switches
* 24 AWG (0.2 mm2) wire
* Pro Micro
* EC11 Rotary Encoder (optional, I used a 15mm EC11 clone)
* 4 M3x10 countersunk screws for the top plate
* 4 M3x10(13mm overall length, 5.5mm diameter head) allen head screws for the bottom plate
* hot glue for securing the pro micro to the bottom case(optional, but recommended)

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/master/keyboards/handwired/void40). Edit them to suit your own needs and build the firmware following the QMK docs.

![VOID40](https://i.imgur.com/dhAZlNd.jpg)
