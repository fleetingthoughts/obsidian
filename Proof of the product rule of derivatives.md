---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Let $f$ and $g$ be functions defined on an interval $A$. If both are differentiable at $c \in A$, then $(fg)'(c) = f'(c)g(c) + f(c)g'(c)$.
#### Notes
- Express the difference quotient $\frac{(fg)(x) - (fg)(c)}{x - c}$ as $f(x) \left[ \frac{g(x) - g(c)}{x - c} \right] + g(c) \left[ \frac{f(x) - f(c)}{x - c} \right]$.
- Use differentiability of $f$ at $c$ to establish continuity at $c$, yielding $\lim_{x \to c} f(x) = f(c)$.
- Apply the Algebraic Limit Theorem for functional limits to evaluate the limit as $x \to c$.