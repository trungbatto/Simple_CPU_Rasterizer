# CPU Software Rasterizer

A CPU-based 3D software rasterizer written in C using SDL2.
This project implements a complete 3D graphics pipeline entirely on the CPU without relying on GPU rasterization APIs such as OpenGL or DirectX.

The renderer supports mesh loading, clipping, perspective projection, textured triangle rasterization, z-buffering, back-face culling, camera movement, and multiple rendering modes.

## Features

* CPU triangle rasterization
* Perspective projection
* World, view, and projection matrix transformations
* OBJ mesh loading
* PNG texture loading
* Perspective-correct texture mapping
* Back-face culling
* Frustum clipping
* Directional lighting
* Z-buffer depth testing
* Multiple render modes
* Camera movement and rotation

## Technologies

* C
* SDL2
* uPNG

## Controls

### Render Modes

    | Key | Action                         |
    | --- | ------------------------------ |
    | 1   | Wireframe vertices             |
    | 2   | Wireframe                      |
    | 3   | Filled triangles               |
    | 4   | Filled triangles + wireframe   |
    | 5   | Textured rendering             |
    | 6   | Textured rendering + wireframe |

### Culling

    | Key | Action                    |
    | --- | ------------------------- |
    | C   | Enable back-face culling  |
    | X   | Disable back-face culling |

### Camera Controls

    | Key         | Action                   |
    | ----------- | ------------------------ |
    | Up Arrow    | Move forward             |
    | Down Arrow  | Move backward            |
    | Left Arrow  | Rotate camera left       |
    | Right Arrow | Rotate camera right      |
    | W           | Rotate camera pitch up   |
    | S           | Rotate camera pitch down |
    | ESC         | Exit program             |

## Graphics Pipeline

The renderer processes geometry through the following stages:
  
    1. Model Space
    2. World Space
    3. Camera/View Space
    4. Frustum Clipping
    5. Perspective Projection
    6. Perspective Divide
    7. Screen Space Transformation
    8. Triangle Rasterization

## Scene

The demo scene contains:

    * Runway environment
    * F-22 model
    * Eurofighter model
    * F-117 model

## Build Instructions

### Requirements

* Visual Studio 2022 (recommended)

### Running the Project

1. Open the `.sln` file in Visual Studio.
2. Build the project in `x86 Debug`.
3. Run the executable.

## Screenshots

Add screenshots or GIFs here.
