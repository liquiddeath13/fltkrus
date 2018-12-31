# What is FLTKRUS?
FLTKRUS project - FLTK with internal russian language support

# What should you do with this files?
Firstly, you need to download original FLTK project source code (Link on GITHUB: https://github.com/fltk/fltk)

Then, you need to remove from FL path original Fl_Widget.h, Fl_Window.h, Fl_Window.cxx, Fl_Text_Buffer.cxx and insert files, which you've got from this repository

Finally, you need to compile project (you can use .sln file for MSVS, which located on ide\VisualC2010). Compiled libs will be on lib path, which located on fltk project path

# How to use?
You should set label or title (for window), with method .label(const std::string&)
Example:

Fl_Button (pointer)btn = new Fl_Button(x, y, w, h, "");

btn->label(std::string("надпись на кнопке на русском языке"));

Fl_Window (pointer)win = new Fl_Window(x, y, w, h, "");

win->label(std::string("заголовок окна на русском языке"));

# TODO
In thoughts will decide, should hide deprecated .label(const char*) methods, or simply remove them (change for new files).

# ON FUTURE
Need to do something with methods in classes, that have functional for text output
