---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: If $A$ and $B$ are simultaneously diagonalizable matrices, then $A$ and $B$ commute.
#### Notes
- By definition, there exists an invertible matrix $Q$ such that $Q^{-1} A Q = D_1$ and $Q^{-1} B Q = D_2$, where $D_1$ and $D_2$ are diagonal matrices.
    
- Isolate $A$ and $B$ to yield $A = Q D_1 Q^{-1}$ and $B = Q D_2 Q^{-1}$.
    
- Multiply the matrices: $AB = (Q D_1 Q^{-1})(Q D_2 Q^{-1}) = Q D_1 D_2 Q^{-1}$.
    
- Because diagonal matrices commute, $D_1 D_2 = D_2 D_1$.
    
- Substitute to obtain $Q D_2 D_1 Q^{-1} = (Q D_2 Q^{-1})(Q D_1 Q^{-1}) = BA$, proving commutativity.
