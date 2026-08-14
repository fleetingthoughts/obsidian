---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.3 Compositions of Linear Transformations and Matrix Multiplication]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following: _:_ Let $V, W$, and $Z$ be vector spaces, and let $T:V \to W$ and $U:W \to Z$ be linear. If $UT$ is onto, then $U$ is onto. Show by counterexample that $T$ need not be onto.
#### Notes
- **Surjectivity Setup:** Assume $UT$ is onto. Let $z \in Z$ be an arbitrary vector in the codomain of $U$.
    
- **Preimage Existence:** Because the composite $UT: V \to Z$ is onto, there exists some vector $v \in V$ such that $(UT)(v) = z$.
    
- **Evaluate Composition:** Rewrite the composite function definition as $U(T(v)) = z$.
    
- **Outer Surjectivity Conclusion:** Let $w = T(v)$. Since $T$ maps $V \to W$, $w \in W$. We have demonstrated that for an arbitrary $z \in Z$, there is a $w \in W$ such that $U(w) = z$. Thus, $U$ is onto.
    
- **Counterexample Construction for $T$:** Define $T: \mathbb{R} \to \mathbb{R}^2$ by $T(x) = (x, 0)$ and $U: \mathbb{R}^2 \to \mathbb{R}$ by $U(x, y) = x$.
    
- **Counterexample Verification:** The composition $(UT)(x) = U(x, 0) = x$ maps $\mathbb{R}$ onto $\mathbb{R}$, meaning $UT$ is onto. However, the range of $T$ is strictly the x-axis in $\mathbb{R}^2$. There is no $x$ such that $T(x) = (0, 1)$, so $R(T) \neq \mathbb{R}^2$, proving $T$ is not onto.
