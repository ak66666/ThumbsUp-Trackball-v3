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


//TODO
![Ball Holder Prototype (without ball)](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/Ball%20Holder%20Prototype%2C%2020250417.jpg)
![Ball Holder Prototype (with a ball inserted)](https://github.com/ak66666/ThumbsUp-Trackball/blob/main/Photos/Ball%20Holder%20Prototype%20(without%20ball)%2C%2020250417.jpg)

Other pictures in Photos folder.

# Firmware

... //TODO


//TODO:
- Add the sensor board (schematics are ready)
- Expand the bottom PCB ball holes to let it poke through downwards, and may be make it off-center, only the bearing needs to be in a specific position. Otherwise the ball can hang out, as long as it does not touch the PCB or the table.
- Extend the middle PCB ball opening - to let the bearings touch/support the ball, but leave enough of a gap for the ball otherwis..
- Extend the top PCB ball opening to prevent the ball from falling out.
- Add the bearing holes
	- Add dummy resistors/shunts in the schematics for all of them
	- Top PCB (???? May be I should leave the top board just a hair off the ball? Without a bearing it may scratch the ball though. Should I add some kind of a pad? Just to prevent the scratching. Some sticky tape?)
	- Middle PCB
 	- Bottom PCB - 1 ball
- Add a (button?) switch for the BT control - to switch to the BT layer and use the mouse buttons to switch between 3 profiles and 1 button for the current profile reset. 