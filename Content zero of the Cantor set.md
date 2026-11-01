---
parent: "[[Understanding Analysis - 7.3 Uniform Convergence and the Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: The Cantor set $C \subseteq [0, 1]$ has content zero.
#### Notes
At stage $n$, $C \subseteq C_n$, where $C_n$ is a union of $2^n$ disjoint closed intervals of length $3^{-n}$. Given $\epsilon \gt 0$, choose $n$ such that $\left(\frac{2}{3}\right)^n \lt \frac{\epsilon}{2}$, and enclose each closed interval of $C_n$ in an open interval of length $3^{-n} + \frac{\epsilon}{2^{n+1}}$, yielding a finite open cover of total length $\left(\frac{2}{3}\right)^n + \frac{\epsilon}{2} \lt \epsilon$.
