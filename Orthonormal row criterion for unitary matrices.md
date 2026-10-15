---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.2 The Gram-Schmidt Orthogonalization Process and Orthogonal Complements]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: For $A \in \mathcal{M}_{n \times n}(\mathbb{C})$, $AA^* = I$ if and only if the rows of $A$ form an orthonormal basis for $\mathbb{C}^n$.
#### Notes
Let $\rho_i$ denote the $i$-th row of $A$. Because $(AA^*)_{ij} = \sum_{k=1}^n A_{ik}\overline{A_{jk}} = \langle \rho_i, \rho_j \rangle$, $AA^* = I$ holds if and only if $\langle \rho_i, \rho_j \rangle = \delta_{ij}$.
