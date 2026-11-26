---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $V$ is a finite-dimensional inner product space over $F$ and $g: V \to F$ is a linear functional, then there exists a unique vector $y \in V$ such that $g(x) = \langle x, y \rangle$ for all $x \in V$
#### Notes
1. Fix an orthonormal basis $\{v_1, \dots, v_n\}$ for $V$.
2. Define $y = \sum_{i=1}^n \overline{g(v_i)} v_i$ and the linear functional $h(x) = \langle x, y \rangle$.
3. Evaluate $h(v_j) = \langle v_j, y \rangle = g(v_j)$ for each $j$ via orthonormality and conjugate-linearity in the second slot; conclude $g = h$ on $V$ since both linear maps agree on a basis.
4. Establish uniqueness: if $\langle x, y \rangle = \langle x, y' \rangle$ for all $x \in V$, then $\langle x, y - y' \rangle = 0$ for all $x \in V$; setting $x = y - y'$ yields $\Vert{}y - y'\Vert{}^2 = 0$, so $y = y'$.
    
- Define the linear functional $h: V \to F$ by $h(x) = \langle x, y \rangle$ and evaluate $h$ on each basis vector $v_j \in \beta$:$$\begin{aligned} h(v_j) &= \left\langle v_j, \sum_{i=1}^n \overline{g(v_i)} v_i \right\rangle \\ &= \sum_{i=1}^n g(v_i) \langle v_j, v_i \rangle \\ &= g(v_j) \end{aligned}$$
- Since $g$ and $h$ are linear functionals that agree on the basis $\beta$, conclude $g(x) = h(x) = \langle x, y \rangle$ for all $x \in V$.
- To prove uniqueness, suppose $g(x) = \langle x, y' \rangle$ for all $x \in V$; then $\langle x, y - y' \rangle = 0$ for all $x \in V$, which for $x = y - y'$ gives $\Vert{}y - y'\Vert{}^2 = 0 \implies y = y'$.
