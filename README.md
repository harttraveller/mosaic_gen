# mosaic_gen
A notebook that can generate a mosaic from a large number of images, useful when used in conjunction with the instagram-scraper package.
https://github.com/rarcega/instagram-scraper

# Dependencies
Python v3

Pandas

Numpy

Pillow (PIL)

os, sys (included with python by default)


# How it works
The notebook uses a collection of images to generate a mosaic of a target photo. It does this by converting the target image to greyscale, cropping it, and splitting it into the square root of the number of images that the user wants to use to construct the mosaic (each image effectively representing a pixel). For instance, if you have 1600 images, then your final mosaic resolution (with each image as a pixel) will be 40x40, while the literal resolution will be 1000x1000.

# How to use it
After cloning the repository, you must place the the images you want the repository to be constructed from in the "photos" folder. Then you must place your target image in the "target" folder. Then simply run the program "mosaic_gen.py" from your command line while in the directory of the program folder. After a few seconds (could be closer to a minute depending on the speed of your computer), an image should appear in the program folder called "final". This is the generated mosaic.

# Example
Target photo (subject is Hugh Jackman):
![alt text](https://raw.githubusercontent.com/harttraveller/mosaic_gen/master/target.jpg)

Generated mosaic (with photos from Hugh Jackman's instagram):
![alt text](https://raw.githubusercontent.com/harttraveller/mosaic_gen/master/final.png)


