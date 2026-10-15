---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.2 The Gram-Schmidt Orthogonalization Process and Orthogonal Complements]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: Let $\beta$ be a basis for a subspace $W$ of an inner product space $V$. A vector $z \in V$ lies in $W^\perp$ if and only if $\langle z, v \rangle = 0$ for all $v \in \beta$.
#### Notes
Necessity holds because $\beta \subseteq W$. Conversely, any $w \in W$ is a finite linear combination $w = \sum_{i=1}^m c_i v_i$ with $v_i \in \beta$, so $\langle z, w \rangle = \sum_{i=1}^m \overline{c_i} \langle z, v_i \rangle = 0$.
