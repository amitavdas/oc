[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)

oc\
Optimum Colour

This is a very small program written in python that should print best suited\
foreground colours for a terminal with specific background colour.

It uses the terminal's colour palette for this task.\
So it takes a background colour e.g. `./oc 200` or `./oc 1d1f21` and then\
prints suitable colours from 16 to 255.

It has been configured to use contrast ratio within 4.5 to 7 by\
default.
At least 4.5 is recommended.
Source: http://www.w3.org/TR/WCAG20/#contrast-ratiodef

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
