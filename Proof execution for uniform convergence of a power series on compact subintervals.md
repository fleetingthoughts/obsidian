---
parent: "[[Understanding Analysis - 6.5  Power Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove if a power series $\sum_{n=0}^{\infty} a_n x^n$ converges absolutely at $x_0$, then it converges uniformly on $[-c, c]$ where $c = \vert{}x_0\vert{}$
#### Notes
Define $M_n = \vert{}a_n x_0^n\vert{} = \vert{}a_n\vert{} c^n$. Because the series converges absolutely at $x_0$, $\sum M_n$ converges. For all $x \in [-c, c]$, $\vert{}a_n x^n\vert{} \le M_n$. By the Weierstrass M-test, the series converges uniformly on $[-c, c]$.
