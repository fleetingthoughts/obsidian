---
parent: "[[Understanding Analysis - 3.3 Compact Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-07-24
---
Prove the nested interval property of compact sets.
#### Notes
- Construct a sequence by selecting $x_n \in K_n$ for each $n \in \mathbb{N}$.
- Due to nesting, the entire sequence $(x_n)$ is contained in $K_1$.
- Apply compactness of $K_1$: $(x_n)$ has a convergent subsequence $(x_{n_k})$ whose limit $x$ belongs to $K_1$.
- Fix an arbitrary $n_0 \in \mathbb{N}$. For indices $n_k \ge n_0$, the terms $x_{n_k}$ are fully contained in $K_{n_0}$.
- Use the closedness of $K_{n_0}$ to conclude the limit $x$ belongs to $K_{n_0}$ for all $n$, guaranteeing $\bigcap_{n=1}^\infty K_n$ is nonempty.
