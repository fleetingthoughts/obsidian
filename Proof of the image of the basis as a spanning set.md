---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.1 Linear Transformations, Null Spaces, and Ranges]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following. Let $T:V \to W$ be linear. If $\beta = \{v_1, v_2, \dots, v_n\}$ is a basis for $V$, then $R(T) = \text{span}(T(\beta)) = \text{span}(\{T(v_1), T(v_2), \dots, T(v_n)\})$.
#### Notes
- **Subset 1 ($\text{span}(T(\beta)) \subseteq R(T)$):** Take $w \in \text{span}(T(\beta))$, express as a linear combination $\sum a_i T(v_i)$, and pull scalars/sums inside $T$ to show it maps from a vector in $V$.
    
- **Subset 2 ($R(T) \subseteq \text{span}(T(\beta))$):** Take $w \in R(T)$ such that $w = T(v)$.
    
- **Basis Expansion:** Express $v$ as $\sum c_i v_i$ using the basis $\beta$.
    
- **Linearity Application:** Apply $T$ to the expansion and distribute to show $w$ is a linear combination of vectors in $T(\beta)$.
