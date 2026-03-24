---
tags:
  - linear_algebra
  - math
  - arnold_friedberg
date_created: 2026-03-23
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
With the fundamental results of vector spaces developed in chapters 1 and 2, we now look at one of the most important applications of linear algebra: the solving of systems of linear equations. In this chapter the basic linear transformations that will be performed throughout are defined:
- The definition of elementary operations and the elementary operation performed on the identity matrix
- The elementary row/column operation as a linear transformation and so it can be represented by a matrix and the image is represented by a matrix multiplication
- Developing a fundamental result of the elementary operation: invertibility.
# Definitions
***Definition (Elementary operation).*** Let $A$ be an $m\times n$ matrix, then any one of the following is called an elementary row/column operation:
1) Interchanging any tow rows/columns of $A$
2) Multiplying any row/column of $A$ by a nonzero scalar
3) Adding any scalar multiple of a row/column of $A$ to another row/column

***Definition (Elementary matrix).*** An elementary matrix is a $n \times n$ (i.e. square) matrix that is obtained by performing a singular elementary operation on the $I_n$ identity matrix
# Theorems
***Theorem 3.1 (The elementary operation operation as a matrix multiplication of the elementary matrix).*** Given a $m \times n$ matrix $A$, an elementary row operation performed on $A$ is linear transformation that is represented by an elementary matrix with the same operation such that the matrix multiplication $EA$ results in the desired row operation. Similarly, the column operation on $A$ is represented by a elementary matrix $E$ such that $AE$ results in the desired column operation.

***Theorem 3.2 (invertibility of elementary matrix).*** Elementary matrices are invertible and its inverse is an elementary matrix of the same type (i.e. one of the 3 elementary operations in the definition of row/column operations).

