---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: If $(f_n)_{n=1}^\infty$ is a sequence of Riemann-integrable functions on $[a, b]$ and $f_n \to f$ uniformly on $[a, b]$, then $f$ is Riemann-integrable on $[a, b]$.
#### Notes
- **Uniform approximation:** Given $\epsilon \gt 0$, choose $N \in \mathbb{N}$ such that $\vert{}f_N(x) - f(x)\vert{} \lt \frac{\epsilon}{3(b - a)}$ for all $x \in [a, b]$, which implies $f$ is bounded.
    
- **Partition selection for $f_N$:** By the integrability of $f_N$, choose a partition $P$ of $[a, b]$ such that $U(f_N, P) - L(f_N, P) \lt \frac{\epsilon}{3}$.
    
- **Extrema perturbation bounds:** On each subinterval $[x_{k-1}, x_k]$, $f(x) \lt f_N(x) + \frac{\epsilon}{3(b - a)}$ implies $M_k(f) \le M_k(f_N) + \frac{\epsilon}{3(b - a)}$ and analogously $m_k(f) \ge m_k(f_N) - \frac{\epsilon}{3(b - a)}$.
    
- **Darboux difference estimate:** Sum over $P$ to obtain $U(f, P) - L(f, P) \le [U(f_N, P) - L(f_N, P)] + \frac{2\epsilon}{3(b - a)}\sum_{k=1}^n \Delta x_k \lt \frac{\epsilon}{3} + \frac{2\epsilon}{3} = \epsilon$.
