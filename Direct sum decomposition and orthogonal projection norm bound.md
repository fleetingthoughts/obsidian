---
parent:
tags:
  - "#flashcard"
date_created: 2022-08-25
---
Prove: Let $W$ be a finite-dimensional subspace of an inner product space $V$. Then $V = W \oplus W^\perp$, and the projection $T: V \to V$ on $W$ along $W^\perp$ satisfies $N(T) = W^\perp$ and $\Vert{}T(y)\Vert{} \le \Vert{}y\Vert{}$ for all $y \in V$.
#### Notes
- By orthogonal decomposition, every $y \in V$ writes uniquely as $y = u + z$ with $u \in W$ and $z \in W^\perp$; hence $V = W + W^\perp$ and $W \cap W^\perp = \{0\}$, establishing $V = W \oplus W^\perp$.
- Define $T(y) = u$; then $T(y) = 0 \iff u = 0 \iff y = z \in W^\perp$, proving $N(T) = W^\perp$.
- Apply the Pythagorean theorem to the orthogonal vectors $u$ and $z$: $\Vert{}y\Vert{}^2 = \Vert{}u\Vert{}^2 + \Vert{}z\Vert{}^2 = \Vert{}T(y)\Vert{}^2 + \Vert{}z\Vert{}^2 \ge \Vert{}T(y)\Vert{}^2$, so $\Vert{}T(y)\Vert{} \le \Vert{}y\Vert{}$.