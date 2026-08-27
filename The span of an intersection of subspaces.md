---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.4 Linear Combinations and Systems of Linear Equations]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
Given a vector space $V$ and subsets $S_1,S_2 \subseteq V$, state the relation between $span(S_1 \cap S_2)$  and the intersection of the spans and prove it.
#### Notes
Let $V$ be a vector space over a field $F$, and let $S_1$ and $S_2$ be subsets of $V$. The relation between the span of their intersection and the intersection of their individual spans is that the span of the intersection is always a subset of the intersection of the spans:

$$\text{span}(S_1 \cap S_2) \subseteq \text{span}(S_1) \cap \text{span}(S_2)$$
Let $v$ be an arbitrary vector in $\text{span}(S_1 \cap S_2)$.

By the definition of the span, $v$ can be written as a finite linear combination of vectors strictly in the intersection $S_1 \cap S_2$. Thus, there exist vectors $u_1, u_2, \dots, u_n \in S_1 \cap S_2$ and scalars $c_1, c_2, \dots, c_n \in F$ such that:

$$v = c_1u_1 + c_2u_2 + \dots + c_nu_n$$

By the definition of set intersection, if $u_i \in S_1 \cap S_2$ for each index $i$, then it must be true that:

1. $u_i \in S_1$ for all $i = 1, \dots, n$
    
2. $u_i \in S_2$ for all $i = 1, \dots, n$
    

Because every vector $u_i$ is in $S_1$, the linear combination $c_1u_1 + c_2u_2 + \dots + c_nu_n$ is formed entirely by vectors in $S_1$. Therefore, by definition:

$$v \in \text{span}(S_1)$$

Similarly, because every vector $u_i$ is also in $S_2$, the exact same linear combination is formed entirely by vectors in $S_2$. Therefore, by definition:

$$v \in \text{span}(S_2)$$

Since the vector $v$ belongs to both $\text{span}(S_1)$ and $\text{span}(S_2)$, it must belong to their intersection:

$$v \in \text{span}(S_1) \cap \text{span}(S_2)$$

Because we chose an arbitrary vector $v \in \text{span}(S_1 \cap S_2)$ and showed it must also exist in $\text{span}(S_1) \cap \text{span}(S_2)$, it follows that:

$$\text{span}(S_1 \cap S_2) \subseteq \text{span}(S_1) \cap \text{span}(S_2)$$

_(Note: The reverse inclusion, $\text{span}(S_1) \cap \text{span}(S_2) \subseteq \text{span}(S_1 \cap S_2)$, is generally false. The two sets are only guaranteed to be equal under specific conditions, so the subset relation is the strongest general statement that can be made.)_