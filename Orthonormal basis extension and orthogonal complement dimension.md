---
parent:
tags:
  - "#flashcard"
date_created: 2022-08-25
---
Prove: Suppose $S = \{v_1, v_2, \dots, v_k\}$ is an orthonormal set in an $n$-dimensional inner product space $V$. Then: (a) $S$ can be extended to an orthonormal basis $\{v_1, v_2, \dots, v_k, v_{k+1}, \dots, v_n\}$ for $V$. (b) If $W = \text{span}(S)$, then $S_1 = \{v_{k+1}, v_{k+2}, \dots, v_n\}$ is an orthonormal basis for $W^\perp$. (c) If $W$ is any subspace of $V$, then $\dim(V) = \dim(W) + \dim(W^\perp)$.
#### Notes
- Extend the linearly independent set $S$ to an ordered basis $\{v_1, \dots, v_k, w_{k+1}, \dots, w_n\}$ for $V$.
- Apply Gram–Schmidt (which leaves $v_1, \dots, v_k$ fixed by orthogonality) and normalize the remaining $n - k$ vectors to form an orthonormal basis $\{v_1, \dots, v_n\}$ for $V$.
- Verify $S_1 = \{v_{k+1}, \dots, v_n\} \subseteq W^\perp$ by orthonormality; for any $x \in W^\perp$, expand $x = \sum_{i=1}^n \langle x, v_i \rangle v_i$ and use $\langle x, v_i \rangle = 0$ ($1 \le i \le k$) to show $S_1$ spans $W^\perp$.
- Conclude $\dim(V) = n = k + (n - k) = \dim(W) + \dim(W^\perp)$.
