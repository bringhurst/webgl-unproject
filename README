WebGL Unproject
===============

This is a port of the usual gluUnProject function to javascript for use in WebGL applications. To use, read the included JSDoc for the unProject function -- it closely matches the API for the common C variant of the same function.

Simple Example
==============

    var modelPointArrayResults = [];
    
    var success = GLU.unProject(
        windowPointX, windowPointY, windowPointZ,
        modelViewMatrix, projectionMatrix,
        viewportArray, modelPointArrayResults);
    
    modelPointArrayResults[0] = ... // x model coordinate
    modelPointArrayResults[1] = ... // y model coordinate
    modelPointArrayResults[2] = ... // z model coordinate
