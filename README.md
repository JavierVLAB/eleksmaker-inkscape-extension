# eleksmaker-inkscape-extension

This is a fork of the "EleksMaker Tool" Inkscape extension, with updates
to make it work on Inkscape 0.92.4 without weird scaling effects.

There are actually two plugins as part of EleksMaker Tool - the cutter
("Gcode output") and the hatcher ("Filling Gcode"), the former looking
like it's derived from the regular Gcode tools, and the latter appearing
to be from egg-bot. I have yet to try the hatcher, so I can offer no
comments as to whether it has scaling issues (but I didn't see the magic
values to indicate that it has issues, for what it's worth).

December 2020
Reviewed Eleksmaker.py to get rid of calls to deprecated Inkscape libraries
(refer to https://wiki.inkscape.org/wiki/index.php/Updating_your_Extension_for_1.0
and https://inkscape.gitlab.io/inkscape/doxygen-extensions/deprecated_8py_source.html
and https://inkscape.gitlab.io/extensions/documentation/index.html)

Also updated some old Python 2 to Python 3

Seems to work on simple drawings in Inkscape as well as bitmaps traced to
path (refer to examples from Eleksmaker in https://wiki.eleksmaker.com/doku.php?id=inkscape)

Managed to send generated GCode from Inkscape 1.0 to EleksDraw machine using Candle
(all on MacOS)