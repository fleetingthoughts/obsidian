---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: Let VVV be a finite-dimensional inner product space and g:V→Fg: V \to Fg:V→F be a linear functional. Then there exists a unique vector y∈Vy \in Vy∈V such that g(x)=⟨x,y⟩g(x) = \langle x, y \rangleg(x)=⟨x,y⟩ for all x∈Vx \in Vx∈V.
#### Notes
- Choose an orthonormal basis $\beta = \{v_1, v_2, \dots, v_n\}$ for $V$ and define the candidate vector:   $$y = \sum_{i=1}^n \overline{g(v_i)} v_i \in V$$
    
- Define the linear functional $h: V \to F$ by $h(x) = \langle x, y \rangle$ and evaluate $h$ on each basis vector $v_j \in \beta$:$$\begin{aligned} h(v_j) &= \left\langle v_j, \sum_{i=1}^n \overline{g(v_i)} v_i \right\rangle \\ &= \sum_{i=1}^n g(v_i) \langle v_j, v_i \rangle \\ &= g(v_j) \end{aligned}$$
- Since $g$ and $h$ are linear functionals that agree on the basis $\beta$, conclude $g(x) = h(x) = \langle x, y \rangle$ for all $x \in V$.
- To prove uniqueness, suppose $g(x) = \langle x, y' \rangle$ for all $x \in V$; then $\langle x, y - y' \rangle = 0$ for all $x \in V$, which for $x = y - y'$ gives $\Vert{}y - y'\Vert{}^2 = 0 \implies y = y'$.
