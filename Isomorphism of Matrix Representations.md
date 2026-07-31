---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.2 The Matrix Representation of A Linear Transformation]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Let $V$ and $W$ be finite-dimensional vector spaces with ordered bases $\beta$ and $\gamma$, respectively, and let $T, U: V \rightarrow W$ be linear transformations. Prove that the matrix representation operation perfectly preserves addition and scalar multiplication, expressed formally as $[T + U]_\beta^\gamma = [T]_\beta^\gamma + [U]_\beta^\gamma$ and $[aT]_\beta^\gamma = a[T]_\beta^\gamma$
#### Notes
Let $\beta = \{v_1, \dots, v_n\}$ and $\gamma = \{w_1, \dots, w_m\}$. By the definition of matrix representations, there exist unique scalars $a_{ij}$ and $b_{ij}$ such that applying the transformations to the basis yields $T(v_j) = \sum_{i=1}^m a_{ij} w_i$ and $U(v_j) = \sum_{i=1}^m b_{ij} w_i$ for each column index $1 \le j \le n$. We evaluate the action of the summed transformation $T + U$ on the domain basis vector $v_j$, which yields $(T + U)(v_j) = T(v_j) + U(v_j) = \sum_{i=1}^m a_{ij} w_i + \sum_{i=1}^m b_{ij} w_i$. Factoring out the codomain basis vectors $w_i$ gives $\sum_{i=1}^m (a_{ij} + b_{ij}) w_i$. By definition, the scalar in the $i$-th row and $j$-th column of the combined representation $[T + U]_\beta^\gamma$ is precisely this aggregated coefficient $a_{ij} + b_{ij}$. This scalar is exactly the sum of the individual matrix entries $([T]_\beta^\gamma)_{ij} + ([U]_\beta^\gamma)_{ij}$. Therefore, $[T + U]_\beta^\gamma = [T]_\beta^\gamma + [U]_\beta^\gamma$. A strictly parallel algebraic expansion substituting $aT$ proves that $([aT]_\beta^\gamma)_{ij} = a(a_{ij})$, validating $[aT]_\beta^\gamma = a[T]_\beta^\gamma$.
