# ma-to-svg
Command line app to convert Maya 2017 ASCII (`.ma`) files to Scalable Vector Graphics (`.svg`) files.

* Supports NURBS Curves
  * The shape node's `Object Display`->`Drawing Overrides`->`RGB Color` will be exported as the SVG stroke color
  * The shape node's parent name is used as the id of the `<path>`  

As SVG's have their origin in the upper right corner of the viewport it is recommended that you set maya to `Z` up and then create curves in the positive `X`&`Y` space.
