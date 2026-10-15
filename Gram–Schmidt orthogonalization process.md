---
parent:
tags:
  - "#flashcard"
date_created: 2022-08-25
---
Prove: Let $V$ be an inner product space and $S = \{w_1, w_2, \dots, w_n\}$ be a linearly independent subset of $V$. Define $S' = \{v_1, v_2, \dots, v_n\}$ by $v_1 = w_1$ and $$v_k = w_k - \sum_{j=1}^{k-1} \frac{\langle w_k, v_j \rangle}{\Vert{}v_j\Vert{}^2} v_j \quad \text{for } 2 \le k \le n.$$

Then $S'$ is an orthogonal set of nonzero vectors such that $\text{span}(S') = \text{span}(S)$
#### Notes
- Induct on $n$. For $n = 1$, $v_1 = w_1 \neq 0$ by linear independence of $S$, and $\text{span}(S') = \text{span}(S)$.
    
- Assume $S_{k-1}' = \{v_1, \dots, v_{k-1}\}$ is an orthogonal set of nonzero vectors with $\text{span}(S_{k-1}') = \text{span}(S_{k-1})$.
    
- If $v_k = 0$, then $w_k \in \text{span}(S_{k-1}') = \text{span}(S_{k-1})$, contradicting linear independence of $S$; thus $v_k \neq 0$.
    
- For $1 \le i \lt k$, take the inner product $\langle v_k, v_i \rangle$ and use the inductive orthogonality $\langle v_j, v_i \rangle = 0$ ($j \neq i$) to obtain $\langle v_k, v_i \rangle = \langle w_k, v_i \rangle - \frac{\langle w_k, v_i \rangle}{\Vert{}v_i\Vert{}^2}\Vert{}v_i\Vert{}^2 = 0$.
    
- Observe $\text{span}(S_k') \subseteq \text{span}(S_k)$; since $S_k'$ is an orthogonal set of $k$ nonzero vectors, it is linearly independent, so equal dimensions force $\text{span}(S_k') = \text{span}(S_k)$.
