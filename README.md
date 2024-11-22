# Pigges's build of DWM
dwm is an extremely fast, small and dynamic window manager for X.

## Patches
* [Vanitygaps](https://dwm.suckless.org/patches/vanitygaps/)
* [Swallow](https://dwm.suckless.org/patches/swallow/)

Some patches are rewritten or modified to work together.

## Requirements
In order to build dwm you need the Xlib header files.

## Installation
```sh
sudo make clean install
```

## Running dwm
Add the following line to your .xinitrc to start dwm using startx:
```sh
exec dwm
```

In order to display status info in the bar, you can do something like this in your .xinitrc:
```sh
while xsetroot -name "`date` `uptime | sed 's/.*,//'`"
do
	sleep 1
done &
exec dwm
```

## Configuration
The configuration of dwm is done by creating a custom config.h and (re)compiling the source code.
