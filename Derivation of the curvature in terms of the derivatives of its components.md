---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (h). Curvature]]"
tags:
  - "#flashcard"
  - macro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Derive the formulas for the curvature:
$$\kappa = \frac{x'y'' - y'x''}{((x')^2 + (y')^2)^{3/2}}$$
and in polar form:$$\kappa = \frac{r^2 + 2\left(\frac{dr}{d\theta}\right)^2 - r\frac{d^2r}{d\theta^2}}{\left(r^2 + \left(\frac{dr}{d\theta}\right)^2\right)^{3/2}}$$
#### Notes
Curvature is the rate of change of the angle of inclination with respect to arc length: $\kappa = \frac{d\phi}{ds} = \frac{d\phi/dt}{ds/dt}$.

Given $\tan \phi = \frac{\dot{y}}{\dot{x}}$, differentiating with respect to $t$ gives the numerator:

$$\sec^2 \phi \cdot \dot{\phi} = \frac{\dot{x}\ddot{y} - \dot{y}\ddot{x}}{\dot{x}^2} \implies \dot{\phi} = \frac{\dot{x}\ddot{y} - \dot{y}\ddot{x}}{\dot{x}^2 + \dot{y}^2}$$

The rate of change of arc length gives the denominator:

$$\frac{ds}{dt} = \sqrt{\dot{x}^2 + \dot{y}^2}$$

Dividing $\dot{\phi}$ by $\frac{ds}{dt}$ yields the parametric curvature:

$$\kappa = \frac{\dot{x}\ddot{y} - \dot{y}\ddot{x}}{(\dot{x}^2 + \dot{y}^2)^{3/2}}$$

### 2. Curvature in Polar Coordinates

For a polar curve $r(\theta)$, map to Cartesian coordinates $x = r\cos\theta$ and $y = r\sin\theta$. Using $\theta$ as the parameter $t$, calculate the derivatives.

The denominator term $(\dot{x}^2 + \dot{y}^2)$ simplifies via the Pythagorean identity to:

$$\dot{x}^2 + \dot{y}^2 = r^2 + \dot{r}^2$$

The numerator term $(\dot{x}\ddot{y} - \dot{y}\ddot{x})$ expands and simplifies to:

$$\dot{x}\ddot{y} - \dot{y}\ddot{x} = r^2 + 2\dot{r}^2 - r\ddot{r}$$

Substituting these directly into the parametric formula yields the polar curvature:

$$\kappa = \frac{r^2 + 2\dot{r}^2 - r\ddot{r}}{(r^2 + \dot{r}^2)^{3/2}}$$
