# slock - simple screen locker

simple screen locker utility for X.

## dwrik's build

This is my build of slock (simple X screen locker) from [suckless](https://suckless.org/). This build includes the following patches:

- dpms - to automatically turn off display after given interval
- capscolor - changes indicator color if caps lock is activated
- xresources - to draw in colors from xresources (pywal compatible)
- dwmlogo - shows a custom shape (dwm logo by default) instead of a blank screen

## Requirements

In order to build slock you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (slock is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install slock
(if necessary as root):
```
make clean install
```

## Running slock

Simply invoke the 'slock' command. To get out of it, enter your password.

Slock can also be enabled as a systemd unit or be invoked with xss-lock during xinit.
