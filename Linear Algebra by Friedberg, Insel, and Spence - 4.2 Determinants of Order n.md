---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-04-03
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
The determinant is defined for an arbitrary matrix recursively with the base case in a 2x2 matrix.

# Definitions
- ***Determinant defined for an arbitrary matrix.*** 
- ***Cofactor Matrix.*** The cofactor of a matrix is a determinant who's magnitude is determined by the determinant of the matrix with one of its rows and columns deleted. The 
- ***Cofactor.*** The cofactor is specified by an entry (i.e. row and column) of a matrix and is a scalar quantity that is determined from the cofactor matrix: 
$$(-1)^{i+j}det(\tilde{A})$$
# Theorems
***Theorem 4.3 (Change in determinant with linear transformation of one row with all others constant).*** The determinant of an $n \times n$ matrix is a linear function of each row when the remaining rows are held fixed.

***Corollary to Theorem 4.3.*** If a matrix has a row consisting entire of zeroes, then its determinant is 0.
***Lemma to 4.3.*** If any of the rows of a matrix, say row $j$ is entirely 0 except for a 1 at column $k$ then the determinant of the entire matrix is determined only by the single cofactor on non-zero entry in row $j$:
$$\det B = (-1)^{i+k}\det \tilde{B_{ik}}$$
***Theorem 4.4 (alternative cofactor formulations to compute the determinant)*** The determinant of a square matrix while defined for the cofactor expansion along the first row, can be evaluated by the cofactor expansion along any row. 

***Corollary to Theorem 4.4.*** If a matrix has two identical rows, then its determinant is 0.

***Theorem 4.5 (Swapping rows changes sign of determinant).*** If $A\in M_{n\times n}(F)$ and $B$ is a matrix obtained from $A$ by interchanging two rows, then $det(B)=-det(A)$ 

***Theorem 4.5 (Determinant is invariant to multiples of an existing row added to another row).*** If $A\in M_{n\times n}(F)$ and $B$ is a matrix obtained from $A$ by adding a multiple of one row to another row, then $det(B)=det(A)$ 

***Corollary to Theorem 4.5.*** If a $n \times n$ matrix has a rank less than $n$, then its determinant is 0.