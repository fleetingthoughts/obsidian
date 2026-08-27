---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.3 Compositions of Linear Transformations and Matrix Multiplication]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following: Let $V, W$, and $Z$ be vector spaces, and let $T:V \to W$ and $U:W \to Z$ be linear. If $UT$ is one-to-one, then $T$ is one-to-one. Show by counterexample that $U$ need not be one-to-one.
#### Notes
- **Null Space Setup:** Assume $UT$ is one-to-one. Let $x \in N(T)$, which means $T(x) = 0$.
    
- **Apply Outer Transformation:** Apply $U$ to both sides of the equation to get $U(T(x)) = U(0)$. By linearity of $U$, this yields $(UT)(x) = 0$.
    
- **Injectivity Application:** Because $UT$ is one-to-one, its null space is trivial ($N(UT) = \{0\}$). Therefore, $(UT)(x) = 0 \implies x = 0$. Since $x \in N(T)$ implies $x = 0$, $N(T) = \{0\}$, proving $T$ is one-to-one.
    
- **Counterexample Construction for $U$:** Define $T: \mathbb{R} \to \mathbb{R}^2$ by $T(x) = (x,0)$ and $U: \mathbb{R}^2 \to \mathbb{R}$ by $U(x,y) = x$.
    
- **Counterexample Verification:** The composition is $(UT)(x) = U(x,0) = x$, which is the identity map on $\mathbb{R}$ and is clearly one-to-one. However, $U(0,1) = 0$, meaning $(0,1) \in N(U)$. Since $N(U) \neq \{(0,0)\}$, $U$ is not one-to-one.
