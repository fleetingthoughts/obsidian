---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.3 Subspaces]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove that given a subset $S \subseteq V$, $span(S)$ is the smallest subspace containing $S$.
#### Notes
- Handle the trivial case: if $S = \emptyset$, $\text{span}(\emptyset) = \{0\}$, which is trivially a subspace.
- If $S \neq \emptyset$, pick $u \in S$. Compute $0u = 0$, so $0 \in \text{span}(S)$.
- Take $x, y \in \text{span}(S)$. Write both as finite linear combinations of vectors in $S$.
- Compute $x + y$ and $cx$. Group terms to show both results are also finite linear combinations of vectors in $S$. Thus, $\text{span}(S)$ is a subspace.
- Any $v \in S$ can be written as $1v \in \text{span}(S)$, so $S \subseteq \text{span}(S)$.
- Let $W$ be any subspace containing $S$. Because $W$ is closed under addition and scalar multiplication, any linear combination of elements in $S$ must be in $W$, forcing $\text{span}(S) \subseteq W$.
