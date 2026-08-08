---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.3 Vectors in Two Dimensions]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
  - calculus
  - richard_courant
date_created: 2026-07-24
---
Define the following:
- Positional vector $\mathbf{R}=(a,b)$
- The direction cosines of the angle with the positive $x$-axis
- The dot and cross product of two vectors in terms of their elements
- The magnitude of a vector
Use these definitions to then determine a relationship between the dot product and cross product with the angle $\theta$ between any two vectors $\mathbf{R}$ and $\mathbf{R^*}$ and their magnitudes.  
#### Notes

**Vector Definitions**

- **Positional Vector $\mathbf{R} = (a, b)$:** Anchored at origin $(0,0)$ with terminal point at $(a, b)$.
- **Direction Cosine:** Angle $\alpha$ with positive $x$-axis: $\cos \alpha = \frac{a}{\Vert{}\mathbf{R}\Vert{}}$.
- **Dot Product:** Sum of entry products: $\mathbf{R} \cdot \mathbf{R}^* = aa^* + bb^* + cc^*$.
- **Cross Product:** Perpendicular vector: $\mathbf{R} \times \mathbf{R}^* = (bc^* - cb^*)\mathbf{i} - (ac^* - ca^*)\mathbf{j} + (ab^* - ba^*)\mathbf{k}$.
- **Magnitude:** Euclidean length: $\Vert{}\mathbf{R}\Vert{} = \sqrt{a^2 + b^2 + c^2}$.

Formulas for angle $\theta$ between $\mathbf{R}$ and $\mathbf{R}^*$: $\mathbf{R} \cdot \mathbf{R}^* = \Vert{}\mathbf{R}\Vert{}\Vert{}\mathbf{R}^*\Vert{} \cos \theta$ and $\Vert{}\mathbf{R} \times \mathbf{R}^*\Vert{} = \Vert{}\mathbf{R}\Vert{}\Vert{}\mathbf{R}^*\Vert{} \sin \theta$.
- **1. Tangent Relationship (Ratio):** Dividing cross by dot product yields $\tan \theta = \frac{\Vert{}\mathbf{R} \times \mathbf{R}^*\Vert{}}{\mathbf{R} \cdot \mathbf{R}^*}$.
- **2. Lagrange's Identity (Sum of Squares):** Applying $\sin^2 \theta + \cos^2 \theta = 1$ yields $\Vert{}\mathbf{R} \times \mathbf{R}^*\Vert{}^2 + (\mathbf{R} \cdot \mathbf{R}^*)^2 = \Vert{}\mathbf{R}\Vert{}^2 \Vert{}\mathbf{R}^*\Vert{}^2$.
