---
parent: "[[Understanding Analysis - 6.5  Power Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove if $\sum_{n=0}^{\infty} a_n x^n = \sum_{n=0}^{\infty} b_n x^n$ for all $x \in (-R, R)$, then $a_n = b_n$ for all $n \ge 0$
#### Notes
Let $f(x)$ and $g(x)$ represent the two series. They are infinitely differentiable on $(-R, R)$ and equal everywhere, so their derivatives match. Evaluating at $x = 0$ gives $n! a_n = f^{(n)}(0) = g^{(n)}(0) = n! b_n$, which implies $a_n = b_n$.
