---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.4 Invertibility and Isomorphisms]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-08-17)
---
Prove that the collection of linear transformations $\mathcal{L}(V,W)$ is isomorphic to the vector space of $M_{n \times m}(F)$ if $dim(V)=n$ and $dim(W)=m$ 
#### Notes
- Linearity: Show $\Phi_\beta^\gamma(cT + U) = [cT + U]_\beta^\gamma = c[T]_\beta^\gamma + [U]_\beta^\gamma = c\Phi_\beta^\gamma(T) + \Phi_\beta^\gamma(U)$.
    
- Surjectivity/Bijectivity: Let $A \in M_{m \times n}(F)$. Construct a transformation by mapping the basis vectors of $V$: $T(v_j) = \sum_{i=1}^m A_{ij}w_i$.
    
- Uniqueness: By the linear extension theorem, this $T$ is the unique transformation satisfying this mapping.
    
- Conclusion: By definition of matrix representation, $[T]_\beta^\gamma = A$, meaning $\Phi_\beta^\gamma$ maps exactly one transformation to every matrix.
