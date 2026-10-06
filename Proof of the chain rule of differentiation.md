---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Let $f : A \to \mathbf{R}$ and $g : B \to \mathbf{R}$ satisfy $f(A) \subseteq B$. If $f$ is differentiable at $c \in A$ and $g$ is differentiable at $f(c) \in B$, then $(g \circ f)'(c) = g'(f(c)) \cdot f'(c)$.
#### Notes
- Define $d(y) = \frac{g(y) - g(f(c))}{y - f(c)}$ for $y \neq f(c)$ and $d(f(c)) = g'(f(c))$, ensuring $d$ is continuous at $f(c)$.
- Rewrite $g(y) - g(f(c)) = d(y)(y - f(c))$ for all $y \in B$.
- Substitute $y = f(t)$ for $t \neq c$ and divide by $(t - c)$ to obtain $\frac{g(f(t)) - g(f(c))}{t - c} = d(f(t)) \frac{f(t) - f(c)}{t - c}$.
- Take the limit as $t \to c$, applying the composition theorem for continuous functions to $d(f(t))$ and the Algebraic Limit Theorem.
