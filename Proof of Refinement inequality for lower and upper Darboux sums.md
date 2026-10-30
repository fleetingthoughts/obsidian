---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: Let $f: [a, b] \to \mathbb{R}$ be bounded and let $P, Q$ be partitions of $[a, b]$. If $P \subseteq Q$, then $L(f, P) \le L(f, Q)$ and $U(f, P) \ge U(f, Q)$.
#### Notes
- **Single-point reduction:** Adjoin one point $z \in (x_{k-1}, x_k)$ to $P$ and split the interval length as $x_k - x_{k-1} = (x_k - z) + (z - x_{k-1})$.
    
- **Subinterval infima comparison:** Define $m_k' = \inf_{x \in [z, x_k]} f(x)$ and $m_k'' = \inf_{x \in [x_{k-1}, z]} f(x)$; subset inclusion of domains yields $m_k \le m_k'$ and $m_k \le m_k''$.
    
- **Local sum inequality:** Multiply and sum to obtain $m_k(x_k - x_{k-1}) \le m_k'(x_k - z) + m_k''(z - x_{k-1})$, establishing $L(f, P) \le L(f, P \cup \{z\})$.
    
- **Induction and dualization:** Induct on the finite number of points in $Q \setminus P$ to obtain $L(f, P) \le L(f, Q)$, and apply the dual supremum inequality to establish $U(f, P) \ge U(f, Q)$.
