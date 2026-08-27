---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.3 Compositions of Linear Transformations and Matrix Multiplication]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following: Let $T:V \to V$ be linear. If $W$ is a $T$-invariant subspace of $V$ with $\dim(W) = k$, there exists an ordered basis $\beta$ for $V$ such that $[T]_\beta$ has the block form $\begin{pmatrix} A & B \\ O & C \end{pmatrix}$, where $A$ is $k \times k$ and $O$ is the $(n-k) \times k$ zero matrix.
#### Notes
- **Basis Construction:** Choose a basis $\{v_1, \dots, v_k\}$ for $W$. Extend this to an ordered basis $\beta = \{v_1, \dots, v_k, v_{k+1}, \dots, v_n\}$ for $V$.
    
- **Evaluate Invariance:** For any $j \le k$, $v_j \in W$. Since $W$ is $T$-invariant, $T(v_j) \in W$.
    
- **Determine Coefficients:** Because $T(v_j) \in W$, it can be written strictly as a linear combination of the first $k$ basis vectors.
    
- **Matrix Structure Consequence:** For columns $1 \le j \le k$, the coefficients for $v_{k+1}, \dots, v_n$ are strictly $0$. Thus, the lower-left block of $[T]_\beta$ is the zero matrix $O$.
