---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 6.3 The Adjoint of a Linear Operator]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch6
date_created: 2022-08-25
---
Prove: If $T$ is a linear operator on a finite-dimensional inner product space $V$, then $\text{rank}(T) = \text{rank}(T^*)$ and $\text{rank}(T^* T) = \text{rank}(T T^*) = \text{rank}(T)$.
#### Notes
Using $R(T^*) = (N(T))^\perp$ and the dimension theorem:

$$\text{rank}(T^*) = \dim(R(T^*)) = \dim((N(T))^\perp) = \dim(V) - \text{nullity}(T) = \text{rank}(T)$$

Since $N(T^* T) = N(T)$, we have $\text{rank}(T^* T) = \text{rank}(T)$. Replacing $T$ with $T^*$ gives $\text{rank}(T T^*) = \text{rank}(T^*) = \text{rank}(T)$.
