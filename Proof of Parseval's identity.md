---
parent:
tags:
  - "#flashcard"
date_created: 2022-08-25
---
Prove: Let $\{v_1, v_2, \dots, v_n\}$ be an orthonormal basis for a finite-dimensional inner product space $V$. For any $x, y \in V$,

$$\langle x, y \rangle = \sum_{i=1}^n \langle x, v_i \rangle \overline{\langle y, v_i \rangle}.$$
#### Notes
- Expand both vectors in the orthonormal basis: $x = \sum_{i=1}^n \langle x, v_i \rangle v_i$ and $y = \sum_{j=1}^n \langle y, v_j \rangle v_j$.
- Substitute into the inner product and use sesquilinearity: $\langle x, y \rangle = \sum_{i=1}^n \sum_{j=1}^n \langle x, v_i \rangle \overline{\langle y, v_j \rangle} \langle v_i, v_j \rangle$.
- Invoke orthonormality ($\langle v_i, v_j \rangle = \delta_{ij}$) to collapse the double sum to $\sum_{i=1}^n \langle x, v_i \rangle \overline{\langle y, v_i \rangle}$.
