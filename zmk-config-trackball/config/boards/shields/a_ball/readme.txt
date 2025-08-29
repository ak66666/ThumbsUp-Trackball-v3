20250730 1442

The layer-based direction switch works now.
My mistake was to put &zip_xy_swap_mapper and some other transformations into the base/default layer 0.
It was not turning off, or didn't play well with a similar transformations in other layers.
Once I removed everything from layer 0  (the default left hand configuration), and put the XY swap 
into layer 1 (the right hand layout), and set all the defatul XY swap and X- and Y-inversions in the config file,
that functionality started working.

The scrolling works for the left-hand configuration only.
I suspect that's because of the way I switch between the layers - and it never goes to the level 3 (right hand scrolling.)
I will remove that separate right hand scrolling layer, and leave a single scrolling layer.
The XY swap will be done in layer 2 for both scrolling and pointing.

20250730 1911

Started laying out the keys.
I have 9 pins available for direct control - on the left side of PriMicro, 1..9.
That leaves 0 for the ball irq and two ground pins.

I seem to be unable to move to a layer after the next one - in the trackball listener code.
It is simply ignored, even the laye is selected - I confirmed it by placind specific letter on those layers.
 
20250731 1414

Made the scrolling work - the missing ingridient was "process-next" command in the input processor.
Without that command the first layer-filtered segment was running but not going to the next layers, if any.
That is the right-hand layer #1 was activated, its block swapped the navigation direction from the default left-handed.
When the scrolling layer #3 was activated - it was not reached without "process-next" in the block for layer 1.

I think I can remove the extra layer, just keep the common shared scrolling layer now.
Its sole purpose is to turn the scrolling on, no key modifications.



20250828 1339

Yesterday I received and assembled PCBs - after some tweaking it works.
There were two obstacles:
- the 3610 not starting up in time, had to increase the delay from 1s to 2s.
- the sensor lens was too close to the ball, adjusted its location.
The rest of the code was the same as in the mock-up.
