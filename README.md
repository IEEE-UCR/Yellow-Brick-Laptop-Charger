Yellow-Brick-Laptop-Charger
===========================

Because why not charge your laptop from a giant, scary yellow brick lipo?

Made with KiCAD nightly.

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

Here is a Digi-key link for enough parts to prototype three of these boards.
http://www.digikey.com/short/749jqc  These include the test points.  Feel
free to modify things as fit.  Do note that these BOMs do not contain the
LEDs for indicating that the board is powered.  (Or at least I don't think
they do...)

PCB
---
There is a dirty PCBs order that I placed a while ago.
Here is the "share" link.
http://dirtypcbs.com/view.php?share=4775&accesskey=4ce9e3b627f7e16a034119993f725ab9

You should be able to order the protopack pretty easily through this link.
Beware that these may not be the most current PCBs.

Important Notes
---------------
There are some specific packages that are not included in the KiCAD libraries,
but all of those should be included within this package.

Note that this.pretty contains component footprints associated to this build.
Note that the schematic symbols associated with this build aren't very neatly
organized in a separate folder.
