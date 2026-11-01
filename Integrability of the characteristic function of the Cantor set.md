---
parent: "[[Understanding Analysis - 7.3 Uniform Convergence and the Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: The characteristic function of the Cantor set, $\chi_C(x) = 1$ for $x \in C$ and $0$ for $x \in [0, 1] \setminus C$, is Riemann-integrable on $[0, 1]$ with $\int_0^1 \chi_C = 0$.
#### Notes
Since $C$ is closed and nowhere dense, the set of discontinuities of $\chi_C$ is exactly $C$, which has content zero, so $\chi_C$ is integrable. Because $[0, 1] \setminus C$ is dense in $[0, 1]$, $m_k = 0$ on every subinterval, giving $L(\chi_C, P) = 0$ for all $P$ and $\int_0^1 \chi_C = L(\chi_C) = 0$.