---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: If $f: [a, b] \to \mathbb{R}$ is monotone increasing on $[a, b]$, then $f$ is Riemann-integrable on $[a, b]$.
#### Notes
- **Uniform partition construction:** Assume $f(a) \lt f(b)$ (otherwise $f$ is constant) and let $P_n$ be the uniform partition of $[a, b]$ with $\Delta x_k = \frac{b - a}{n}$.
    
- **Endpoint extrema:** Monotonicity implies $m_k = f(x_{k-1})$ and $M_k = f(x_k)$ on every subinterval $[x_{k-1}, x_k]$.
    
- **Telescoping sum:** Compute $U(f, P_n) - L(f, P_n) = \frac{b - a}{n}\sum_{k=1}^n [f(x_k) - f(x_{k-1})] = \frac{b - a}{n}[f(b) - f(a)]$.
    
- **Archimedean choice:** Given $\epsilon \gt 0$, choose $n \in \mathbb{N}$ with $n \gt \frac{(b - a)[f(b) - f(a)]}{\epsilon}$ so that $U(f, P_n) - L(f, P_n) \lt \epsilon$.
