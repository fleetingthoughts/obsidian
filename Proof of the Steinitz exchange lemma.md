---
tags:
  - linear_algebra
  - proof
  - math
date_created: 2026-02-28
---
The proof is by induction. We are given the following:
1) A vector space $V$
- A generating set $G$ containing $n$ vectors
- A linearly independent subset $L \subseteq V$ that contains $m$ vectors $L = \{v_1,...v_m\}$ 
- The inductive hypothesis. Assuming if $L'$ contains $m$ vectors and there is some $H'\subseteq G$ that contains $n-m$ vectors such that $L' \cup H$ generates $V$
- $L$ has $m+1$ vectors, show there there is a $H \subseteq G$ containing $n-(m+1)$ vectors such that $L\cup H$ generates $V$

Then the goal for the proof by induction is to prove the following two things:
- Prove the base case where $L$ contains no vector and is the null set is true
- Show there there is a $H \subseteq G$ containing $n-(m+1)$ vectors such that $L\cup H$ generates $V$

Some facts we will use:
1) Arbitrarily construct from the given $L' =\{v_1,..v_m\}$
2) Arbitrarily construct from the given $H' =\{u_1,...u_{n-m}\}$
3) Arbitrarily construct from the given $L = \{v_1,...,v_{m+1}\}=L'\cup\{v_{m+1}\}$
4) By 3), $L' \subseteq L$ 
5) The additional vector $v_{m+1}\in span\{L'\cup H'\}$ := by $L'\cup H' = V$
6) By 4) and the assumption $L' \cup H'$ generates $V$, the union of $L$ and $H'$ also spans the vector space: $span \{L\cup H'\}=V$ 
7) By 4), since $v_{m+1}$ can be expressed as a linear combination of $L' \cup H'$ so $L\cup H'$ is a linearly dependent set and we can express one of the $u_i$ as a linear combination of the others
8) Construct $H\subseteq H'$ by removing one of those $u_i$ so that it has $n-m-1$ vectors
9) By 7), there is some $(L'\cup H')\subseteq span(L\cup H)$ with the same span by removing one of the $u_i$
10) By [Theorem 1.5](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.5%20Linear%20Dependence%20and%20Linear%20Independence.md), the span is a subspace, and any subspace that contains a set of vectors contains its span. 
11) By assumption, $span(L'\cup H')= V$ then we have proven for $L$ containing $m+1$ vectors,  $L\cup H$ can generate the vector space with $H \subseteq H'\subseteq G$  containing $n-m-1$ vectors 
