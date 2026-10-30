---
parent: "[[Understanding Analysis - 6.5  Power Series]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch6
date_created: 2022-08-25
---
Prove that for any sequence $(b_n)$ satisfying $b_1 \ge b_2 \ge \dots \ge 0$, and any series $\sum_{n=1}^{\infty} a_n$ with partial sums bounded by $A$, the inequality $\vert{}\sum_{k=1}^n a_k b_k\vert{} \le A b_1$ holds
#### Notes
- Define partial sums $s_n = a_1 + \dots + a_n$ and apply summation-by-parts to rewrite $\sum_{k=1}^n a_k b_k = s_n b_{n+1} + \sum_{k=1}^n s_k (b_k - b_{k+1})$.
- Apply the triangle inequality and bound each $\vert{}s_k\vert{}$ by $A$.
- Factor out $A$ and use the assumption $b_k - b_{k+1} \ge 0$ to resolve the telescoping sum $\sum_{k=1}^n (b_k - b_{k+1})$.
- Conclude the bound simplifies to $A b_{n+1} + A (b_1 - b_{n+1}) = A b_1$.
