OC
Opto Color

This is a very small program written in python that should print best suited
forground colors for a specific background color (16-231).

This uses the 256 colour terminal colour codes for this task.
So it takes a background color e.g. `./oc 200` and then prints suitable colors
from 16-255.

Currently the input background color has to be from 16-231.
Support for some other colors will be added.

It by default considers contrast ratio between 4.5 to 7 acceptable by default.
But one can change these in the script.
