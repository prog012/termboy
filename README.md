Termboy
=======

Termboy is a Nintendo Game Boy emulator...for your terminal.  
Termboy is based on [Higan](http://byuu.org/higan/), but uses ncurses to render the screen.

Compiling
---------
Required Tools:

* g++ (>= 4.7)

Required Libraries:

* ncurses
* alsa

**Note:** The defintion for mvaddwstr is in "ncurses/curses.h" on Ubuntu, but it's just "curses.h" on Arch Linux.  For development purposes, Just create an ncurses folder in /usr/include and symlink ncurses/curses.h to curses.h.

TODO
----
* Keyboard input fix (multipress & key up/down events)
* Restore terminal settings after exit
* Accept parameters in run script; handle bad input
* GB Color support
* Remove configuration files
* Check for boot.rom
* Continue deleting unused code

WISHLIST
--------
* Rewrite in ANSI C
* Restyle code to K&R
* Remove GCC-specific code
* Create Arch PKGBUILD
* Port to other Unices
