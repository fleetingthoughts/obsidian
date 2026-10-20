---
parent: "[[Understanding Analysis - 2.5 Subsequences and the Bolzano-Weierstrass Theorem]]"
tags:
  - "#flashcard"
  - math
  - stephen_abbot
  - micro/math/abbott/ch2
date_created: 2026-07-24
---
Given a sequence $(a_n)$, what propositions solely about its subsequences are sufficient  for the divergence or convergence of $(a_n)$.
#### Notes
## 1. Propositions Sufficient for Convergence

* **Universal Subsequential Convergence:** A sequence $(a_n)$ converges to a limit $L$ if and only if **every** subsequence of $(a_n)$ converges to $L$.
* **Even and Odd Subsequences:** If both the subsequence of even-indexed terms ($a_{2k}$) and the subsequence of odd-indexed terms ($a_{2k-1}$) converge to the *same* limit $L$, then the full sequence $(a_n)$ converges to $L$.
* **Finite Partition of Subsequences:** If the set of natural numbers $\mathbb{N}$ can be partitioned into a finite number of disjoint subsets, each generating a subsequence that converges to the exact same limit $L$, then $(a_n)$ converges to $L$.
* **Boundedness and a Unique Subsequential Limit:** If a sequence $(a_n)$ is bounded and all of its convergent subsequences converge to the same unique limit $L$, then $(a_n)$ converges to $L$.

---

### 2. Propositions Sufficient for Divergence

* **Conflicting Subsequential Limits:** If $(a_n)$ has at least two subsequences that converge to *different* limits ($L_1 \neq L_2$), then the sequence $(a_n)$ diverges. (For example, alternating signs where even and odd terms converge to $1$ and $-1$).
* **Unbounded Subsequence:** If $(a_n)$ contains even a single subsequence that is unbounded (or diverges to $\pm\infty$), then $(a_n)$ cannot converge as a real sequence.
* **Multiple Subsequential Limits:** If the set of all subsequential limits contains more than one element, the sequence diverges.
<!--SR:!fsrs,2026-10-28T22:48:39.694Z,8,8.2956,1,2,1,0,0,2026-10-20T22:48:39.694Z-->

