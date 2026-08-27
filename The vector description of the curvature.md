---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.3 Vectors in Two Dimensions]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Derive the formula for the curvature of a curve defined by a position vector $\bf{R}(t)$ 
#### Notes
- **1. Velocity and Unit Tangent:** The velocity vector is $\mathbf{R}'(t) = v(t)\mathbf{T}(t)$, where speed is $v(t) = \Vert{}\mathbf{R}'(t)\Vert{} = \frac{ds}{dt}$.
    
- **2. Acceleration Vector:** Differentiating velocity using the product rule yields acceleration: $\mathbf{R}''(t) = v'(t)\mathbf{T}(t) + v(t)\mathbf{T}'(t)$.
    
- **3. Chain Rule for $\mathbf{T}'(t)$:** By definition, $\frac{d\mathbf{T}}{ds} = \kappa\mathbf{N}$. Applying the chain rule gives the time derivative: $\mathbf{T}'(t) = \frac{d\mathbf{T}}{ds}\frac{ds}{dt} = \kappa v(t)\mathbf{N}$.
    
- **4. Substitute and Cross Multiply:** Substitute $\mathbf{T}'(t)$ into the acceleration equation: $\mathbf{R}''(t) = v'(t)\mathbf{T}(t) + \kappa v^2(t)\mathbf{N}(t)$. Now, take the cross product of velocity and acceleration: $\mathbf{R}'(t) \times \mathbf{R}''(t) = (v\mathbf{T}) \times (v'\mathbf{T} + \kappa v^2\mathbf{N})$.
    
- **5. Simplify:** Because the cross product of parallel vectors is zero ($\mathbf{T} \times \mathbf{T} = \mathbf{0}$) and $\mathbf{T} \times \mathbf{N} = \mathbf{B}$ (the unit binormal vector), the equation simplifies to $\mathbf{R}'(t) \times \mathbf{R}''(t) = \kappa v^3\mathbf{B}$.
    
- **6. Final Formula:** Take the magnitude of both sides. Since $\Vert{}\mathbf{B}\Vert{} = 1$, we get $\Vert{}\mathbf{R}'(t) \times \mathbf{R}''(t)\Vert{} = \kappa v^3$. Solving for $\kappa$ and substituting $v = \Vert{}\mathbf{R}'(t)\Vert{}$ yields:
    
    $$\kappa = \frac{\Vert{}\mathbf{R}'(t) \times \mathbf{R}''(t)\Vert{}}{\Vert{}\mathbf{R}'(t)\Vert{}^3}$$
