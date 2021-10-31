oc

Optimum Colour

This is a very small program written in python that should print best suited\
foreground colours for a terminal with specific background colour within 16 to\
231 terminal colour palettes.

This uses the 256 colour terminal colour codes for this task.\
So it takes a background colour e.g. `./oc 200` and then prints suitable colours\
from 16-255.

Currently the input background colour has to be within 16 to 231.\
Support for RGB background colours should be added.

It uses contrast ratio between 4.5 to 7 acceptable by default.\
But these can be changed in the script.
