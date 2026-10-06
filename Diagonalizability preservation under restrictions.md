---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.4 Invariant Subspaces and the Cayley-Hamilton Theorem]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-10-04
---
Prove: The restriction $T_W$ of a diagonalizable linear operator $T$ to any nontrivial $T$-invariant subspace $W$ is diagonalizable.
#### Notes
- Express $V = \bigoplus_{i=1}^k E_{\lambda_i}$ using the eigenspaces of the diagonalizable operator $T$.
    
- For any $w \in W$, write $w = v_1 + \dots + v_k$ where $v_i \in E_{\lambda_i}$.
    
- Use eigenvector decomposition properties within invariant subspaces to deduce that each component $v_i$ must reside in $W$.
    
- Conclude $W = \bigoplus_{i=1}^k (W \cap E_{\lambda_i})$, satisfying the direct sum condition of 1-dimensional invariant subspaces for the diagonalizability of $T_W$.
