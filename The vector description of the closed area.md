---
parent: "[Introduction to Calculus I by Fritz and Courant - 4.3 Vectors in Two Dimensions](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%204.3%20Vectors%20in%20Two%20Dimensions.md)"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
  - richard_courant
  - calculus
date_created: 2026-07-24
---
Given a curve described by a vector function $\mathbf{R}(t)=(x(t),y(t))$, derive the formula of a closed area in terms of the position vector.
#### Notes
- **1. Symmetric Area Integral:** Recall the standard parametric area formula for a closed counter-clockwise loop: $A = \frac{1}{2}\int_a^b (x(t)y'(t) - y(t)x'(t))\,dt$.
    
- **2. Vector Definition:** Embed the 2D position vector and its differential (velocity) in 3D space to utilize the cross product: $\mathbf{R}(t) = x(t)\mathbf{i} + y(t)\mathbf{j}$ and $\mathbf{R}'(t) = x'(t)\mathbf{i} + y'(t)\mathbf{j}$.
    
- **3. Evaluate Cross Product:** Compute the cross product $\mathbf{R}(t) \times \mathbf{R}'(t)$. The $x$ and $y$ components cancel out, yielding a vector strictly in the $z$-direction: $(x(t)y'(t) - y(t)x'(t))\mathbf{k}$.
    
- **4. Vector Formula:** The scalar term perfectly matches the symmetric integral's integrand. Substitute it back to define the area as half the integral of the cross product: $A = \frac{1}{2}\int_a^b (\mathbf{R}(t) \times \mathbf{R}'(t)) \cdot \mathbf{k} \, dt$.