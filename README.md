# ma-to-svg
Command line app to convert Maya 2017 ASCII (`.ma`) files to Scalable Vector Graphics (`.svg`) files.

* Supports NURBS Curves
  * The shape node's `Object Display`->`Drawing Overrides`->`RGB Color` will be exported as the SVG color
  * The shape node's parent name is used as the id of the `<path>`  

The coordinates are normalised on export meaning the lowest coord will be scaled to 0,0 and the max will be scaled to the resolution dimensions.  
As SVG's have their origin in the upper right corner of the viewport it is recommended that the model is created below the grid that way it won't be inverted.  
