---
# Edge Detection
Leonhard Applis - 05.11.2018
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
<div>
<div><h3> Problem I: similiar colours</h3></div>
<div>
    <img src="images/simcolour.png" style="width: 60%; height: 60%; margin-top: 0px; border: none; background: none; box-shadow: none;"/> 
</div>
</div>
+++?image=images/gradientchange.jpg
### Problem II: minor changes

+++
<div>
<div><h3> Problem III: Random Noise</h3></div>
<div>
    <img src="images/noise.png" style="width: 60%; height: 60%; margin-top: 0px; border: none; background: none; box-shadow: none;"/> 
</div>
</div>
+++
### Definition
@quote[In Image Processing, an edge can be defined as a set of contiguous pixel positions where an abrupt change of intensity, gray- or color-values occur. Edges represent boundaries between objects and background. Sometimes, the edge-pixel-sequence may be broken due to insufficient intensity difference.](Malay K. Pakhira )

---
## The basics of gradient-based edgedetection

+++
@transition[none]

@snap[east]
![sample](images/greyball.PNG)
@snapend

@snap[north]
<h3> Image-requirements</h3>
@snapend

@snap[west]
Requirements: <br/>
<ol>
<li>1. color values known </li>
<li>2. picture scale known </li>
<li>3. load as pixelmatrix </li>
</ol>
@snapend

+++
<div style="align-items: center;">
<h3>One dimensional approach</h3> 
    <div style="width:100% ; height=60%">
        <img src="images/1DGradient.png" style="width: 60%; height: 100%; margin-top: 0px; border: none; background: none; box-shadow: none;"/> 
    </div>
<div style="width:80% ; height=30%">
    take one row of the matrix, and plot a function and a derivative
</div>
</div>
+++
<div style="align-items: center ;">
    <div> Problem: Image can only be seen as discrete Function (Pixel per Pixel) </div>
    <div> Therefore: $$\dfrac{df}{dx}(u) \approx \dfrac{f(u+1) - f(u-1)}{(u+1)-(u-1)} = \dfrac{f(u+1) - f(u-1)}{2}$$ </div>   
</div>
+++
<div>
    <div>If working with full images,we got two dimensions and therefore two partial derivations:  </div>
    <div>$$I_x = \dfrac{\partial I}{\partial x}(u,v) , I_y = \dfrac{\partial I}{\partial y}(u,v)$$ </div>
    <div>the <b>gradient</b> at the point (u,v) is
        <img src="images/texGradient.JPG" style="width: 70%; height: 100%; margin-top: 0px; border: none; background: none; box-shadow: none;"/>
    </div>
    <div> and the <b>magnitude</b> <br/> $$|\nabla I|=\sqrt{I_x^2 + I_y^2}$$ </div>
</div>
+++
![2D Derivates](images/2DEdgeGradient.PNG)
+++
<div>
    <h3> Applying a filter </h3>
    <div>Transfering the gradient to a linear filter is simple:</div>
        <div>
        <img src="images/texLinIX.jpg" style="width: 30%; height: 100%; margin-top: 0px; border: none; background: none; box-shadow: none;"/> 
        <img src="images/texLinY.JPG" style="width: 30%; height: 100%; margin-top: 0px; border: none; background: none; box-shadow: none;"/> 
    </div>
</div>
---
## Advanced gradient-based edgedetection

+++
### Using 3x3 filters
basic Idea how we can apply 3x3 filters to our picture

+++
<div style="align-items: center;">
<h3>Prewitt Operator</h3> 
<div style="width:100% ; height=60%">
    <img src="images/texPrewittX.JPG" style="width: 40%; height: 100%; margin-top: 0px; border: none; background: none; box-shadow: none;"/> 
    <img src="images/texPrewittY.JPG" style="width: 40%; height:100% ; margin-top: 0px; border: none; background: none; box-shadow: none;"/>
</div>
<div style="width:80% ; height=30%">
<img src="images/texPrewittGradient.JPG" style="heigth: 150%; margin-top: 0px; border: none; background: none; box-shadow: none;"/>
</div>
</div>
+++
<div style="align-items: center;">
<h3>Sobel Operator</h3> 
<div style="width:100% ; height=60%">
<img src="images/texSobelX.JPG" style="width: 40%; height: 100%; margin-top: 0px; border: none; background: none; box-shadow: none;"/> 
<img src="images/texSobelY.JPG" style="width: 40%; height:80% ; margin-top: 0px; border: none; background: none; box-shadow: none;"/>
</div>
<div style="width:80% ; height=30%">
<img src="images/texSobelGradient.JPG" style="heigth: 80%; margin-top: 0px; border: none; background: none; box-shadow: none;"/>
</div>
</div>
+++
<div>
<h3>General Magnitude</h3>
    <div>
    <img src="images/texGeneralMagnitude.JPG" style="heigth: 150%; margin-top: 0px; border: none; background: none; box-shadow: none;"/>    
    </div>
    <div>holds for every Operator </div>
</div>
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