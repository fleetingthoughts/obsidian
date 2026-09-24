---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.4 Invertibility and Isomorphisms]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch2
date_created: 2026-09-23
---
Let $V$ and $W$ be finite-dimensional vector spaces and $T: V \to W$ be an isomorphism, and let $V_0$ be a subspace of $V$. Then $T(V_0)$ is a subspace of $W$, and $\dim(V_0) = \dim(T(V_0))$
#### Notes
- Verify $T(V_0)$ is a subspace by showing it contains the zero vector and is closed under addition and scalar multiplication using the linearity of $T$.
- Select a basis $\beta$ for $V_0$ and demonstrate that the image $T(\beta)$ spans $T(V_0)$.
- Apply the injectivity of the isomorphism $T$ to establish that $T(\beta)$ is linearly independent.
- Conclude that $T(\beta)$ is a basis for $T(V_0)$, which yields $\dim(V_0) = \dim(T(V_0))$
