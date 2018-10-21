---
# Edge Detection

+++
## Table of Contents
1. What makes an edge?
2. Basics of gradient-based edgedetection
3. Advanced gradient-based edgedetection
4. compass operators
5. (can be left) medical use

---
## What makes an edge?

+++
### Problem I
Picture of Low-Contrast Edge (e.g. orange edge in yellow picture)

![Image](/template/img/SimColour.png)

+++
### Problem II
Picture of fade-out-edge
![Image](/template/img/gradientchange.jpg)

+++
### Problem III
Picture of thick edge (basicly new item)

+++
### Problem IV
![Image](/template/img/noise.png )

+++
### Definition
In Image Processing, an edge can be defined as a set of contiguous pixel positions where an abrupt change of intensity (gray or color) values occur. Edges represent boundaries between objects and background. Sometimes, the edge-pixel-sequence may be broken due to insufficient intensity difference. (Malay K. Pakhira )

---
## The basics of gradient-based edgedetection

+++
### Image as Pixelmatrix
Just show what i'm working on, and what we are talking about
Figure of a picture with a grid-raster on it
+++
### One dimensional approach
Take one row of pixels from the previous picture to show how we use the derivative of the discrete function

+++
### Two dimensional approach
show why we need a real gradient when we have 2 Dimensions

+++
### Applying a filter
show how to scale the derivatives and why its usefull

---
## Advanced gradient-based edgedetection

+++
### Using 3x3 filters
basic Idea how we can apply 3x3 filters to our picture

+++
### Prewitt Operator

+++
### Sobel Operator

+++
### Calculating the direction
show arctang and what it does

show possible problems

---
## Compass Operators
Idea and Main Problems (Tradeoff Edge-Detection and Direction-Detection)

+++
### Extended Sobel Operator
Show the Extended Sobel operators and why we have 8 of them now, what we are doing with them and why its good.

+++
### Kirsch Operator
i guess just presenting it would be enough, if i explain a lot at the extended sobel

+++
### Canny-Edge Operator
why its the "best" and how it works with 2nd derivative

---
## Edge sharpening

+++
### Smoothing

---
## Medical use
Iff i still have time to fill or i find something very nice dudes

---
## Questions
also list primary sources here