---
parent: "[[Understanding Analysis - 6.4  Series of Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove: Let $f_n$ be continuous functions defined on a set $A \subseteq \mathbf{R}$, and assume $\sum_{n=1}^{\infty} f_n$ converges uniformly on $A$ to a function $f$. Then, $f$ is continuous on $A$.
#### Notes
- Define the sequence of partial sums $s_k(x) = \sum_{n=1}^k f_n(x)$.
- Note that $s_k$ is continuous on $A$ for every $k \in \mathbf{N}$ by the algebraic continuity theorem for finite sums.
- Apply the continuous limit theorem to the sequence of continuous functions $(s_k)$.
- Conclude that since $(s_k)$ converges uniformly to $f$ on $A$, the limit function $f$ is continuous on $A$.
