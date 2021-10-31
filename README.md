oc

Optimum Colour

This is a very small program written in python that should print best suited\
foreground colours for a terminal with specific background colour.

This uses the 256 colour terminal colour codes for this task.\
So it takes a background colour e.g. `./oc 200` and then prints suitable colours\
from 16-255.

Currently the input background colour has to be within 16 to 231.\
Support for RGB background colours should be added.

It has been configured to use contrast ratio within 4.5 to 7 as acceptable by\
default.

```
usage: oc [-h] [--crl crl] [--crh crh] bg

Prints suitable foreground colours for specific background colour.

positional arguments:
  bg          Accepts Background colour input, as (16 to 255) or Hex RGB e.g. 1d1f21

optional arguments:
  -h, --help  show this help message and exit
  --crl crl   lower limit of contrast ratio to be used, 4.5 recommended (default)
  --crh crh   upper limit of contrast ratio to be used, default 7, must be grater than crl
```
