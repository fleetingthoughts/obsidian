---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (h). Curvature]]"
tags:
  - "#flashcard"
  - macro/math/courant_calc1/ch4
date_created: 2026-07-24
---
Prove that the curvature of a curve defined parametrically by $t$ is invariant to a reparameterization by $\theta(t)$ that is monotonic.
#### Notes
Let the parameter change to $t = \phi(\tau)$, strictly where $\phi'(\tau) > 0$. Let dot ($\dot{x}$) denote derivatives with respect to $\tau$, and prime ($x'$) denote derivatives with respect to $t$.

By the Chain and Product Rules:

$$\dot{x} = x'\phi' \quad \text{and} \quad \ddot{x} = x''(\phi')^2 + x'\ddot{\phi}$$

$$\dot{y} = y'\phi' \quad \text{and} \quad \ddot{y} = y''(\phi')^2 + y'\ddot{\phi}$$

- **The Numerator:** Compute the cross-product $\dot{x}\ddot{y} - \dot{y}\ddot{x}$:
    
    $$\dot{x}\ddot{y} = (x'\phi')[y''(\phi')^2 + y'\ddot{\phi}] = x'y''(\phi')^3 + x'y'\phi'\ddot{\phi}$$
    
    $$\dot{y}\ddot{x} = (y'\phi')[x''(\phi')^2 + x'\ddot{\phi}] = y'x''(\phi')^3 + y'x'\phi'\ddot{\phi}$$
    
    Subtracting them perfectly cancels the $x'y'\phi'\ddot{\phi}$ terms, leaving:
    
    $$\dot{x}\ddot{y} - \dot{y}\ddot{x} = (x'y'' - y'x'')(\phi')^3$$
    
- **The Denominator:** Compute the sum of squares $(\dot{x}^2 + \dot{y}^2)^{3/2}$:
    
    $$\dot{x}^2 + \dot{y}^2 = (x'\phi')^2 + (y'\phi')^2 = (\phi')^2(x'^2 + y'^2)$$
    
    Because $\phi' > 0$, we can cleanly evaluate the exponent $3/2$ without sign changes:
    
    $$(\dot{x}^2 + \dot{y}^2)^{3/2} = (\phi')^3(x'^2 + y'^2)^{3/2}$$
    

When dividing the transformed numerator by the transformed denominator, the $(\phi')^3$ term cleanly divides out from both, leaving the original expression **invariant**.
