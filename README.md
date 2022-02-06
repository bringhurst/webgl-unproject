WebGL Unproject
===============

This is a port of the usual gluUnProject function to javascript for use in WebGL applications. To use, read the included JSDoc for the unProject function -- it closely matches the API for the common C variant of the same function.

This code was originally written for picking support in Lanyard (http://github.com/fintler/lanyard). See lanyard.BasicOrbitView for a working example.

Simple Example
--------------
```js
const viewportArray = [
    viewportOriginX, viewportOriginY, viewportWidth, viewportHeight
];

// The results of the operation will be stored in this array.
const modelPointArrayResults = [];

const success = GLU.unProject(
    windowPointX, windowPointY, windowPointZ,
    modelViewMatrix, projectionMatrix,
    viewportArray, modelPointArrayResults);

modelPointArrayResults[0] = <'x' model coordinate value>
modelPointArrayResults[1] = <'y' model coordinate value>
modelPointArrayResults[2] = <'z' model coordinate value>
```
