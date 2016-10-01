LAMPS - The Open Hardware SLA Printer
-------------------------------------
LAMPS (Laser Arduino Mega Pololu Shield|SLA Printer) is an open control board and SLA printer design.  The SLA Printer strives to be a low-cost, small footprint (It is only 200mmx350mm!), highly capable SLA Printer. The build platform size is currently 100mmx100mm, but could probably be increased by someone who is motivated to enhance the design.

#License
The schematic for the OpenSL electronics are licensed under the GPL.

The printer and its associated parts are licensed under the Creative Commons Attribution-NonCommercial-ShareAlike 3.0 Unported License.

Basically, use my design all you want! :) But, don't sell it.  If you want an exception, contact me.

#LAMPS Board
LAMPS is the PCB control board that rides on top of an Arduino Mega 2560.  It provides Galvanometer control (Through 12 bit DACs).  It also controls the laser, buttons, Z Stepper Motor (Through Pololu Carrier), End Stops, LEDs, etc...  (It is the Brainz).

Version 1.0 of the LAMPS board has been manufactured and tested... I found a few issues with the board and am currently redesigning and removing a few unnecessary components for 1.1. Release date T.B.D.

#Firmware
The firmware for LAMPS is a fork of Marlin (The best open source RepRap firmware I know of), and can be found here: https://github.com/beardface/Marlin-OpenSL
The firmware is very much an active work-in-progress, and I encourage you to fork, and contribute.

#LAMPS Printer Parts -WARNING... THIS IS NOT UP TO DATE-
All of the parts are available as sketchup (skp) and stl files.

##Printed Parts
* 1x [Laser Mount](https://github.com/beardface/LAMPS/blob/master/parts/lasermount.stl)
* 1x [Mirror Mount](https://github.com/beardface/LAMPS/blob/master/parts/mirrormount.stl)
* 4x [Vibrating Vat Mount](https://github.com/beardface/LAMPS/blob/master/parts/vibrating_vat_mount.stl)
* 1x [Z-Axis Top Mount](https://github.com/beardface/LAMPS/blob/master/parts/z_top_mount.stl)
* 1x [Z-Axis Bottom Mount](https://github.com/beardface/LAMPS/blob/master/parts/z_bottom_mount.stl)
* 1x [Build Platform Mount](https://github.com/beardface/LAMPS/blob/master/parts/platform_mount.stl)
* 1x [Build Stage](https://github.com/beardface/LAMPS/blob/master/parts/build_platform_connector.stl)
* 1x Endstop Mount

##Laser Cut Parts
###Platform
Use 3/16"-1/4" thick acrylic for the platforms.
* 1x [Vat Platform](https://github.com/beardface/LAMPS/blob/master/parts/top_platform.svg)
* 1x [Component Platform](https://github.com/beardface/LAMPS/blob/master/parts/bottom_platform.svg)
* 1x 80mmx80mm 1/4"Acryilc Stage Mount (leftover part from cutting of top_platform)

###VAT
Use 1/4" Clear (Transparent) Acrylic for the VAT!
* 1x [Vat Back](https://github.com/beardface/LAMPS/blob/master/parts/vat_design/vat_back.svg)
* 1x [Vat Front](https://github.com/beardface/LAMPS/blob/master/parts/vat_design/vat_front.svg)
* 1x [Vat Bottom](https://github.com/beardface/LAMPS/blob/master/parts/vat_design/vat_bottom.svg)
* 1x [Vat Handle](https://github.com/beardface/LAMPS/blob/master/parts/vat_design/vat_handle.svg)
* 2x [Vat Sides](https://github.com/beardface/LAMPS/blob/master/parts/vat_design/vat_side.svg)

##Non-Printed Parts
* 1x NEMA 17 Stepper Motor (Low Profile!)
* 2x 8mm Smooth Rod (~260mm)
* 1x 8mm Threaded Rod (~260mm) and 2-M8 nuts
* 4x LM8UU Bearings
* 1x LAMPS Electronics Kit (w/Pololu and 2x endstops)
* 1x LAMPS PCB Build Platform
* 1x LAMPS Musimi 2020 Rail Kit and connectors
  * 4x  350mm 2020 Extrusions w/end tapping holes
  * 11x 160mm 2020 Extrusions
  * 1x  110mm 2020 Extrusion
* 1x LAMPS Enclsoure & Hatch Kit
* 1x 405nm Laser (20mw-150mw) -- Build properties/cure time/etc... vary by laser!
* 1x 3" Square Mirror
* 1x Laser Galvo Set (20kpps) w/power supply
 * Resistance Configuration (Note to Self)
  * AXIS  |  SIZE     | GAIN      | LF         | HF        | LINEAR
  * X     |  4.96Kohm | 4.68 Kohm | 26.36 Kohm | 4.78 Kohm | 1.75 Kohm
  * Y     |  6.1Kohm  | 4.18 Kohm | 26.47 Kohm | 4.37 Kohm | 2.3 Kohm
* 1x +/-12V Power Supply (~1-3Amps)
* USB Cable
* Power Cable
* Screws, Nuts, Wires, Solder, Patience

##Optional (But Useful) Non-Printed Parts
* 1xLCD Screen
* 1xSD Card Reader (and corresponding circuit... T.B.D.)
* 1x Power Switch (110-250VAC), lighted
* 1x Power Terminal (Two combine power into single input)
* 1x 3-Prong Power Jack
 
###LAMPS IS A WORK IN PROGRESS.

##Some words of Caution
* Careful with 110-250VAC, it can --bite-- Seriously Harm you if you aren't careful
* Some 405nm Resins can be toxic while curing- take the appropriate measures to ensure you are working in a well ventelated room

~LAMPS design, details, and parts list are provided without any warranty or gaurantee- this is a community project, so lets work together to solve issues that may arise!
