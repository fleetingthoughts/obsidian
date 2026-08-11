---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.3 Vectors in Two Dimensions]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Use the definition of curve length of a parametrically defined function to derive the formula for the curve length of a curve defined by a position vector.
#### Notes
- **Parametric Definition:** The standard arc length for a curve parametrically defined by $x(t)$, $y(t)$, and $z(t)$ from $t=a$ to $t=b$ is $L = \int_a^b \sqrt{(x'(t))^2 + (y'(t))^2 + (z'(t))^2} \, dt$.
    
- **Position Vector:** Let the curve be defined by the vector function $\mathbf{R}(t) = x(t)\mathbf{i} + y(t)\mathbf{j} + z(t)\mathbf{k}$.
    
- **Derivative (Velocity):** The derivative with respect to $t$ is $\mathbf{R}'(t) = x'(t)\mathbf{i} + y'(t)\mathbf{j} + z'(t)\mathbf{k}$.
    
- **Magnitude:** The Euclidean norm (magnitude) of this derivative vector is strictly equivalent to the integrand of the parametric definition: $\Vert{}\mathbf{R}'(t)\Vert{} = \sqrt{(x'(t))^2 + (y'(t))^2 + (z'(t))^2}$.
    
- **Vector Formula:** Substituting the magnitude into the original integral yields the simplified vector formula for arc length: $L = \int_a^b \Vert{}\mathbf{R}'(t)\Vert{} \, dt$.
