---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.3 Systems of Linear Equations - Theoretical Aspects]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch3
date_created: 2026-09-28
---
Prove: Let $Ax = 0$ be a homogeneous system of $m$ linear equations in $n$ unknowns over a field $F$, and let $K$ be its solution set. Then $\text{dim}(K) = n - \text{rank}(A)$
#### Notes
- Identify $K$ as the null space $N(L_A)$ of the linear transformation $L_A: F^n \to F^m$.
    
- Conclude $K$ is a subspace of $F^n$.
    
- Apply the Dimension Theorem to $L_A$: $\text{dim}(F^n) = \text{dim}(N(L_A)) + \text{dim}(R(L_A))$.
    
- Substitute known dimensions to yield $\text{dim}(K) = n - \text{rank}(L_A) = n - \text{rank}(A)$.
