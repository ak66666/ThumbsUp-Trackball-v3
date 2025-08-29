# ThumbsUp! Trackball

A PCB-based thumb-operated trackball, inspired by Elecom EX-G left hand trackball, Ploopy Nano trackball, and my own ThumbsUp! keyboards.

To be suitable for both left- and right-hand usage.
The top two the plates can be re-attached at 180 degree and the cross-board connectors will swap left and right buttons, and the firmware will change the trackball movement direction.
 
Off-the-shelf ProMicro-style MCUs are considered: 
- Atmega- or RP2040-driven with QMK-based firmware - wired.
- nice!nano v2 (and clones) with ZMK-based firmware - wireless.

34 mm ball, same as in Elecom EX-G.
For bearings - uxcell 2.5mm Ceramic Bearing Balls, ZrO2 Zirconium Oxide Ball, again, the same as used to improve my Elecom trackballs.
Bearings to be implanted into PCBs, no 3D-printed ball shroud/holder.

![Photos](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/01.%204%20hrs%20view.jpg)
![Photos](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/02.%2010%20hrs%20view.jpg)
![](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/03.%205%20hrs%20view,%20top%20PCB%20removed.jpg)
![](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/04.%20Exploded%20view.jpg)
![](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/05.%204%20hrs%20view%20in%20hand.jpg)
![](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/06.%2012%20hrs%20view,%20hand%20on%20top.jpg)
![](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/07.%20Bottom%20view%20in%20hand.jpg)
![](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/08.%208%20hrs%20view%20in%20finger-controlled%20position.jpg)

Other pictures in Photos folder.

# Firmware

In zmk-config-trackball folder


//TODO:
There are many deficiencies found in the first version - it works, but the ergonomics and usability may be improved.
Luckily the sensor board, the costliest part, turned out to be good, and the rest is in the "passive" PCBs.
They are big and look as the trackball itself, but much cheaper to update and fix.
Changes are substantial, so I abandon this project repository as is.
There will be a separate project/repository for the new version.
