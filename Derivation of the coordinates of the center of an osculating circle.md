---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (h). Curvature]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Derive the coordinates for the center of an osculating circle.
#### Notes
- **1. Define Tangent Angle:** For a curve $y = f(x)$ at point $(x, y)$, the tangent angle $\phi$ relates to the first derivative via $\tan \phi = y'$.
    
- **2. Normal Components:** By geometric properties, the horizontal and vertical projection components of the unit normal vector are $-\sin \phi = -\frac{y'}{\sqrt{1+(y')^2}}$ and $\cos \phi = \frac{1}{\sqrt{1+(y')^2}}$.
    
- **3. Radius of Curvature:** The scalar distance to the center of the circle is $R = \frac{(1 + (y')^2)^{3/2}}{y''}$.
    
- **4. Shift to Center:** The coordinates $(X_c, Y_c)$ are found by shifting distance $R$ along the normal line from the original point: $X_c = x - R \sin \phi$ and $Y_c = y + R \cos \phi$.
    
- **5. Final Equations:** Substituting $R$ and the trigonometric components into the shift equations cancels the square root denominators to yield the exact center coordinates.
    

$$X_c = x - \frac{y'(1 + (y')^2)}{y''}$$

$$Y_c = y + \frac{1 + (y')^2}{y''}$$

