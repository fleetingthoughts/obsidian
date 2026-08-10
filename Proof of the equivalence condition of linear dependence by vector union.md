---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.5 Linear Dependence and Linear Independence]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove that a linearly independent set $S$ expanded by an element $v$ is linearly dependent if and only if $v \in \text{span}(S)$.
#### Notes
- **Forward ($\Rightarrow$):** Assume $S \cup \{v\}$ is linearly dependent. Write $av + \sum a_i u_i = 0$ where not all coefficients are zero.
    
- If $a = 0$, then $\sum a_i u_i = 0$ is a non-trivial relation on $S$, contradicting $S$ being independent. Thus $a \neq 0$.
    
- Solve for $v = \sum (-a^{-1}a_i)u_i$, concluding $v \in \text{span}(S)$.
    
- **Reverse ($\Leftarrow$):** Assume $v \in \text{span}(S)$. Write $v = \sum b_j v_j$.
    
- Rearrange to $1v + \sum (-b_j)v_j = 0$. The coefficient $1 \neq 0$, proving $S \cup \{v\}$ is linearly dependent.
