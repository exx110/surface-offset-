This repository demonstrates how to extract the velocity field 3 m above complex terrain in OpenFOAM using a normal-offset surface generated from an STL terrain mesh.

Instead of slicing in ParaView, this workflow automatically generates a terrain-following sampling surface using OpenFOAM’s distanceSurface and samples the velocity field U on it.

The resulting surface follows the terrain and remains exactly 3 m away from the ground along the surface normal.

Use Cases

This method is useful for:

wind resource assessment

wind comfort analysis

atmospheric boundary layer studies

terrain-following flow analysis

automated CFD post-processing

Method

The workflow uses the OpenFOAM surfaces function object with distanceSurface.

Steps:

Import terrain STL

Generate a surface offset 3 m from terrain

Sample velocity U on that surface

Export sampled data
