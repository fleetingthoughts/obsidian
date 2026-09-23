---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.6 Bases and Dimension]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove that the basis of a vector space has a unique number of vectors.
#### Notes
Let $\beta$ be a finite basis for $V$ containing $n$ vectors, and let $\gamma$ be any other basis for $V$.
1. Finiteness of $\gamma$Show by contradiction that $\gamma$ cannot contain more than $n$ vectors. If $\gamma$ contained more than $n$ vectors, we could select a subset $S \subseteq \gamma$ of $n+1$ vectors. Since $S$ is linearly independent and $\beta$ generates $V$, the Replacement Theorem would force $n+1 \le n$, which is a contradiction. Thus, $\gamma$ must be finite, containing some integer $m$ vectors.

2. Upper Bound ($m \le n$)Since $\gamma$ is a linearly independent set with $m$ vectors and $\beta$ is a generating set with $n$ vectors, the Replacement Theorem implies $m \le n$.

3. Lower Bound ($n \le m$)Reversing the roles, since $\beta$ is a linearly independent set with $n$ vectors and $\gamma$ is a generating set with $m$ vectors, the Replacement Theorem implies $n \le m$.
4. Conclusion: Since $m \le n$ and $n \le m$, it follows that $m = n$, proving that the number of vectors in any basis is unique.
<!--SR:!fsrs,2026-11-04T15:24:19.691Z,42,41.57871783,1,2,2,0,0,2026-09-23T15:24:19.691Z-->
