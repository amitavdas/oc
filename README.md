[![License](https://img.shields.io/badge/License-BSD_3--Clause-blue.svg)](https://github.com/ragnarov/oc/blob/master/LICENSE)

'**o**ptimum **c**olour' or 'oc' is a utility to print list of suitable\
candidates for foreground colour of a terminal with given background colour in\
descending order based on contrast ratio (cr) as defined by **WCAG 2.0**.

Nothing is Guaranteed to work. See License.

**Only the colors in terminal's colour palette from** `16 to 255` **is considered.**

It uses the terminal's colour palette for this task.\
So it takes a background colour e.g. `./oc 200` or `./oc 1d1f21` and then\
prints suitable colours from `16 to 255`.

**Background color can be** `16 to 255` in terminal's colour palette.\
Additionally **RGB hex value as background colour can be used**.\
This is because many terminal emulators support setting custom background color.

The user still has to select which colour they want to use.\
Because colour preference varies a lot person to person.\
There can still be some colours that look good but are outside\
default `cr` range.\
So it my be of interest to adjust `cr` range according to personal preference.

Note: `--pl` option is not based on **WCAG 2.0**\
That was added out of curiosity only and is not recommended for use.

Note: Default `cr` range `4.5 to 7`.\
A lower limit of at least `4.5` is recommended by **WCAG 2.0**.\
Source: http://www.w3.org/TR/WCAG20/#contrast-ratiodef

```
usage: oc [-h] [--crl crl] [--crh crh] [--pl] bg

Prints suitable foreground colours for specific background colour.

positional arguments:
  bg          Accepts Background colour input, as (16 to 255) or Hex RGB e.g. 1d1f21

optional arguments:
  -h, --help  show this help message and exit
  --crl crl   lower limit of contrast ratio to be used, 4.5 recommended (default)
  --crh crh   upper limit of contrast ratio to be used, default 7, must be grater than crl
  --pl        Show colors according to Perceived lightness
```
