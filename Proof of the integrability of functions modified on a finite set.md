---
parent: "[[Understanding Analysis - 7.3 Uniform Convergence and the Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: If $f : [a, b] \to \mathbf{R}$ is Riemann-integrable and $g : [a, b] \to \mathbf{R}$ satisfies $g(x) = f(x)$ for all but finitely many points in $[a, b]$, then $g$ is Riemann-integrable and $\int_a^b g = \int_a^b f$.
#### Notes
- By induction, it suffices to prove the case where $g$ differs from $f$ at a single point $z \in [a, b]$; define $h(x) = g(x) - f(x)$ and let $K = \vert{}g(z) - f(z)\vert{} \gt 0$.
    
- Given $\epsilon \gt 0$, choose a partition $P_1$ of $[a, b]$ such that $U(f, P_1) - L(f, P_1) \lt \frac{\epsilon}{2}$.
    
- Refine $P_1$ to $P_\epsilon$ by adding points around $z$ so that $z$ belongs to at most two subintervals of $P_\epsilon$, each of length less than $\frac{\epsilon}{8K}$.
    
- Compare the Darboux sums of $g$ and $f$ on $P_\epsilon$: on subintervals not containing $z$, $M_k(g) = M_k(f)$ and $m_k(g) = m_k(f)$, while on the at most two subintervals containing $z$, $\vert{}M_k(g) - M_k(f)\vert{} \le K$ and $\vert{}m_k(g) - m_k(f)\vert{} \le K$, yielding:
    
    $$\vert{}U(g, P_\epsilon) - U(f, P_\epsilon)\vert{} \lt \frac{\epsilon}{4}, \quad \vert{}L(g, P_\epsilon) - L(f, P_\epsilon)\vert{} \lt \frac{\epsilon}{4}$$
    
- Apply the triangle inequality to obtain $U(g, P_\epsilon) - L(g, P_\epsilon) \lt [U(f, P_\epsilon) - L(f, P_\epsilon)] + \frac{\epsilon}{2} \lt \epsilon$, and take $\epsilon \to 0$ to conclude $\int_a^b g = \int_a^b f$.
