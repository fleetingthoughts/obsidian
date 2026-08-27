---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (k). Integrals Expressing Area within Closed Curves]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
  - richard_courant
  - calculus
date_created: 2026-07-24
---
Geometrically derive the the area of a closed loop with a counter-clockwise sense in terms of the integral $-\int ydx=-\int yx' dt$ where $t$ is the variable used to parametrically define the curve. With this integral determine the following:
- Derive two other forms of this integral for a parametrically defined curve.
- Use these forms to determine the area of a closed curve in polar coordinates.
#### Notes
- **Geometric Derivation:** Integrating $\int y\,dx$ around a counter-clockwise loop calculates the signed area down to the $x$-axis. The upper path traverses right-to-left ($dx < 0$), yielding a negative integral. The lower path traverses left-to-right ($dx > 0$), yielding a positive integral. Negating their sum isolates the positive enclosed area: $A = -\oint y\,dx = -\int yx'\,dt$.
- **Alternative Form 1 ($x\,dy$):** Applying the product rule over a closed loop yields zero net change: $\oint d(xy) = \oint x\,dy + \oint y\,dx = 0$. Rearranging this identity provides a second area formula: $A = \oint x\,dy = \int xy'\,dt$.
- **Alternative Form 2 (Symmetric):** Averaging the two individual area integrals produces the standard symmetric equation (Green's Theorem for area): $A = \frac{1}{2}\oint (x\,dy - y\,dx) = \frac{1}{2}\int (xy' - yx')\,dt$.
- **Polar Coordinate Area:** Substitute $x = r\cos\theta$ and $y = r\sin\theta$ into the symmetric form, treating $\theta$ as the parameter $t$. Evaluating the term $xy' - yx'$ yields $(r\cos\theta)(r'\sin\theta + r\cos\theta) - (r\sin\theta)(r'\cos\theta - r\sin\theta) = r^2(\cos^2\theta + \sin^2\theta) = r^2$. The symmetric integral simplifies directly to $A = \frac{1}{2}\int r^2\,d\theta$.
