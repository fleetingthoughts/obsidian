---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.2 The Matrix Representation of A Linear Transformation]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Let $V$ and $W$ be vector spaces over a field $F$, and let $T, U: V \rightarrow W$ be linear transformations. Prove that the composite function $(aT + U)$ formed by standard scalar multiplication and addition is itself inherently linear
#### Notes
Let $x, y \in V$ and let $c \in F$. We must evaluate the action of the combined transformation on the linear combination $cx + y$, written as $(aT + U)(cx + y)$. By the formal definition of transformation addition and scalar multiplication, this expands to $aT(cx + y) + U(cx + y)$. Because $T$ and $U$ are independently given as linear, we can distribute the operations inside the functions to yield $a(cT(x) + T(y)) + (cU(x) + U(y))$. Distributing the exterior scalar $a$ yields $acT(x) + aT(y) + cU(x) + U(y)$. By regrouping the terms associated with the scalar $c$, we obtain $c(aT(x) + U(x)) + (aT(y) + U(y))$. By definition, this factors back into $c(aT + U)(x) + (aT + U)(y)$. This equality strictly satisfies the condition of linearity for the function $aT + U$.
