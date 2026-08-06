---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.3 Compositions of Linear Transformations and Matrix Multiplication]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
  - linear_algebra
  - stephen_abbot
date_created: 2026-07-24
---
Let $V$ and $W$ be finite-dimensional vector spaces having ordered bases $\beta$ and $\gamma$, respectively, and let $T: V \rightarrow W$ be linear. Prove that the coordinate vector of the image $T(u)$ can be computed directly via left-multiplication of the domain coordinate vector by the transformation's matrix representation.
#### Notes
Fix a vector $u \in V$. Define two new linear transformations: $f: F \rightarrow V$ by $f(a) = au$, and $g: F \rightarrow W$ by $g(a) = aT(u)$. Let $\alpha = \{1\}$ be the standard ordered basis for the field $F$. By definition, the composite transformation $Tf$ acts on $a$ as $T(f(a)) = T(au) = aT(u)$, which is exactly $g(a)$. Therefore, $g = Tf$. Taking the matrix representation of both sides with respect to $\alpha$ and $\gamma$, we have $[g]_\alpha^\gamma = [Tf]_\alpha^\gamma$. Applying Theorem 2.11 (composition representation) splits the right side into $[T]_\beta^\gamma [f]_\alpha^\beta$. We then evaluate the representations acting on the basis scalar $1$: $[g(1)]_\gamma = [g]_\alpha^\gamma$ and $[f(1)]_\beta = [f]_\alpha^\beta$. Substituting $g(1) = T(u)$ and $f(1) = u$ into the equation yields the final coordinate identity: $[T(u)]_\gamma = [T]_\beta^\gamma [u]_\beta$.
