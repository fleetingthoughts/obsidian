---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.3 Vectors in Two Dimensions]]"
tags:
  - "#flashcard"
  - richard_courant
  - calculus
  - macro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Define the limit and derivative of a vector, then derive the formula for the derivative of a vector in terms of the differentiation of its elements.

Refer to the figure below. Given the acceleration vector, velocity vector, and the angle $\gamma$ between the two vectors, define the tangential and normal component of acceleration. With this definition, determine the following:
- Derive the relationship between the tangential component of acceleration with the magnitude of the velocity
- The magnitude of the normal component of acceleration with respect to its curvature
![](Pasted%20image%2020260726234230.png)
#### Notes
**Vector Limit and Derivative**
- **Limit:** A vector function $\mathbf{R}(t)$ approaches a limit $\mathbf{L}$ as $t \to t_0$ if $\lim_{t \to t_0} \Vert{}\mathbf{R}(t) - \mathbf{L}\Vert{} = 0$.
- **Derivative Definition:** The instantaneous rate of change vector: $\frac{d\mathbf{R}}{dt} = \lim_{\Delta t \to 0} \frac{\mathbf{R}(t + \Delta t) - \mathbf{R}(t)}{\Delta t}$.
- **Element-wise Derivation:** Let $\mathbf{R}(t) = x(t)\mathbf{i} + y(t)\mathbf{j} + z(t)\mathbf{k}$. Because the limit operator distributes linearly and the standard basis vectors are constant:$$\frac{d\mathbf{R}}{dt} = \lim_{\Delta t \to 0} \left( \frac{x(t+\Delta t)-x(t)}{\Delta t} \right)\mathbf{i} + \lim_{\Delta t \to 0} \left( \frac{y(t+\Delta t)-y(t)}{\Delta t} \right)\mathbf{j} + \dots$$$$\dot{\mathbf{R}}(t) = \dot{x}(t)\mathbf{i} + \dot{y}(t)\mathbf{j} + \dot{z}(t)\mathbf{k}$$

	**Acceleration Components**
- **Tangential Acceleration ($a_T$):** The projection of the acceleration vector $\ddot{\mathbf{R}}$ onto the velocity vector $\dot{\mathbf{R}}$. It measures the rate of change of the _magnitude_ of velocity (speed).
- **Normal Acceleration ($a_N$):** The orthogonal component of acceleration perpendicular to the velocity, directed inward toward the center of curvature. It measures the rate of change of the _direction_ of velocity.
**Kinematic Derivations & Significance**
- **Tangential to Velocity Magnitude:** Let $v = \Vert{}\dot{\mathbf{R}}\Vert{}$ represent speed. The tangential component is the direct scalar time-derivative of this speed: $a_T = \dot{v}$. From the given angle $\gamma$, $a_T = \Vert{}\ddot{\mathbf{R}}\Vert{} \cos \gamma$. _Significance:_ Captures pure scalar acceleration along the path trajectory without altering direction.
- **Normal to Curvature:** The normal component acts as a function of the path's instantaneous curvature $\kappa$ and the square of the speed: $a_N = \kappa v^2$. From the given angle $\gamma$, $a_N = \Vert{}\ddot{\mathbf{R}}\Vert{} \sin \gamma$. _Significance:_ Quantifies the centripetal acceleration required to steer the vector strictly along the geometric curve.
