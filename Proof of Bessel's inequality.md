---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.2 The Gram-Schmidt Orthogonalization Process and Orthogonal Complements]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: Let $S = \{v_1, v_2, \dots, v_n\}$ be an orthonormal subset of an inner product space $V$. For any $x \in V$,

$$\Vert{}x\Vert{}^2 \ge \sum_{i=1}^n \vert{}\langle x, v_i \rangle\vert{}^2.$$
#### Notes
- Set $W = \text{span}(S)$ and decompose $x = u + z$ with $u = \sum_{i=1}^n \langle x, v_i \rangle v_i \in W$ and $z \in W^\perp$.
    
- Apply the Pythagorean theorem to obtain $\Vert{}x\Vert{}^2 = \Vert{}u\Vert{}^2 + \Vert{}z\Vert{}^2$.
    
- Compute $\Vert{}u\Vert{}^2 = \sum_{i=1}^n \vert{}\langle x, v_i \rangle\vert{}^2 \Vert{}v_i\Vert{}^2 = \sum_{i=1}^n \vert{}\langle x, v_i \rangle\vert{}^2$ by orthonormality of $S$.
    
- Use $\Vert{}z\Vert{}^2 \ge 0$ to conclude $\Vert{}x\Vert{}^2 = \sum_{i=1}^n \vert{}\langle x, v_i \rangle\vert{}^2 + \Vert{}z\Vert{}^2 \ge \sum_{i=1}^n \vert{}\langle x, v_i \rangle\vert{}^2$.
