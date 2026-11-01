---
parent: "[[Understanding Analysis - 7.3 Uniform Convergence and the Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: If $f : [a, b] \to \mathbf{R}$ is bounded on $[a, b]$ and Riemann-integrable on $[c, b]$ for every $c \in (a, b)$, then $f$ is Riemann-integrable on $[a, b]$.
#### Notes
- Since $f$ is bounded on $[a, b]$, choose $M \gt 0$ such that $\vert{}f(x)\vert{} \le M$ for all $x \in [a, b]$, which implies $M_k - m_k \le 2M$ on any subinterval.
    
- Given $\epsilon \gt 0$, choose $x_1 \in (a, b)$ close to $a$ such that $x_1 - a \lt \frac{\epsilon}{4M}$, ensuring $(M_1 - m_1)(x_1 - a) \le 2M(x_1 - a) \lt \frac{\epsilon}{2}$.
    
- Since $f$ is integrable on $[x_1, b]$, choose a partition $P_1$ of $[x_1, b]$ such that $U(f, P_1) - L(f, P_1) \lt \frac{\epsilon}{2}$.
    
- Define the partition $P = \{a\} \cup P_1$ of $[a, b]$ and combine the bounds:
    
    $$U(f, P) - L(f, P) = (M_1 - m_1)(x_1 - a) + [U(f, P_1) - L(f, P_1)] \lt \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon$$
