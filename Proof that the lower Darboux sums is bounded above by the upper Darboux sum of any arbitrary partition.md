---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: Let $f: [a, b] \to \mathbb{R}$ be bounded. For any two partitions $P_1$ and $P_2$ of $[a, b]$, $L(f, P_1) \le U(f, P_2)$.
#### Notes
- **Common refinement construction:** Define the partition $Q = P_1 \cup P_2$ so that $P_1 \subseteq Q$ and $P_2 \subseteq Q$.
- **Lower refinement bound:** Apply the refinement inequality to $P_1 \subseteq Q$ to obtain $L(f, P_1) \le L(f, Q)$.
- **Same-partition comparison:** Use $m_k \le M_k$ on every subinterval of $Q$ to establish $L(f, Q) \le U(f, Q)$.
- **Upper refinement bound and transitivity:** Apply the refinement inequality to $P_2 \subseteq Q$ to get $U(f, Q) \le U(f, P_2)$, chaining into $L(f, P_1) \le L(f, Q) \le U(f, Q) \le U(f, P_2)$.
