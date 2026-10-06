---
parent: "[[Understanding Analysis - 5.3 The Mean Value Theorems]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-04
---
Prove: If $g : A \to \mathbf{R}$ is differentiable on an interval $A$ and satisfies $g'(x) = 0$ for all $x \in A$, then $g(x) = k$ for some constant $k \in \mathbf{R}$.
#### Notes
- Choose arbitrary points $x, y \in A$ with $x < y$.
- Apply the Mean value theorem to $g$ on $[x, y]$ to find $c \in (x, y)$ such that $\frac{g(y) - g(x)}{y - x} = g'(c)$.
- Since $g'(c) = 0$, conclude $g(y) = g(x)$ for all $x, y \in A$, establishing $g(x) = k$.
