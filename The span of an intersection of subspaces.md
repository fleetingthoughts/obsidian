---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.4 Linear Combinations and Systems of Linear Equations]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
Given a vector space $V$ and subsets $S_1,S_2 \subseteq V$, state the relation between $span(S_1 \cap S_2)$  and the intersection of the spans and prove it.
#### Notes
For subsets $S_1, S_2 \subseteq V$, the relation between $\text{span}(S_1 \cap S_2)$ and the intersection of their spans is:
   $$\text{span}(S_1 \cap S_2) \subseteq \text{span}(S_1) \cap \text{span}(S_2)$$

Assume: Let $v \in \text{span}(S_1 \cap S_2)$.
Expand: By definition of span, $v$ can be written as a finite linear combination: $v = c_1u_1 + c_2u_2 + \dots + c_ku_k$, where each vector $u_i \in S_1 \cap S_2$.
Separate: By the definition of set intersection, every $u_i$ is an element of $S_1$, and every $u_i$ is an element of $S_2$.
Evaluate Span 1: Because $v$ is a linear combination of vectors entirely contained in $S_1$, it follows that $v \in \text{span}(S_1)$.
Evaluate Span 2: Because $v$ is a linear combination of vectors entirely contained in $S_2$, it follows that $v \in \text{span}(S_2)$.
Conclude: Since $v \in \text{span}(S_1)$ and $v \in \text{span}(S_2)$, therefore $v \in \text{span}(S_1) \cap \text{span}(S_2)$.
<!--SR:!fsrs,2026-10-19T03:07:15.475Z,18,17.65630407,5.19004872,2,3,0,0,2026-10-01T03:07:15.475Z-->

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