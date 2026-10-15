---
parent:
tags:
  - "#flashcard"
date_created: 2022-08-25
---
Prove: Let $V$ be an inner product space and $S = \{v_1, v_2, \dots, v_k\}$ be an orthogonal subset of $V$ consisting of nonzero vectors. If $y \in \text{span}(S)$, then
#### Notes
- Write $y = \sum_{i=1}^k a_i v_i$ for scalars $a_1, \dots, a_k \in F$.
- Fix $j \in \{1, \dots, k\}$ and take the inner product with $v_j$: $\langle y, v_j \rangle = \sum_{i=1}^k a_i \langle v_i, v_j \rangle$.
- Apply orthogonality ($\langle v_i, v_j \rangle = 0$ for $i \neq j$) to collapse the sum to $\langle y, v_j \rangle = a_j \Vert{}v_j\Vert{}^2$.
- Divide by $\Vert{}v_j\Vert{}^2 \neq 0$ (since $v_j \neq 0$) to isolate $a_j = \frac{\langle y, v_j \rangle}{\Vert{}v_j\Vert{}^2}$.
