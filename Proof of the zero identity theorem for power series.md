---
parent: "[[Understanding Analysis - 6.5  Power Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove if $g(x) = \sum_{n=0}^{\infty} b_n x^n$ converges on $(-R, R)$ and there exists a sequence $x_n \to 0$ with $x_n \neq 0$ such that $g(x_n) = 0$ for all $n$, then $b_n = 0$ for all $n \ge 0$
#### Notes
- Use continuity of $g$ at zero to establish $b_0 = g(0) = \lim g(x_n) = 0$.
- Proceed by induction, assuming $b_0 = \dots = b_{k-1} = 0$, and factor $g(x) = x^k h(x)$ where $h(x) = \sum_{m=0}^{\infty} b_{k+m} x^m$.
- Acknowledge that since $g(x_n) = 0$ and $x_n \neq 0$, the equation forces $h(x_n) = 0$.
- Use continuity of $h$ at zero to deduce $b_k = h(0) = \lim h(x_n) = 0$, completing the induction.
