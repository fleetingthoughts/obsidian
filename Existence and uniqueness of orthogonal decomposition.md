---
parent:
tags:
  - "#flashcard"
date_created: 2022-08-25
---
Prove: Let $W$ be a finite-dimensional subspace of an inner product space $V$, and let $y \in V$. Then there exist unique vectors $u \in W$ and $z \in W^\perp$ such that $y = u + z$. Furthermore, if $\{v_1, v_2, \dots, v_k\}$ is an orthonormal basis for $W$, then

$$u = \sum_{i=1}^k \langle y, v_i \rangle v_i.$$
#### Notes
- Let $\{v_1, \dots, v_k\}$ be an orthonormal basis for $W$; define $u = \sum_{i=1}^k \langle y, v_i \rangle v_i \in W$ and $z = y - u$.
- For each $j \in \{1, \dots, k\}$, compute $\langle z, v_j \rangle = \langle y, v_j \rangle - \sum_{i=1}^k \langle y, v_i \rangle \langle v_i, v_j \rangle = 0$; since $z$ is orthogonal to a basis of $W$, $z \in W^\perp$.
- For uniqueness, suppose $y = u + z = u' + z'$ with $u, u' \in W$ and $z, z' \in W^\perp$.
- Rearrange to $u - u' = z' - z \in W \cap W^\perp = \{0\}$, which forces $u = u'$ and $z = z'$.
