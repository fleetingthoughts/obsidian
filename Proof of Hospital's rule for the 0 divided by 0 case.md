---
parent: "[[Understanding Analysis - 5.3 The Mean Value Theorems]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-04
---
Prove: Let $f$ and $g$ be continuous on an interval containing $a$, and differentiable except possibly at $a$. If $f(a) = g(a) = 0$, $g'(x) \ne 0$ for $x \ne a$, and $\lim_{x \to a} \frac{f'(x)}{g'(x)} = L$, then $\lim_{x \to a} \frac{f(x)}{g(x)} = L$.
#### Notes
- Apply the Generalized mean value theorem to $f$ and $g$ on $[a, x]$ to write $\frac{f(x)}{g(x)} = \frac{f(x) - f(a)}{g(x) - g(a)} = \frac{f'(c_x)}{g'(c_x)}$ for some $c_x \in (a, x)$.
- Observe that as $x \to a$, the intermediate point $c_x \to a$ by the Squeeze theorem.
- Take the limit as $x \to a$ to yield $\lim_{x \to a} \frac{f(x)}{g(x)} = \lim_{c_x \to a} \frac{f'(c_x)}{g'(c_x)} = L$.
