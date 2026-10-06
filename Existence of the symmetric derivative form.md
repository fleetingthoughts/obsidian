---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Prove: If $A$ is open and $g$ is differentiable at $c \in A$, then $g'(c) = \lim_{h \to 0} \frac{g(c+h) - g(c-h)}{2h}$
#### Notes
- Write $\frac{g(c+h) - g(c-h)}{2h} = \frac{1}{2} \left[ \frac{g(c+h) - g(c)}{h} + \frac{g(c-h) - g(c)}{-h} \right]$.
- Take the limit as $h \to 0$ of both terms to obtain $\frac{1}{2}[g'(c) + g'(c)] = g'(c)$.
