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
@snap[north-east] ### Problem I: similiar colours @snapend
![Image](images/simcolour.png)

+++?image=images/gradientchange.jpg
### Problem II: minor changes

+++
### Problem III: random noise
![Image](images/noise.png )

+++
### Definition
@quote[In Image Processing, an edge can be defined as a set of contiguous pixel positions where an abrupt change of intensity, gray- or color-values occur. Edges represent boundaries between objects and background. Sometimes, the edge-pixel-sequence may be broken due to insufficient intensity difference.](Malay K. Pakhira )

---
## The basics of gradient-based edgedetection

+++
@transition[none]

@snap[north] <h3> Image-requirements</h3>@snapend

@snap[east]
![TestImage](/images/noise.png)
@snapend

@snap[west]
<b>Requirements:</b> <br/>
<ol>
<li>1. color values known </li>
<li>2. picture scale known </li>
<li>3. load picture as <br/> pixel-matrix </li>
</ol>
@snapend

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