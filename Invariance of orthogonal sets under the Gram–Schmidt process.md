---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.2 The Gram-Schmidt Orthogonalization Process and Orthogonal Complements]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $\{w_1, w_2, \dots, w_n\}$ is an orthogonal set of nonzero vectors in an inner product space, then the vectors $v_1, v_2, \dots, v_n$ produced by the Gram–Schmidt process satisfy $v_k = w_k$ for $1 \le k \le n$.
#### Notes
By induction: $v_1 = w_1$; if $v_j = w_j$ for all $j \lt k$, then $\langle w_k, v_j \rangle = \langle w_k, w_j \rangle = 0$, so $v_k = w_k - \sum_{j=1}^{k-1} \frac{\langle w_k, v_j \rangle}{\Vert{}v_j\Vert{}^2} v_j = w_k$.
