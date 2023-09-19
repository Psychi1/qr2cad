Convert a qr code to a .scad, .dxf, or .stl file

Dependencies
============
* Python >= 3.9
* Python libraries (specified in requirements.txt)
  - Pillow (or Python Imaging Library)
  - qrcode
* [OpenSCAD](http://www.openscad.org)

Usage
=====

```
usage: qr2cad.py [-h] [-x] [-m] [-d MAXDIM] [-z ZHEIGHT] CONTENT

Convert qr codes to CAD objects

positional arguments:
  CONTENT     The content you want to create a qr code for.

optional arguments:
  -h, --help  show this help message and exit
  -x          Defaults to .stl by default, this option changes output to .dxf
  -m          Outputs qr2cad.scad by default, this options makes the result
              into a .dxf or .stl
  -d MAXDIM   The maximum size in mm to make the x or y dimension.
  -z ZHEIGHT  The max z-height of the text, defaults to 5. Not relevant for
              .dxf files
```