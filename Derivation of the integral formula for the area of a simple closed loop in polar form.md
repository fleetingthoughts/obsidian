---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (h). Curvature]]"
tags:
  - "#flashcard"
  - macro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Derive the integral formula for the area of a simple closed loop in polar form.
#### Notes
### Brief Derivation: Polar Area Formula
Start with the Cartesian oriented area integral:
$$A = \frac{1}{2} \oint_C (x \, dy - y \, dx)$$
Substitute polar coordinates ($x = r\cos\theta, y = r\sin\theta$) and their differentials ($dx = \cos\theta dr - r\sin\theta d\theta, dy = \sin\theta dr + r\cos\theta d\theta$):
$$x \, dy - y \, dx = (r\cos\theta)(\sin\theta dr + r\cos\theta d\theta) - (r\sin\theta)(\cos\theta dr - r\sin\theta d\theta)$$
Expand and group terms (the $dr$ terms cancel):
$$x \, dy - y \, dx = r^2(\cos^2\theta + \sin^2\theta)d\theta = r^2 d\theta$$
Substitute back into the original integral:

$$A = \frac{1}{2} \oint_C r^2 \, d\theta$$
