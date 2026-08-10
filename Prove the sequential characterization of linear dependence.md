---
parent:
tags:
  - "#flashcard"
date_created: 2026-07-24
---
Prove that a set $S\{u_{1}u_{2},\dots,u_{n}\}$ is linearly dependent if and only if $u_1=0$ or $u_{k+1}\in span(\{u_1,...,u_{k+1}\})$ 
#### Notes
- **Forward:** Assume $S = \{u_1, \dots, u_n\}$ is dependent. $\sum_{i=1}^n c_i u_i = 0$ with not all $c_i = 0$. Let $k+1$ be the largest index such that $c_{k+1} \neq 0$. If $k+1 = 1$, then $u_1 = 0$. If $k+1 > 1$, solve for $u_{k+1}$ to show it is in $\text{span}(\{u_1, \dots, u_k\})$.
    
- **Reverse:** If $u_1 = 0$, $1u_1 = 0$, making $S$ dependent. If $u_{k+1} = \sum_{i=1}^k a_i u_i$, rearrange to $\sum a_i u_i - u_{k+1} = 0$, a non-trivial linear combination equaling zero.