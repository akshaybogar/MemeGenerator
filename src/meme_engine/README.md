# meme_engine module

This module contains MemeEngine class which takes the location for storing the meme generated.


## Roles and Responsibilities

The meme_engine module takes the location where generated meme needs to be stored.


The make_meme method defined in MemeEngine class takes image, text and author and generates the meme accordingly.
The MemeHelper.py file contains all the helper functions required to generate meme.


## Dependencies

Libraries Pillow, os and random are required for using this module.


## How to use

meme = MemeEngine('./tmp')
path = meme.make_meme(img, quote_body, quote_author)


Here, meme object is created by providing the location. Then image, quote and author are passed to generate meme.
The module returns the path of the meme stored on disk.

