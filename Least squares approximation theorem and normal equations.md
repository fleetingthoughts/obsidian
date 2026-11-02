---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
State the least squares approximation theorem for $A \in \mathcal{M}_{m \times n}(F)$ and $y \in F^m$, including the explicit formula when $\text{rank}(A) = n$.
#### Notes
There exists $x_0 \in F^n$ satisfying the normal equations $(A^* A)x_0 = A^* y$ such that $\Vert{}Ax_0 - y\Vert{} \le \Vert{}Ax - y\Vert{}$ for all $x \in F^n$. If $\text{rank}(A) = n$, then:

$$x_0 = (A^* A)^{-1} A^* y$$
