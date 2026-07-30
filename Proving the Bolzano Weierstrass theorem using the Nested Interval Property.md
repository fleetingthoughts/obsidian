---
parent: "[[Understanding Analysis - 2.5 Subsequences and the Bolzano-Weierstrass Theorem]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch2
date_created: 2026-07-24
---
Outline the core steps to prove the Bolzano-Weierstrass Theorem using the Nested Interval Property
#### Notes
- Let $(a_n)$ be a bounded sequence, so all terms exist within a closed interval $[-M, M]$.
- Bisect the interval; at least one half must contain an infinite number of terms of $(a_n)$. Label this interval $I_1$ and pick a term $a_{n_1} \in I_1$.
- Repeatedly bisect $I_k$ to create $I_{k+1}$, each time selecting a half with infinite terms and picking $a_{n_k}$ such that $n_k > n_{k-1}$.
- This creates a nested sequence of closed intervals $I_1 \supseteq I_2 \supseteq \dots$ whose lengths converge to zero.
- By the Nested Interval Property, there is at least one point $x$ contained in every $I_k$.
- Because the length of $I_k$ goes to zero, and both $a_{n_k}$ and $x$ are in $I_k$, the subsequence $(a_{n_k})$ converges to $x$.
