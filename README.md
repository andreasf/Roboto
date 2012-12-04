Roboto for Fontconfig
=====================

This version of Google's Roboto font has fontconfig-compatible metadata. This
means that font pickers in Linux will not just show all 16 style variants, but
when choosing one, fontconfig will give you the expected font!


Why is this even necessary?
---------------------------

The files contain several conflicting versions of the same metadata 
(Postscript, Windows, OpenType), and fontconfig handles those conflicts
in a different way than Windows or Mac OS. This is bad for Linux users, while 
font designers don't seem to care much.

More about the problem: https://bugzilla.redhat.com/show_bug.cgi?id=706559#c11


What did you change?
--------------------

I opened all files in FontForge and changed 

* Postscript weight
* TTF styles
* OS/2 weight class (only for Black and Thin variants)


License
-------

Copyright (c) 2011-2012, The Android Open Source Project

Licensed under the Apache License, Version 2.0. See file COPYING for details.
