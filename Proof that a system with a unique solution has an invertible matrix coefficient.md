---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 3.3 Systems of Linear Equations - Theoretical Aspects]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch3
date_created: 2026-09-28
---
Prove: A system of $n$ linear equations in $n$ unknowns $Ax = b$ has exactly one solution if and only if $A$ is invertible.
#### Notes
- ($\Rightarrow$) Assume $A$ is invertible. Verify $s = A^{-1}b$ is a solution: $A(A^{-1}b) = b$.
    
- Assume $As = b$. Multiply both sides by $A^{-1}$ to yield $s = A^{-1}b$, proving uniqueness.
    
- ($\Leftarrow$) Assume $Ax = b$ has a unique solution $s$.
    
- Apply the structure theorem $K = \{s\} + K_H$. Uniqueness forces $K_H = \{0\}$.
    
- Since $N(L_A) = \{0\}$, $L_A$ is injective; because $A$ is $n \times n$, $L_A$ is an isomorphism and $A$ is invertible.
