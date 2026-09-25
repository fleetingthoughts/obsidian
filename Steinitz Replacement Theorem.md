---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.6 Bases and Dimension]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
State the Steinitz Replacement Theorem
#### Notes
Let $V$ be a vector space over a field $F$. Let $U = \{u_1, u_2, \dots, u_m\}$ be a finite set of linearly independent vectors in $V$. Let $W = \{w_1, w_2, \dots, w_n\}$ be a finite set of vectors that spans $V$.
1. $m \le n$
2. The vectors in $W$ can be reordered such that the set $\{u_1, \dots, u_m, w_{m+1}, \dots, w_n\}$ also spans $V$.
<!--SR:!fsrs,2026-10-03T22:49:48.608Z,8,8.2956,1,2,1,0,0,2026-09-25T22:49:48.608Z-->

Equivalently, there exists a subset $W' \subseteq W$ of size $n - m$ such that their union spans the vector space:

$$\text{span}(U \cup W') = V$$
