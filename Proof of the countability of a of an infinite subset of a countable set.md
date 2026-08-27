---
parent: "[[Understanding Analysis - 1.5 Cardinality]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch1
date_created: 2026-07-24
---
Prove if $A$ is countable and $B\subseteq A$, then $B$ is countable as well.
#### Notes
- Assume $B$ is countable, meaning there exists a bijection $f: \mathbf{N} \to B$. Let $A \subseteq B$ be an infinite subset.
- Define the first element mapping $g(1) = f(n_1)$, where $n_1 = \min\{n \in \mathbf{N} : f(n) \in A\}$.
- Inductively define $g(k+1) = f(n_{k+1})$, where $n_{k+1} = \min\{n \in \mathbf{N} : f(n) \in A \setminus \{g(1), \dots, g(k)\}\}$.
- Conclude the constructed function $g: \mathbf{N} \to A$ is 1-1 and onto, proving $A$ is countable.
