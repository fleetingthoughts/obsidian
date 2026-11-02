---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: For any matrix $A \in \mathcal{M}_{m \times n}(F)$, $\text{rank}(A^* A) = \text{rank}(A)$.
#### Notes
- Since $A$ and $A^* A$ both have $n$ columns, the dimension theorem $\text{rank}(B) + \text{nullity}(B) = n$ reduces the claim to showing $N(L_{A^* A}) = N(L_A)$.
- If $x \in N(L_A)$, then $Ax = 0$, which gives $A^* Ax = A^*(0) = 0$, so $N(L_A) \subseteq N(L_{A^* A})$.
- Conversely, suppose $x \in N(L_{A^* A})$, so $A^* Ax = 0$, and compute $\Vert{}Ax\Vert{}^2$ under the standard inner product:
$$\begin{aligned} \Vert{}Ax\Vert{}^2 &= \langle Ax, Ax \rangle_m \\ &= \langle x, A^* Ax \rangle_n \\ &= \langle x, 0 \rangle_n \\ &= 0 \end{aligned}$$
- Conclude $Ax = 0$, so $N(L_{A^* A}) \subseteq N(L_A)$, establishing $\text{nullity}(A^* A) = \text{nullity}(A)$ and $\text{rank}(A^* A) = \text{rank}(A)$.
