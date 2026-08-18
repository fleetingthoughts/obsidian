---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.4 Invertibility and Isomorphisms]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-08-17)
---
Prove that two vector spaces are isomorphic if and only if their dimensions are equal
#### Notes
- Forward Direction ($\implies$): Assume $V \cong W$. The isomorphism $T: V \to W$ is linear and invertible. Apply the rank-invertibility theorem to conclude $\dim(V) = \dim(W)$.
    
- Reverse Direction ($\impliedby$): Assume $\dim(V) = \dim(W) = n$. Define ordered bases $\beta = \{v_1, \dots, v_n\}$ for $V$ and $\gamma = \{w_1, \dots, w_n\}$ for $W$.
    
- Invoke the linear extension theorem to define a unique linear transformation $T$ satisfying $T(v_i) = w_i$.
    
- Show that $T(\beta) = \gamma$ spans $W$. Since $\dim(W) = n$, the $n$-element generating set $T(\beta)$ is a basis, making $T$ one-to-one and onto.
