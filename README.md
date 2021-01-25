# dmenu - dynamic menu | My custom build

[dmenu](https://tools.suckless.org/dmenu/) is an efficient dynamic menu for X.\
In this build I added the following patches:
- Border
- Center
- Grid
- Highlight
- Numbers
- Password
- Xresources


## Features
---
Specify different highlight colors on launch. Or launch in password mode
- `-hf` - Highlight color (normal and selected)
- `-nh` - Normal highlight color
- `-sh` - Selected highlight color
- `-P`  - Dmenu will not directly display the keyboard input, but replace it with given char in config.h

Specify how dmenu with items will be displayed on monitor
- Border will only show when centered
- `-c`  - Dmenu appears centered
- `-g [number]` - Dmenu list items with given number of columns
- `-l [number]` - Dmenu list items with given number of lines

Set colors with Xresources.
The availible options are:
- `dmenu.font`
- `dmenu.normbackground`
- `dmenu.normselforeground` *
- `dmenu.normforeground`
- `dmenu.selbackground`
- `dmenu.selforeground`
- `dmenu.normhighlightforeground`
- `dmenu.selhighlightforeground`
- `dmenu.highlightforeground` *

\* *The option `normselforeground` set de default foreground which override `normforeground` and `selforeground`. This is also true for `highlightforeground` which override `selnormhighlightforeground` and `selhighlightforeground`.*

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
