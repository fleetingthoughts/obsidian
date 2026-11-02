---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: Let $A \in \mathcal{M}_{m \times n}(F)$ and $b \in F^m$ such that $Ax = b$ is consistent. Then there exists a unique minimal solution $s$ to $Ax = b$, and $s$ is the unique solution to $Ax = b$ lying in $R(L_{A^*})$.
#### Notes
- Set $W = R(L_{A^*})$, so $W^\perp = N(L_A)$; take any solution $x$ to $Ax = b$ and decompose $x = s + y$ with $s \in W$ and $y \in W^\perp = N(L_A)$.
    
- Verify that $s \in R(L_{A^*})$ is a solution to $Ax = b$:
    
    $$As = A(x - y) = Ax - Ay = b - 0 = b$$
    
- For any solution $v$ to $Ax = b$, note that $v - s \in N(L_A) = W^\perp$ while $s \in W$; apply the Pythagorean theorem:
    
    $$\begin{aligned} \Vert{}v\Vert{}^2 &= \Vert{}s + (v - s)\Vert{}^2 \\ &= \Vert{}s\Vert{}^2 + \Vert{}v - s\Vert{}^2 \\ &\ge \Vert{}s\Vert{}^2 \end{aligned}$$
    
- Observe that $\Vert{}v\Vert{} = \Vert{}s\Vert{}$ holds if and only if $\Vert{}v - s\Vert{} = 0 \iff v = s$, proving $s$ is the unique minimal solution.
    
- If $s' \in R(L_{A^*}) = W$ is also a solution to $Ax = b$, then $s' - s \in W \cap N(L_A) = W \cap W^\perp = \{0\}$, so $s$ is the unique solution in $R(L_{A^*})$.
