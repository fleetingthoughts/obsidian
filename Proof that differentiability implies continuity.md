---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Prove: If $g : A \to \mathbf{R}$ is differentiable at a point $c \in A$, then $g$ is continuous at $c$.
#### Notes
- Write $\lim_{x \to c} (g(x) - g(c)) = \lim_{x \to c} \left( \frac{g(x) - g(c)}{x - c} \right) (x - c)$.
- Apply the Algebraic Limit Theorem for functional limits to express the product of limits as $g'(c) \cdot 0 = 0$.
- Conclude that $\lim_{x \to c} g(x) = g(c)$, establishing continuity at $c$.
