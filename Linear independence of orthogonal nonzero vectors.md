---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.2 The Gram-Schmidt Orthogonalization Process and Orthogonal Complements]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $S = \{v_1, v_2, \dots, v_k\}$ is an orthogonal subset of nonzero vectors in an inner product space $V$, then $S$ is linearly independent.
#### Notes
Suppose $\sum_{i=1}^k a_i v_i = 0$. For each $j$, $0 = \left\langle \sum_{i=1}^k a_i v_i, v_j \right\rangle = a_j \Vert{}v_j\Vert{}^2$; since $v_j \neq 0$, $\Vert{}v_j\Vert{}^2 \neq 0$, so $a_j = 0$.
