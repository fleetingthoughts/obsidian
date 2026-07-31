---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.6 Bases and Dimension]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
Define the Lagrange Polynomials.
#### Notes
Let $c_0, c_1, \dots, c_n$ be distinct scalars in a field $F$. The associated Lagrange polynomials $f_0, f_1, \dots, f_n \in P_n(F)$ are defined by $f_i(x) = \prod_{k=0, k \neq i}^{n} \frac{x - c_k}{c_i - c_k}$. They satisfy the foundational Kronecker delta property $f_i(c_j) = \delta_{ij}$.