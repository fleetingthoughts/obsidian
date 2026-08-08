---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (h). Curvature]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Show that the circle that osculates with a curve at a given point has a radius equal to the reciprocal of the curvature at the point
#### Notes
- **1. Parametrize a Circle:** Define an arbitrary circle of radius $R$ using arc length $s$ as the parameter: $\mathbf{r}(s) = (R \cos(s/R), R \sin(s/R))$.

- **2. Unit Tangent Vector ($\mathbf{T}$):** Differentiate the position vector with respect to $s$: $\mathbf{T}(s) = \mathbf{r}'(s) = (-\sin(s/R), \cos(s/R))$.
    
- **3. Curvature Vector ($d\mathbf{T}/ds$):** Differentiate the tangent vector to find its rate of change: $\mathbf{T}'(s) = (-\frac{1}{R}\cos(s/R), -\frac{1}{R}\sin(s/R))$.
    
- **4. Calculate Curvature ($\kappa$):** Curvature is defined as the magnitude of $\mathbf{T}'(s)$: $\kappa = \Vert{}\mathbf{T}'(s)\Vert{} = \sqrt{\frac{1}{R^2}\cos^2(s/R) + \frac{1}{R^2}\sin^2(s/R)} = \frac{1}{R}$.
    
- **5. Conclusion:** Rearranging $\kappa = \frac{1}{R}$ yields $R = \frac{1}{\kappa}$. Because an osculating circle makes second-order contact with a curve at a given point, it perfectly shares the curve's curvature $\kappa$ at that exact location, inherently mandating its radius be the reciprocal of that shared curvature.