# Gantry Mounted Nozzle Scrubber with poop eject

Here's a design for a nozzle scrubber that ejects poop as needed.

[Video Here](https://youtu.be/P8CdES0VPNM)

The scubber has a moving head riding on 6 small bearings that pushes any poop off the poop-deck during the scrubbing motion.

<img src="images/image1.jpg" alt="images/image1.jpg" width="200">
<img src="images/image3.jpg" alt="images/image3.jpg" width="200">

# PoopDeck

This is the location for any poop during a filament change. I recommend covering this with a thin layer of silocone.

<img src="images/image3.jpg" alt="images/image3.jpg" width="200">

For example this tape (many similar tapes available) is easy to attach, wrapping like a rubber band around the deck.

<img src="images/image2.jpg" alt="images/image2.jpg" width="200">

# Scrubber

The scrubber I've attached is a standard bambu-labs style silicone brush. Other brush styles can be used, but keep the depth similar.

<img src="images/image8.jpg" alt="images/image8.jpg" width="200">
<img src="images/image6.jpg" alt="images/image6.jpg" width="200">

# Auto-return

Magnets ensure the scrubber stays in place when not in use. 

<img src="images/image4.jpg" alt="images/image4.jpg" width="200">

# BOM

2x 4mmx5.7mm Magnets
7x 6mm m3 bolts (holding bearings, and brush stop)
8x 10mm m3 bolts (L bracket assembly)
2x 10mm m4 bolts
2x m4 2020-slidein nuts
6x MR63ZZ bearings
Self-Fusing silicone tape

# Build Notes.

The magnet and bearing holes all have small holes into their bases to allow easy removal if needed.

After sliding on the slider, use a 6mm m3 bolt in the base to stop the slider being removed.

<img src="images/image5.jpg" alt="images/image5.jpg" width="200">

A suggested cleannozzle macro is included in the macros/ folder. Modify the x/y positions at the start of the macro as needed.


> [gcode_macro CLEAN_NOZZLE_GANTRY]\
> description: Clean nozzle using sliding gantry brush\
> `#` Define the location where the poop will land, all other locations will be based off\
> `#` this position. It should be the center of the silicone coated poop tray, 5mm left of\
> `#` left edge of the rubber nozzle brush.\
> variable_x_poop: 18\
> variable_y_poop: 300 \
> variable_number_wipes: 3

 