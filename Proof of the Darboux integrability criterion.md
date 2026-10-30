---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: A bounded function $f: [a, b] \to \mathbb{R}$ is Riemann-integrable on $[a, b]$ if and only if for every $\epsilon \gt 0$ there exists a partition $P_\epsilon$ of $[a, b]$ such that $U(f, P_\epsilon) - L(f, P_\epsilon) \lt \epsilon$.
#### Notes
- **Sufficiency ($\impliedby$):** Given $\epsilon \gt 0$ and $P_\epsilon$, bound $0 \le U(f) - L(f) \le U(f, P_\epsilon) - L(f, P_\epsilon) \lt \epsilon$; since $\epsilon \gt 0$ is arbitrary, $U(f) = L(f)$.
    
- **Approximation by infimum and supremum ($\implies$):** Assume $U(f) = L(f)$ and let $\epsilon \gt 0$; choose partitions $P_1, P_2$ such that $U(f, P_1) \lt U(f) + \epsilon/2$ and $L(f, P_2) \gt L(f) - \epsilon/2$.
    
- **Common refinement pivot:** Form $P_\epsilon = P_1 \cup P_2$ so that $U(f, P_\epsilon) \le U(f, P_1)$ and $L(f, P_\epsilon) \ge L(f, P_2)$.
    
- **Difference estimate:** Subtract the bounds to obtain $U(f, P_\epsilon) - L(f, P_\epsilon) \le U(f, P_1) - L(f, P_2) \lt (U(f) + \epsilon/2) - (L(f) - \epsilon/2) = \epsilon$.
