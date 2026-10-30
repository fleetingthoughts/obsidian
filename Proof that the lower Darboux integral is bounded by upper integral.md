---
parent: "[[Understanding Analysis - 7.2 Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
Prove: For any bounded function $f: [a, b] \to \mathbb{R}$, $L(f) \le U(f)$.
#### Notes
- **Fix upper partition:** Fix an arbitrary partition $P_2 \in \mathcal{P}$; since $L(f, P_1) \le U(f, P_2)$ for all $P_1 \in \mathcal{P}$, $U(f, P_2)$ is an upper bound for $\{L(f, P) : P \in \mathcal{P}\}$.
- **Least upper bound step:** Take the supremum over $P_1 \in \mathcal{P}$ to deduce $L(f) \le U(f, P_2)$ for the arbitrary fixed $P_2$.
- **Greatest lower bound step:** Since $L(f)$ is a lower bound for $\{U(f, P_2) : P_2 \in \mathcal{P}\}$, take the infimum over $P_2 \in \mathcal{P}$ to conclude $L(f) \le U(f)$.
