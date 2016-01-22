Example for Genero 3.0 EAP using new image centralization feature

This example shows all the fontawesome files in the current fontfile plus how
to create some coloured image

In FGLDIR/lib you will find a file image2font.txt that references the fontfile 
font file FontAwesome.ttf in the same directory.  These images are on the 
server and are hence available for ALL clients.  Previously we shipped images
inside the GDC, GWC, GeneroMobile 

To see how to do colour and/or add your own images, note the entries in my_image2font.txt ...

circle-red=FontAwesome.ttf:f111:red
circle-orange=FontAwesome.ttf:f111:orange
circle-green=FontAwesome.ttf:f111:#00FF00

... essentially the last entry on the line indicates what colour to use when
rendering the image.  Without colour specified the images will be the system
tint colour.

Also right-click on fontawesome application node and note how FGLIMAGEPATH has
been set to reference
- my_image2font.txt - to gain the custom entries
- FGLDIR/lib/image2font.txt - to reference the default images shipped in FGLDIR/lib
- FGLDIR/lib - to reference the default .ttf file in that directory