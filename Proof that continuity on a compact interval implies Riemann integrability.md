---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: If $f: [a, b] \to \mathbb{R}$ is continuous on $[a, b]$, then $f$ is Riemann-integrable on $[a, b]$.
#### Notes
- **Uniform continuity:** Compactness of $[a, b]$ ensures $f$ is bounded and uniformly continuous; given $\epsilon \gt 0$, choose $\delta \gt 0$ such that $\vert{}x - y\vert{} \lt \delta \implies \vert{}f(x) - f(y)\vert{} \lt \frac{\epsilon}{b - a}$.
    
- **Mesh control:** Select a partition $P = \{x_0, x_1, \dots, x_n\}$ of $[a, b]$ with $\Delta x_k = x_k - x_{k-1} \lt \delta$ for all $k$.
    
- **Subinterval oscillation bound:** By the extreme value theorem on $[x_{k-1}, x_k]$, $f$ attains its supremum $M_k = f(z_k)$ and infimum $m_k = f(y_k)$ at points satisfying $\vert{}z_k - y_k\vert{} \le \Delta x_k \lt \delta$, forcing $M_k - m_k \lt \frac{\epsilon}{b - a}$.
    
- **Telescoping Darboux gap:** Sum over $P$ to obtain $U(f, P) - L(f, P) = \sum_{k=1}^n (M_k - m_k)\Delta x_k \lt \frac{\epsilon}{b - a}\sum_{k=1}^n \Delta x_k = \epsilon$, fulfilling the Darboux integrability criterion.
