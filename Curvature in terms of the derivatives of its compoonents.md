---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (h). Curvature]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
  - math
  - richard_courant
  - calculus
date_created: 2026-07-24
---
Define the curvature as a derivative of the angle with the positive x-axis. Derive the formula the curvature in terms of the derivative of its $x$ and $y$ components
#### Notes
**Curvature by Tangent Angle**
- **Definition:** Curvature $\kappa$ is the instantaneous rate of change of the tangent angle $\phi$ (relative to the positive $x$-axis) with respect to the arc length $s$: $\kappa = \frac{d\phi}{ds}$.

**Derivation from Parametric Components**
- **1. Tangent Angle:** The slope relates to the parametric components via $\tan \phi = \frac{dy}{dx} = \frac{y'}{x'}$.
- **2. Differentiate with respect to $t$:** Differentiating both sides and applying the quotient rule yields: $\sec^2 \phi \cdot \frac{d\phi}{dt} = \frac{x'y'' - y'x''}{(x')^2}$.
- **3. Trig Substitution:** By the Pythagorean identity, $\sec^2 \phi = 1 + \tan^2 \phi = 1 + \left(\frac{y'}{x'}\right)^2 = \frac{(x')^2 + (y')^2}{(x')^2}$. Substitute this back to isolate $\frac{d\phi}{dt}$: $\frac{d\phi}{dt} = \frac{x'y'' - y'x''}{(x')^2 + (y')^2}$.
- **4. Arc Length Derivative:** The rate of change of the arc length with respect to parameter $t$ is $\frac{ds}{dt} = \sqrt{(x')^2 + (y')^2}$.
- **5. Chain Rule & Final Formula:** Substitute these derivations into the expanded definition $\kappa = \frac{d\phi/dt}{ds/dt}$ to yield the exact parametric curvature formula:
$$\kappa = \frac{x'y'' - y'x''}{((x')^2 + (y')^2)^{3/2}}$$
