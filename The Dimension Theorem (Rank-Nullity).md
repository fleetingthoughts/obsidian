---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.1 Linear Transformations, Null Spaces, and Ranges]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
State and prove the rank-nullity theorem
#### Notes
- **Basis Setup:** Let $\dim(N(T)) = k$. Take a basis $\{v_1, \dots, v_k\}$ for $N(T)$ and extend it to a basis $\beta = \{v_1, \dots, v_n\}$ for $V$.
    
- **Span Claim:** Show that the image of the extension vectors, $S = \{T(v_{k+1}), \dots, T(v_n)\}$, spans $R(T)$ by applying the Spanning Set for the Range theorem and eliminating terms mapping to $0$.
    
- **Linear Independence Setup:** Assume a linear combination of $S$ equals $0$: $\sum_{i=k+1}^n b_i T(v_i) = 0$.
    
- **Null Space Bridge:** Pull the sum inside $T$ to show $\sum_{i=k+1}^n b_i v_i \in N(T)$.
    
- **Coefficient Resolution:** Express this sum using the null space basis $\{v_1, \dots, v_k\}$, combine into a single equation equaling $0$, and invoke the linear independence of $\beta$ to conclude all $b_i = 0$. Conclude rank is $n-k$.
