---
parent: "[[Introduction to Calculus I by Fritz and Courant - 4.1 Theory of Plane Curves (a-c)]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch4
  - richard_courant
  - calculus
date_created: 2026-07-24
---
Define the following:
- Simple curve
- Orientation of a curve defined parametrically by $x=\theta (t)$ and y = $\psi (t)$.
- Arc length of the curve as a Riemann sum and passage through the limit
#### Notes
- **Simple Curve:** A curve that does not cross itself; for a parameterization $\mathbf{r}(t)$ on an interval $[a, b]$, $\mathbf{r}(t_1) \neq \mathbf{r}(t_2)$ for all $t_1 \neq t_2$ within the open interval $(a, b)$.
    
- **Orientation:** The inherent direction of traversal along the geometric path as the independent parameter $t$ strictly increases for the coordinate functions $x = \theta(t)$ and $y = \psi(t)$.
    
- **Arc Length (Riemann Sum to Limit):** Partition the parameter interval into subintervals of width $\Delta t_i$. Approximate the curve's length by summing linear secant segments: $L \approx \sum_{i=1}^n \sqrt{(\Delta x_i)^2 + (\Delta y_i)^2}$. Applying the Mean Value Theorem to the coordinate functions translates this into the Riemann sum $\sum_{i=1}^n \sqrt{(\theta'(t_i^*))^2 + (\psi'(t_i^*))^2}\Delta t_i$. Passing through the limit as the maximum partition width approaches zero ($\Vert{}\Delta P\Vert{} \to 0$) yields the exact integral: $L = \int_a^b \sqrt{(\theta'(t))^2 + (\psi'(t))^2} \, dt$.
