---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.3 Subspaces]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove the intersection of subspaces is a subspace
#### Notes
- Let $\mathcal{C}$ be a collection of subspaces and $W = \bigcap_{U \in \mathcal{C}} U$.
- Because $0 \in U$ for every subspace $U$, $0 \in W$.
- Let $x, y \in W$ and $c \in F$. This means $x, y \in U$ for all $U \in \mathcal{C}$.
- Since each $U$ is a subspace, closure guarantees $x + y \in U$ and $cx \in U$ for all $U$.
- Therefore, $x + y \in W$ and $cx \in W$, fulfilling the Subspace Criterion.
