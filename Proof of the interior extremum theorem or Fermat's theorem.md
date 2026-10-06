---
parent: "[[Understanding Analysis - 5.2 Derivatives and the Intermediate Value Property]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch5
date_created: 2026-10-03
---
Prove: Let $f$ be differentiable on an open interval $(a, b)$. If $f$ attains a maximum value at some point $c \in (a, b)$, then $f'(c) = 0$.
#### Notes
- Construct two sequences $(x_n)$ and $(y_n)$ converging to $c$ with $x_n < c < y_n$ for all $n \in \mathbf{N}$.
- Assuming $f(c)$ is a maximum, observe $\frac{f(y_n) - f(c)}{y_n - c} \le 0$; apply the Order Limit Theorem to yield $f'(c) \le 0$.
- Observe $\frac{f(x_n) - f(c)}{x_n - c} \ge 0$; apply the Order Limit Theorem to yield $f'(c) \ge 0$.
- Combine $f'(c) \le 0$ and $f'(c) \ge 0$ to conclude $f'(c) = 0$.
