---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (d-e).]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
  - math
  - richard_courant
  - calculus
date_created: 2026-07-24
---
Given a parametrically defined curve $(x(t),y(t))$, derive the equation for the tangent to the curve at a point $(x_o,y_o)$ on the curve.
#### Notes
- **1. Identify the Point:** Let the given point $(x_0, y_0)$ correspond to a specific parameter value $t_0$ such that $x(t_0) = x_0$ and $y(t_0) = y_0$.
    
- **2. Determine the Slope:** By the chain rule, the geometric slope $m = \frac{dy}{dx}$ is the ratio of the derivatives with respect to $t$: $m = \frac{y'(t_0)}{x'(t_0)}$, provided $x'(t_0) \neq 0$.
    
- **3. Point-Slope Equation:** Substitute the point and slope into the standard linear equation $Y - y_0 = m(X - x_0)$:
    
    $$Y - y_0 = \frac{y'(t_0)}{x'(t_0)}(X - x_0)$$
    
- **4. Symmetric Form:** Multiplying through by $x'(t_0)$ yields a generalized equation that remains valid even for vertical tangents (where $x'(t_0) = 0$):
    
    $$y'(t_0)(X - x_0) - x'(t_0)(Y - y_0) = 0$$
