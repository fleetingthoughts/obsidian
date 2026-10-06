---
parent: "[[Understanding Analysis - 5.3 The Mean Value Theorems]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-04
---
Prove: If $f : [a, b] \to \mathbf{R}$ is continuous on $[a, b]$ and differentiable on $(a, b)$, then there exists a point $c \in (a, b)$ where $f'(c) = \frac{f(b) - f(a)}{b - a}$.
#### Notes
- Define $d(x) = f(x) - \left[ \left(\frac{f(b) - f(a)}{b - a}\right)(x - a) + f(a) \right]$ as the vertical difference between $f(x)$ and the secant line.
- Observe $d$ is continuous on $[a, b]$, differentiable on $(a, b)$, and satisfies $d(a) = 0 = d(b)$.
- Apply Rolle's theorem to $d$ to obtain $c \in (a, b)$ where $d'(c) = 0$.
- Differentiate $d(x)$ to conclude $f'(c) - \frac{f(b) - f(a)}{b - a} = 0$.
