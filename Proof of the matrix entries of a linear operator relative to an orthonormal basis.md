---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.2 The Gram-Schmidt Orthogonalization Process and Orthogonal Complements]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $\beta = \{v_1, v_2, \dots, v_n\}$ is an orthonormal basis for an inner product space $V$ and $T$ is a linear operator on $V$, then $([T]_\beta)_{ij} = \langle T(v_j), v_i \rangle$.
#### Notes
Expanding $T(v_j)$ in the orthonormal basis $\beta$ yields $T(v_j) = \sum_{i=1}^n \langle T(v_j), v_i \rangle v_i$. By definition of $[T]_\beta$, the coefficient of $v_i$ is $([T]_\beta)_{ij}$.
