# What is FLTKRUS?
FLTKRUS project - FLTK with internal russian language support

# What should you do with this files?
Firstly, you need to download original FLTK project source code (Link on GITHUB: https://github.com/fltk/fltk)

Then, you need to remove from FL path original Fl_Widget.h, Fl_Window.h, Fl_Window.cxx and insert files, which you've got from this repository

Finally, you need to compile project (you can use .sln file for MSVS, which located on ide\VisualC2010). Compiled libs will be on lib path, which located on fltk project path

# TODO
In thoughts will decide, should hide deprecated .label(const char*) methods, or simply remove them (change for new files).
