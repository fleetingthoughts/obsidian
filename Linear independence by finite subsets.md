---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.5 Linear Dependence and Linear Independence]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
Characterize the linear independence of a set by its finite subsets.
#### Notes
Let $V$ be a vector space over a field and $S$ be a subset of $V$ (which may be infinite). The set $S$ is linearly independent if and only if **every finite subset of $S$ is linearly independent**.

### Rigorous proof

**Forward implication (If $S$ is linearly independent, then every finite subset is linearly independent):**

Let $S$ be a linearly independent set, and let $S'$ be an arbitrary finite subset of $S$.

Assume, for the sake of contradiction, that $S'$ is linearly dependent. This means there exists a finite linear combination of distinct vectors $v_1, v_2, \dots, v_n \in S'$ such that:

$$c_1v_1 + c_2v_2 + \dots + c_nv_n = 0$$

where not all scalars $c_i$ are zero.

Because $S'$ is a subset of $S$, all vectors $v_1, v_2, \dots, v_n$ are also elements of $S$. Therefore, this exact same equation constitutes a non-trivial linear combination of vectors in $S$ that equals the zero vector. This directly contradicts the initial premise that $S$ is linearly independent.

Thus, our assumption must be false, and every finite subset $S'$ must be linearly independent.

**Reverse implication (If every finite subset of $S$ is linearly independent, then $S$ is linearly independent):**

Assume that every finite subset of $S$ is linearly independent.

To prove $S$ is linearly independent, we must show that any finite linear combination of distinct vectors in $S$ that equals the zero vector must have all zero coefficients.

Let $v_1, v_2, \dots, v_n$ be arbitrary distinct vectors chosen from $S$, and suppose that:

$$c_1v_1 + c_2v_2 + \dots + c_nv_n = 0$$

The vectors $\{v_1, v_2, \dots, v_n\}$ form a finite subset of $S$. Let's call this subset $S'$.

By our initial premise, $S'$ is linearly independent. The definition of linear independence for a finite set dictates that the only way a linear combination of its vectors can equal the zero vector is if all the coefficients are zero. Therefore:

$$c_1 = c_2 = \dots = c_n = 0$$

Because this strictly trivial solution holds true for any arbitrary finite collection of vectors drawn from $S$, the entire set $S$ is linearly independent.