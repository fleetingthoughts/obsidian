---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $V$ is a finite-dimensional inner product space, $\beta = \{v_1, \dots, v_n\}$ is an orthonormal basis for $V$, and $T$ is a linear operator on $V$, then $[T^*]_\beta = ([T]_\beta)^*$.
#### Notes
- Let $A = [T]_\beta$ and $B = [T^*]_\beta$.
- Because $\beta$ is an orthonormal basis, the entries of $A$ and $B$ are given by the Fourier coefficients:
    $$A_{ji} = \langle T(v_i), v_j \rangle \quad \text{and} \quad B_{ij} = \langle T^*(v_j), v_i \rangle$$
- Apply conjugate symmetry and the defining property of the adjoint to $B_{ij}$:$$\begin{aligned} B_{ij} &= \langle T^*(v_j), v_i \rangle \\ &= \overline{\langle v_i, T^*(v_j) \rangle} \\ &= \overline{\langle T(v_i), v_j \rangle} \end{aligned}$$
- Substitute $A_{ji} = \langle T(v_i), v_j \rangle$ to obtain $B_{ij} = \overline{A_{ji}} = (A^*)_{ij}$ for all $i, j$, proving $[T^*]_\beta = ([T]_\beta)^*$.
