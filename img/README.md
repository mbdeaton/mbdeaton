# How to Edit Images for Project Portfolio
Brett's Notes - Summer 2022

This file is now under version control in mbdeaton.github.io.

These images are for my project website,
[mbdeaton.github.io](https://mbdeaton.github.io).

The goal is a simple, lightweight, black and white image with some color
highlights. Sometimes it's a png from a jpg, sometimes it's an svg.
Always it's got an aspect ratio of 3:1, width:height.


## JPG to PNG

### Gimp
Crop image to desired aspect ratio, convert to grayscale, and introduce
a splash of color.

* import `IMAGE.jpg`
* save project as an *xcf
* highlight any region with the crop tool
* in the tool options, select fixed aspect ratio, 3:1
* find nice selection from the photo, and click inside to crop
* reduce file size by scaling image to 600x200 Image > Scale
* convert to grayscale Colors > Desaturate > Color to Gray
* invert colors Colors > Invert
* introduce a new layer "Drawing"
* decrease opacity to 50%
* use paint brush 2 to introduce some orangy-red #ff2200, size 10, opacity 50%
* export to png and save as `IMAGE-final.png`, unchecking all export options to
  reduce file size


## JPG to SVG

### Gimp
Crop image to desired aspect ratio and increase contrast.

* import `IMAGE.jpg`
* save project as an *xcf
* highlight any region with the crop tool
* in the tool options, select fixed aspect ratio, 3:1
* find nice selection from the photo, and click inside to crop
* adjust brightness/contrast Colors > Brightness-Contrast
* export to jpg and save as `IMAGE-cropped.jpg`

### Inkscape
Here's a short tutorial on the Inkscape
[bitmap tracer](https://inkscape.org/doc/tutorials/tracing/tutorial-tracing.html).

* open template.svg in Inkscape, save as new project name
* import source `IMAGE-cropped.jpg`
* trace bitmap to generate a vector image Path > Trace Bitmap
* reduce the number of nodes in the path Path > Simplify
* delete bitmap
* make the paths white (for use on a dark background)
* introduce one or two little regions of bright color for highlight
* export as `IMAGE-final.svg`
