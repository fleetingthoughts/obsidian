---
parent: "[[Understanding Analysis - 6.6 Taylor Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: If $E_N(x) = f(x) - S_N(x)$ is the Taylor remainder centered at $0$, then $E_N^{(n)}(0) = 0$ for all $0 \le n \le N$.
#### Notes
Differentiating $S_N(x) = \sum_{k=0}^N \frac{f^{(k)}(0)}{k!} x^k$ yields $S_N^{(n)}(0) = f^{(n)}(0)$ for all $0 \le n \le N$. By linearity, $E_N^{(n)}(0) = f^{(n)}(0) - S_N^{(n)}(0) = 0$.
