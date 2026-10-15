---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.2 The Gram-Schmidt Orthogonalization Process and Orthogonal Complements]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: Let $W$ be a finite-dimensional subspace of an inner product space $V$, let $y \in V$, and let $u \in W$ be the orthogonal projection of $y$ on $W$. Then for any $x \in W$, $\Vert{}y - x\Vert{} \ge \Vert{}y - u\Vert{}$, with equality if and only if $x = u$.
#### Notes
- Decompose $y = u + z$ with $u \in W$ and $z = y - u \in W^\perp$; for any $x \in W$, write $y - x = (u - x) + z$.
- Note $u - x \in W$ and $z \in W^\perp$, so $(u - x) \perp z$; apply the Pythagorean theorem to obtain $\Vert{}y - x\Vert{}^2 = \Vert{}u - x\Vert{}^2 + \Vert{}z\Vert{}^2$.
- Substitute $z = y - u$ to conclude $\Vert{}y - x\Vert{}^2 = \Vert{}u - x\Vert{}^2 + \Vert{}y - u\Vert{}^2 \ge \Vert{}y - u\Vert{}^2$.
- Deduce that equality holds if and only if $\Vert{}u - x\Vert{}^2 = 0$, which is equivalent to $x = u$.
