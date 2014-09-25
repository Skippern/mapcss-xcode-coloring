MapCSS Syntax Coloring
===================

Attempt at MapCSS syntax support for Xcode 6:
* reverse engineering *.xclangspec files in the Xcode.app resource tree

Based on the work of:
* Tiago Bastos (lua-xcode-coloring)
* Alex Karahalios (r-xcode-coloring & Install Script)

For now the coloring loads, but it doesnt autodetect the files, so you have to select the coloring from "*Editor > Syntac Coloring > MapCSS*" menu

Works with:
===================

* Xcode 4
* Xcode 5

MapCSS
===================

MapCSS is a CSS like stylesheet for map data visualization.

MapCSS is still in develoment, the latest specification can be found [here](http://wiki.openstreetmap.org/wiki/MapCSS/0.2)

Because of the higher complexity of MapCSS than its brother (inspired by) language, CSS, I have had to study how Xcode.app defines other languages, such as C, Java, Objective-C, etc. in order to understand the proprietary *.xclangspec definitions, which publically are undocumented by Apple Inc.

Other Documentation
===================

* [JOSM Implementation](http://josm.openstreetmap.de/wiki/Help/Styles/MapCSSImplementation)
* [pgmapcss implementation](https://github.com/plepe/pgmapcss/blob/master/doc/MapCSS.creole)


Xcode 6
===================

This doesn't seem to work properly in **Xcode 6**, somehow Xcode 6 doesn't accept the precense of the file in the directory apointed by the script, which result in the hilighting not being loaded. There must be some other file that need to be edited (adding a line in a menu list or something). This will need to be investigated further.
