# dmenu - dynamic menu | My custom build

[dmenu](https://tools.suckless.org/dmenu/) is an efficient dynamic menu for X.\
In this build I added the following patches:
- highlight
- numbers


## Features
---
Specify different highlight colors on launch.
- `-hf` - Highlight color (normal and selected)
- `-nh` - Normal highlight color
- `-sh` - Selected highlight color


## Requirements

In order to build dmenu you need the Xlib header files.


## Installation

Edit config.mk to match your local setup (dmenu is installed into
the /usr/local namespace by default).

Afterwards enter the following command to build and install dmenu
(if necessary as root):

    make clean install


## Running dmenu

See the man page for details.
