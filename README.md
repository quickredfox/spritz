Spritz v0.0.1
=============

Sprite sheet builder with retina support.


Installation
============

*N.B: Not in NPM repository, install from source.*

Install Cairo.

    brew install cairo
    
Make sure you have coffee-script on your system.

    npm install coffee-script -g

Go to the root of this project...

    cd ./spritz # or wherever you put it.
    
Make sure you have all dependencies installed.

    npm install

If you see something like 

    Package 'xcb-shm', required by 'cairo', not found

You can do this and run ```npm install``` again.

    export PKG_CONFIG_PATH=$PKG_CONFIG_PATH:/opt/X11/lib/pkgconfig

Or see: https://github.com/LearnBoost/node-canvas/wiki/Installation---OSX


Usage
=====

    ./spritz -s [images folder] -r [retina images folder] -o [output folder]
    
    -s, --source    Gets source images from this folder                                                  [required]
    -r, --retina    Gets source retina images from this folder                                           [required]
    -o, --output    Outputs files to this folder                                                         [required]
    -f, --filename  Filename to use for CSS and spritesheet (distinction made by file extension)         [default: "sprites"]
    -p, --prefix    CSS class to use as prefix for sprites.                                              [default: "sprite"]
    -m, --bymax     Sort by max(width,height) before packing (otherwise sorts by greatest height first)  [default: true]
     
