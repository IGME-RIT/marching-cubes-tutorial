# Marching Cubes Tutorial

In this demo we construct a Sphere using marching cubes algorithm.

# About

Marching cubes is a algorithm to construct isosurfaces for oddly shaped objects, like fluids. It can be used to attain higher detail at lower memory cost.

We divide the space into symmetric cubes. these cubes can be subdivided into smaller cubes for better resolution. This structure resembles that of a oct-tree. For each vertex of every cube, we check if that vertex constitutes a part of the surface. Since each vertex can either be a part or not, we have a combination of 2^8 different scenarios. But these can be reduced to 15 unique cases which  can be transformed to reproduce the other formations.

These 8 values can be stored in 1 byte using each bit to represent a corner. In this example, we are using boolean variables instead, for ease of understanding.  

In this example, all the logic is in the setup().

# Setup

In order to setup, run the following in a shell, then open the project in your preferred editor. Windows setup has been configured for use with Visual Studio.

Windows:
```
cd path/to/folder
setup.cmd
```
Linux:
```
cd path/to/folder
./setup
```

# Credits

For more reading, check out the following links:
  - [Technical exploration of Adaptive Cube Tessalation](https://www.jvrb.org/past-issues/5.2008/1309)
  - [Wikipedia overview of the Marching Cubes algorithm](https://en.wikipedia.org/wiki/Marching_cubes)
  - [Visual demo for understanding the algorithm](https://www.youtube.com/watch?v=LfttaAepYJ8)
