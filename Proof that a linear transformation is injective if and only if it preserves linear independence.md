---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.1 Linear Transformations, Null Spaces, and Ranges]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following: If a linear transformation $T$ is one-to-one, a subset $S$ of the domain is linearly independent if and only if its mapped image $T(S)$ is linearly independent in the codomain.
#### Notes
- **Forward Direction Setup:** Assume $S$ is linearly independent and $T$ is one-to-one. Set up the linear combination $\sum_{i=1}^n c_i T(v_i) = 0$ for vectors $v_i \in S$.
    
- **Apply Injectivity:** By linearity, combine the sum to get $T(\sum c_i v_i) = 0$. Because $T$ is one-to-one, $N(T) = \{0\}$, which implies $\sum c_i v_i = 0$.
    
- **Forward Conclusion:** Since $S$ is linearly independent, all $c_i = 0$. Thus, the set $T(S)$ is linearly independent.
    
- **Reverse Direction Setup:** Assume $T(S)$ is linearly independent. Set up the linear combination $\sum_{i=1}^n c_i v_i = 0$ for vectors $v_i \in S$.
    
- **Apply Transformation:** Apply $T$ to both sides of the equation to get $T(\sum c_i v_i) = T(0) = 0$. By linearity, distribute $T$ to get $\sum c_i T(v_i) = 0$.
    
- **Reverse Conclusion:** Since $T(S)$ is linearly independent, all coefficients $c_i = 0$. Thus, $S$ is linearly independent.
