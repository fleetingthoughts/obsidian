---
parent:
tags:
  - "#flashcard"
date_created: "2026-08-17"
---
Prove that the change of coordinate matrices from $\beta$ to $\beta'$ satisfies the following:
1) It is invertible
2) $[v]_{\beta'}=Q[v]_{\beta}$
#### Notes
- Matrix Evaluation: For any $x \in V$, express the transformation evaluation as $[T(x)]_\beta = [T]_\beta [x]_\beta$.
    
- Coordinate Substitution: Substitute $\beta$-coordinates for $\beta'$-coordinates using the change of coordinate matrix: $Q[T(x)]_{\beta'} = [T]_\beta Q[x]_{\beta'}$.
    
- Algebraic Isolation: Left-multiply both sides by $Q^{-1}$ to isolate the evaluation vector: $[T(x)]_{\beta'} = Q^{-1}[T]_\beta Q[x]_{\beta'}$.
    
- Uniqueness Conclusion: Since $[T(x)]_{\beta'}$ also equals $[T]_{\beta'} [x]_{\beta'}$ for all $x$, equate the matrices to conclude $[T]_{\beta'} = Q^{-1}[T]_\beta Q$.
