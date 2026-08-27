---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.2 The Matrix Representation of A Linear Transformation]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following: Let $V$ and $W$ be finite-dimensional vector spaces having ordered bases $\beta$ and $\gamma$, respectively, and let $T:V \to W$ be linear. Then for each $u \in V$: $[T(u)]_\gamma = [T]_\beta^\gamma [u]_\beta$.
#### Notes
- **Construct Auxiliary Functions:** Fix $u \in V$. Define $f:F \to V$ by $f(a) = au$ and $g:F \to W$ by $g(a) = aT(u)$. Both are linear. Let $\alpha = \{1\}$.
    
- **Establish Composition:** Note that $Tf = g$ because $T(f(a)) = T(au) = aT(u) = g(a)$.
    
- **Apply Composition Theorem:** By the matrix representation of composition, $[g]_\alpha^\gamma = [T]_\beta^\gamma [f]_\alpha^\beta$.
    
- **Translate to Coordinates:** Observe that $[g]_\alpha^\gamma$ is just the single column $[g(1)]_\gamma = [T(u)]_\gamma$, and $[f]_\alpha^\beta$ is $[f(1)]_\beta = [u]_\beta$. Substitute these to yield the formula.
