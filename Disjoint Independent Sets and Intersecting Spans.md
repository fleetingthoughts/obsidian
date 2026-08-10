---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.5 Linear Dependence and Linear Independence]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
Let $S_1$ and $S_2$ be disjoint, linearly independent subsets of a vector space $V$. State and prove the condition regarding the intersection of their spans that is equivalent to the union $S_1 \cup S_2$ being linearly independent
#### Notes
Let $V$ be a vector space, and let $S_1$ and $S_2$ be disjoint, linearly independent subsets of $V$. The union $S_1 \cup S_2$ is linearly independent if and only if the intersection of their spans is the zero subspace:

$$\text{span}(S_1) \cap \text{span}(S_2) = \{0\}$$


**Forward implication (If $S_1 \cup S_2$ is linearly independent, then $\text{span}(S_1) \cap \text{span}(S_2) = \{0\}$):**

Let $v$ be an arbitrary vector in the intersection $\text{span}(S_1) \cap \text{span}(S_2)$.

Because $v \in \text{span}(S_1)$, it can be written as a linear combination of vectors in $S_1$:

$$v = c_1x_1 + c_2x_2 + \dots + c_nx_n$$

Because $v$ is also in $\text{span}(S_2)$, it can simultaneously be written as a linear combination of vectors in $S_2$:

$$v = d_1y_1 + d_2y_2 + \dots + d_my_m$$

Setting these two expressions equal to each other gives:

$$c_1x_1 + \dots + c_nx_n = d_1y_1 + \dots + d_my_m$$

Rearranging all terms to one side yields:

$$c_1x_1 + \dots + c_nx_n - d_1y_1 - \dots - d_my_m = 0$$

Because $S_1$ and $S_2$ are given as disjoint sets ($S_1 \cap S_2 = \emptyset$), all the vectors $x_i$ and $y_j$ are distinct from one another. This equation is therefore a linear combination of distinct vectors from the union $S_1 \cup S_2$ that equals the zero vector.

Since we assumed $S_1 \cup S_2$ is linearly independent, the only solution to this equation must be the trivial one, meaning all coefficients are zero ($c_i = 0$ and $d_j = 0$).

If all coefficients are zero, then $v = 0$. Thus, the only vector in the intersection is the zero vector, proving $\text{span}(S_1) \cap \text{span}(S_2) = \{0\}$.

**Reverse implication (If $\text{span}(S_1) \cap \text{span}(S_2) = \{0\}$, then $S_1 \cup S_2$ is linearly independent):**

Assume $\text{span}(S_1) \cap \text{span}(S_2) = \{0\}$. To prove $S_1 \cup S_2$ is linearly independent, we set a linear combination of vectors from $S_1 \cup S_2$ equal to the zero vector:

$$a_1x_1 + \dots + a_kx_k + b_1y_1 + \dots + b_jy_j = 0$$

where $x_1, \dots, x_k \in S_1$ and $y_1, \dots, y_j \in S_2$.

Rearranging the terms gives:

$$a_1x_1 + \dots + a_kx_k = -(b_1y_1 + \dots + b_jy_j)$$

The left side of this equation is a vector that strictly belongs to $\text{span}(S_1)$. The right side is a vector that strictly belongs to $\text{span}(S_2)$. Since they are equal to each other, this single vector must belong to both spans, meaning it is in the intersection $\text{span}(S_1) \cap \text{span}(S_2)$.

By our assumption, the intersection only contains the zero vector. Therefore, both sides of the equation must equal zero:

$$a_1x_1 + \dots + a_kx_k = 0$$

$$b_1y_1 + \dots + b_jy_j = 0$$

Since we are given that $S_1$ is linearly independent, the first equation dictates that all $a_i = 0$.

Since we are given that $S_2$ is linearly independent, the second equation dictates that all $b_i = 0$.

Because every coefficient in the original linear combination must be zero, the union $S_1 \cup S_2$ is strictly linearly independent.