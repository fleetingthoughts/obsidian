---
parent: "[[Understanding Analysis - 5.3 The Mean Value Theorems]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-04
---
Prove: Let $f : [a, b] \to \mathbf{R}$ be continuous on $[a, b]$ and differentiable on $(a, b)$. If $f(a) = f(b)$, then there exists a point $c \in (a, b)$ where $f'(c) = 0$.
#### Notes
- By the Extreme value theorem, continuous $f$ on compact $[a, b]$ attains a maximum and a minimum.
- If both occur at the endpoints, $f(a) = f(b)$ implies $f$ is constant, yielding $f'(c) = 0$ for all $c \in (a, b)$.
- If either the maximum or minimum occurs at an interior point $c \in (a, b)$, apply the Interior extremum theorem to deduce $f'(c) = 0$.
