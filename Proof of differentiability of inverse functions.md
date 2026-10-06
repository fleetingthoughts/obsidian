---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Prove: Let $f : [a, b] \to \mathbf{R}$ be continuous, one-to-one, and differentiable on $[a, b]$ with $f'(x) \neq 0$ for all $x \in [a, b]$. Then $f^{-1}$ is differentiable on its domain $J = f([a, b])$ with $(f^{-1})'(y) = \frac{1}{f'(x)}$ where $y = f(x)$.
#### Notes
- Write $\frac{f^{-1}(y) - f^{-1}(y_0)}{y - y_0} = \frac{x - x_0}{f(x) - f(x_0)} = \frac{1}{\frac{f(x) - f(x_0)}{x - x_0}}$ for $y = f(x)$ and $y_0 = f(x_0)$.
    
- Apply continuity of $f^{-1}$ to assert that $y \to y_0 \implies x \to x_0$.
    
- Take the limit as $y \to y_0$ using the Algebraic Limit Theorem to yield $(f^{-1})'(y_0) = \frac{1}{f'(x_0)}$.
