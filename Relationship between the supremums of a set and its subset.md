---
parent: "[[Understanding Analysis - 1.3 The Axiom of Completeness]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch1
  - stephen_abbot
  - real_analysis
date_created: 2026-07-24
---
Given a bounded set $A$ and a subset $B \subseteq A$, show that $sup(B)\leq sup(A)$.
#### Notes
et $M = \sup(A)$. By definition of supremum, $M$ is an upper bound for $A$, so $x \leq M$ for all $x \in A$. 

Since $B \subseteq A$, any element $b \in B$ must also belong to $A$, which implies $b \leq M$ for all $b \in B$. 

Thus, $M$ is an upper bound for $B$. By definition, $\sup(B)$ is the *least* upper bound of $B$. Therefore, $\sup(B) \leq M$, which means: $$\sup(B) \leq \sup(A) \quad \blacksquare$$
