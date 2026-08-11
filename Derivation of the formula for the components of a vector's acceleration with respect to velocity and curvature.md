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

### Tangential and Normal Acceleration (Scalar Derivation)

Let the instantaneous direction of motion be defined by the angle of inclination $\phi$, and let $v = \frac{ds}{dt}$ be the speed. Adopting the notation from the text, let $\gamma$ be the angle formed by the total acceleration magnitude $a$ with the instantaneous direction of motion.

The tangential component of acceleration is thus the projection $a \cos \gamma$, and the normal component is the projection $a \sin \gamma$.

#### 1. Velocity Components

The Cartesian velocity components are expressed using the speed and the angle of inclination $\phi$:

$$\dot{x} = v \cos \phi$$

$$\dot{y} = v \sin \phi$$

#### 2. Acceleration Components

Differentiating with respect to time $t$ yields the acceleration components:

$$\ddot{x} = \dot{v} \cos \phi - v \dot{\phi} \sin \phi$$

$$\ddot{y} = \dot{v} \sin \phi + v \dot{\phi} \cos \phi$$

#### 3. Tangential Component ($a \cos \gamma$)

The tangential component is the projection of the acceleration onto the direction of motion. We multiply the components by $\cos \phi$ and $\sin \phi$:

$$a \cos \gamma = \ddot{x} \cos \phi + \ddot{y} \sin \phi$$

$$a \cos \gamma = (\dot{v} \cos \phi - v \dot{\phi} \sin \phi)\cos \phi + (\dot{v} \sin \phi + v \dot{\phi} \cos \phi)\sin \phi$$

$$a \cos \gamma = \dot{v}\cos^2 \phi - v \dot{\phi} \sin \phi \cos \phi + \dot{v}\sin^2 \phi + v \dot{\phi} \sin \phi \cos \phi$$

$$a \cos \gamma = \dot{v}(\cos^2 \phi + \sin^2 \phi)$$

$$a \cos \gamma = \dot{v} = \frac{dv}{dt}$$

#### 4. Normal Component ($a \sin \gamma$)

The normal component is the projection perpendicular to the motion. We multiply by $-\sin \phi$ and $\cos \phi$:

$$a \sin \gamma = -\ddot{x} \sin \phi + \ddot{y} \cos \phi$$

$$a \sin \gamma = -(\dot{v} \cos \phi - v \dot{\phi} \sin \phi)\sin \phi + (\dot{v} \sin \phi + v \dot{\phi} \cos \phi)\cos \phi$$

$$a \sin \gamma = -\dot{v}\sin\phi\cos\phi + v\dot{\phi}\sin^2 \phi + \dot{v}\sin\phi\cos\phi + v\dot{\phi}\cos^2 \phi$$

$$a \sin \gamma = v\dot{\phi}(\sin^2 \phi + \cos^2 \phi)$$

$$a \sin \gamma = v\dot{\phi}$$

#### 5. Relation to Curvature ($\kappa$)

Curvature is the rate of change of the angle of inclination with respect to arc length: $\kappa = \frac{d\phi}{ds}$.

Using the chain rule:

$$\dot{\phi} = \frac{d\phi}{dt} = \frac{d\phi}{ds} \frac{ds}{dt} = \kappa v$$

Substituting this into the normal component formula yields the final result:

$$a \sin \gamma = v(\kappa v) = \kappa v^2$$
