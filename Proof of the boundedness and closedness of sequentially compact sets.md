---
parent: "[[Understanding Analysis - 3.3 Compact Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-07-24
---
Prove that a set is compact if and only if it is closed and bounded
#### Notes
We prove boundedness and closedness separately. For boundedness:
- Assume for contradiction that $K$ is compact but is not bounded.
- Construct a sequence $(x_n) \in K$ satisfying $\vert{}x_n\vert{} > n$ for each $n \in \mathbb{N}$.
- Apply sequential compactness: $(x_n)$ must contain a convergent subsequence $(x_{n_k})$ with a limit $x \in K$.
- Observe that the subsequence terms satisfy $\vert{}x_{n_k}\vert{} > n_k \ge k$, implying the subsequence is unbounded.
- Derive a contradiction, as all convergent sequences must be bounded.

For closedness we do the following:
- Let $x$ be a limit point of $K$. Define a sequence $(x_n) \subseteq K$ converging to $x$.
- Apply sequential compactness: $(x_n)$ contains a convergent subsequence $(x_{n_k})$ with limit $y \in K$.
- Invoke subsequence convergence rules: Subsequences of a convergent sequence converge to the identical limit, forcing $y = x$.
- Conclude that since $y \in K$, it follows that $x \in K$, proving $K$ contains its limit points and is closed.