---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.1 Linear Transformations, Null Spaces, and Ranges]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following. Let $V$ and $W$ be vector spaces, and let $T:V \to W$ be linear. Then $T$ is one-to-one if and only if $N(T) = \{0\}$.
#### Notes
- **Forward Direction:** Assume $T$ is one-to-one. Let $x \in N(T)$. Since $T(x) = 0$ and $T(0) = 0$, $x = 0$ by injectivity. Thus $N(T) = \{0\}$.
    
- **Reverse Direction Setup:** Assume $N(T) = \{0\}$. Suppose $T(x) = T(y)$.
    
- **Linearity Application:** Re-arrange to $T(x) - T(y) = 0$, then apply linearity to get $T(x-y) = 0$.
    
- **Conclusion:** This implies $x-y \in N(T)$. Since $N(T) = \{0\}$, $x-y = 0 \implies x=y$.
