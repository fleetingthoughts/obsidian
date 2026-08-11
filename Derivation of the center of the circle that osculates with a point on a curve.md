---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (h). Curvature]]"
tags:
  - "#flashcard"
  - macro/math/courant_calc1/ch4
  - richard_courant
  - calculus
date_created: 2026-07-24
---
Derive the coordinates of the center of the circle that osculates with a parametrically defined curve at the point $(x(t_o),y(t_o))$.
#### Notes
Let $\rho$ be the radius of curvature and $\alpha$ be the angle of the tangent to the positive $x$-axis. The center of curvature lies along the normal line at a distance of $\rho$ from $P$. For positive curvature ($\kappa > 0$), the direction to the center forms an angle of $\alpha + \frac{\pi}{2}$.

Using the geometric components of the tangent line ($\dot{x}, \dot{y}$), we can state the coordinate offsets:

$$\frac{\xi - x}{\rho} = \cos\left(\alpha + \frac{\pi}{2}\right) = -\sin \alpha = \frac{-\dot{y}}{\sqrt{\dot{x}^2 + \dot{y}^2}}$$

$$\frac{\eta - y}{\rho} = \sin\left(\alpha + \frac{\pi}{2}\right) = \cos \alpha = \frac{\dot{x}}{\sqrt{\dot{x}^2 + \dot{y}^2}}$$

Multiplying by $\rho$ and isolating $\xi$ and $\eta$ yields the center coordinates:

$$\xi = x - \frac{\rho \dot{y}}{\sqrt{\dot{x}^2 + \dot{y}^2}}$$

$$\eta = y + \frac{\rho \dot{x}}{\sqrt{\dot{x}^2 + \dot{y}^2}}$$

> **Note:** If arc length $s$ is used as the parameter $t$, then $\sqrt{\dot{x}^2 + \dot{y}^2} = 1$, reducing the formulas to $\xi = x - \rho \dot{y}$ and $\eta = y + \rho \dot{x}$.
