--- @title[Edge Detection]
# Edge Detection

+++?include=template/md/list-content/PITCHME.md @title[Table of Contents]
## Table of Contents
1. What makes an edge?
2. Basics of gradient-based edgedetection
3. Advanced gradient-based edgedetection
4. compass operators
5. (can be left) medical use

--- @title[What makes an Edge?]
## What makes an edge?

+++?include=template/img/SimColour.png @title[Problem 1]
### Problem I
Picture of Low-Contrast Edge (e.g. orange edge in yellow picture)

+++?include=template/img/gradientchange.jpg @title[Problem 2]
### Problem II
Picture of fade-out-edge

+++ @title[Problem 3]
### Problem III
Picture of thick edge (basicly new item)

+++?include=template/img/noise.png @title[Problem 4]
### Problem IV

+++ @title[Definition]
### Definition

@snap[east text-white span-50]
@quote[In Image Processing, an edge can be defined as a set of contiguous pixel positions where an abrupt change of intensity (gray or color) values occur. Edges represent boundaries between objects and background. Sometimes, the edge-pixel-sequence may be broken due to insufficient intensity difference.](Malay K. Pakhira )
@snapend

--- @title[The Basics for Gradient-Based edgedetection]
## The basics of gradient-based edgedetection

+++ @title[Image as Pixel Matrix]
### Image as Pixelmatrix
Just show what i'm working on, and what we are talking about
Figure of a picture with a grid-raster on it
+++ @title[One Dimensional Approach]
### One dimensional approach
Take one row of pixels from the previous picture to show how we use the derivative of the discrete function
+++ @title[Two Dimensional Approach]
### Two dimensional approach
show why we need a real gradient when we have 2 Dimensions
+++ @title[Applying a filter]
### Applying a filter
show how to scale the derivatives and why its usefull
--- @title[Advanced Gradient-Based Edgedetection]
## Advanced gradient-based edgedetection
+++ @title[Using 3x3 Filters]
### Using 3x3 filters
basic Idea how we can apply 3x3 filters to our picture
+++ @title[Prewitt Operator]
### Prewitt Operator
+++ @title[Sobel Operator]
### Sobel Operator
+++ @title[Getting the Direction]
### Calculating the direction
show arctang and what it does

show possible problems
--- @title[Compass Operators]
## Compass Operators
Idea and Main Problems (Tradeoff Edge-Detection and Direction-Detection)
+++ @title[Extended Sobel operator]
### Extended Sobel Operator
Show the Extended Sobel operators and why we have 8 of them now, what we are doing with them and why its good.
+++ @title[Kirsch Operator]
### Kirsch Operator
i guess just presenting it would be enough, if i explain a lot at the extended sobel
+++ @title[Canny-Edge Operator]
### Canny-Edge Operator
why its the "best" and how it works with 2nd derivative

--- @title[Edge Sharpening]
## Edge sharpening
+++ @title[Smoothing]
### Smoothing
--- @title[Possible Addition: Use in Medicine]
## Medical use
Iff i still have time to fill or i find something very nice dudes
--- @title[Questions and Discussions]
## Questions
also list primary sources here