# VOID40
*A 40% handwired ortholinear keyboard*

![VOID40](https://i.imgur.com/dhAZlNd.jpg)

The VOID40 is a 3d printed, handwired, 40% ortholinear keyboard running QMK Firmware on a Pro Micro controller. The case is designed to fit the bed of a stock Ender 3 when the parts are rotated 45 degrees and the skirt/brim is disabled in the slicers settings.

I suggest printing the case using a 0.4 mm nozzle, supports are not needed for any of the parts.

You might want/need to use small dabs of hot glue to secure the switches in the plate depending on how well calibrated your printer is(if you're generous with it, it will add to the weight of the keyboard and it might change the feel of it).

Dont overtighten the screws as the posts could break off and the threads might get stripped.


# Bill Of Materials

* 47/48 diodes (tme.eu [link](https://www.tme.eu/ro/en/details/1n4148-dio/tht-universal-diodes/diotec-semiconductor/1n4148/))
* 47/48 cherry mx style switches
* 24 AWG (0.2 mm2) wire
* Pro Micro
* EC11 Rotary Encoder (optional / I used a 15mm EC11 clone, mounted to the plate using [this adapter](https://www.thingiverse.com/thing:3770166))
* 4 M3x10 countersunk screws that go through the top case (tme.eu [link](https://www.tme.eu/ro/en/details/b3x10_bn661/bolts/bossard/1250752/))
* 4 M3x10(13mm overall length, 5.5mm diameter head) allen head screws that go through the bottom plate (tme.eu [link](https://www.tme.eu/ro/en/details/m3x10_d912-a2/bolts/kraftberg/))
* hot glue for securing the pro micro to the bottom case(optional, but recommended)

A fork containing the QMK config files can be found [here](https://github.com/victorlucachi/qmk_firmware/tree/master/keyboards/handwired/void40). Edit them to suit your own needs and build the firmware following the QMK docs.
