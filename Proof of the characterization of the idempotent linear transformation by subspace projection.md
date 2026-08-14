---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.3 Compositions of Linear Transformations and Matrix Multiplication]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following: Let $V$ be a finite-dimensional vector space and $T:V \to V$ be linear. Prove that $T^2 = T$ if and only if $T$ is a projection on $W_1 = \{y \in V : T(y) = y\}$ along $N(T)$.
#### Notes
- **Reverse Direction Setup (If Projection $\implies T^2 = T$):** If $T$ is a projection on $W_1$ along $N(T)$, any $x \in V$ can be written $x = x_1 + x_2$ where $x_1 \in W_1, x_2 \in N(T)$. $T(x) = x_1$. Then $T^2(x) = T(x_1) = x_1 = T(x)$, so $T^2 = T$.
    
- **Forward Direction Setup ($T^2 = T \implies$ Projection):** Assume $T^2 = T$. We must show $V = W_1 \oplus N(T)$.
    
- **Sum Decomposition:** For any $x \in V$, rewrite it as $x = T(x) + (x - T(x))$. Let $x_1 = T(x)$ and $x_2 = x - T(x)$.
    
- **Subspace Verification:** Observe $T(x_1) = T^2(x) = T(x) = x_1$, so $x_1 \in W_1$. Observe $T(x_2) = T(x - T(x)) = T(x) - T^2(x) = T(x) - T(x) = 0$, so $x_2 \in N(T)$. Thus $V = W_1 + N(T)$.
    
- **Direct Sum (Intersection = 0):** Let $z \in W_1 \cap N(T)$. Since $z \in W_1$, $T(z) = z$. Since $z \in N(T)$, $T(z) = 0$. Therefore $z = 0$. It is a direct sum, and $T(x) = x_1$, matching the definition of a projection.
