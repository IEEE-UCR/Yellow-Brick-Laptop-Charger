Yellow-Brick-Laptop-Charger
===========================

Because why not charge your laptop from a giant, scary yellow brick lipo?

Design Specifics
----------------
The most important things (the soft start and such are all set to the Ti
reference values) are the UVLO and output voltage divider.


The UVLO circuit is set to around 36V (3.0V per cell in a 12S configuration).
It is noted that paranoid users can use a 10S lipo (which would cut off at
around 3.6V per cell).

The output voltage divider is set at 19V.  This is enough to power most devices.  It is crucial that a 5V buck converter be added for USB devices (or else they
might blow up.)

BOM
---
The Bill of Materials is actually pretty hard to generate from the nightly
version of kicad that Brandon is running.
So, the XML file actually has all of the materials in it.
Most of the components are 0805 sized, except for the 1μF capacitors which are
(and don't quote me on this) 1206 sized.
There are some specific packages that are not included in the KiCAD libraries,
but all of those should be included within this package.
Note that this.pretty contains component footprints associated to this build.
Note that the schematic symbols associated with this build aren't very neatly
organized in a separate folder.
