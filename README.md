# DCJ11_carrier

To protect the sensitive pins on the DCJ11 CPU, I designed a small carrier board to keep it safe.

I added a few extras to the board, like reverse polarity protection—just a simple reverse diode that shorts the power if applied incorrectly. (I know it really should have been a proper P-MOS instead, but hey, it’s better than nothing.) I also included pull-ups and pull-downs on the inputs since many of them won’t be in use for simple applications. This keeps them stable at the carrier level, so there’s no need to add jumpers externally.

There are also two extra capacitor footprints on the top side of the carrier if needed, though the DCJ11 itself seems to have plenty of local capacitance. Just for fun, I added footprints for a few LEDs and resistors, hoping that the ceramic package of the DCJ11 would let some light through and create a cool glowing effect—but no joy. The ceramic is completely opaque.

The PCB is designed to use turned IC socket contacts. The row with smaller holes is for the DCJ11 itself, lifting it up a few millimeters above the PCB. The larger holes allow the contacts to drop down fully to their flanges, making them protrude as much as possible below the board so the carrier can later be inserted into the user motherboard.
