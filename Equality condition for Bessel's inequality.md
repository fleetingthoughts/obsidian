---
parent:
tags:
  - "#flashcard"
date_created: 2022-08-25
---
Prove: Let $S = \{v_1, v_2, \dots, v_n\}$ be an orthonormal subset of an inner product space $V$. For $x \in V$, $\Vert{}x\Vert{}^2 = \sum_{i=1}^n \vert{}\langle x, v_i \rangle\vert{}^2$ if and only if $x \in \text{span}(S)$.
#### Notes
Decompose $x = u + z$ with $u = \sum_{i=1}^n \langle x, v_i \rangle v_i \in \text{span}(S)$ and $z \in \text{span}(S)^\perp$. By the Pythagorean theorem, $\Vert{}x\Vert{}^2 = \sum_{i=1}^n \vert{}\langle x, v_i \rangle\vert{}^2 + \Vert{}z\Vert{}^2$, so equality holds if and only if $z = 0$, i.e., $x = u \in \text{span}(S)$.
