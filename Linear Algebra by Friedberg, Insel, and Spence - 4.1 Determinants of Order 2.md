---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-04-02
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
- Determinant defined by 2 x 2 matrix
- Area of parallelogram determined by absolute value of determinant
- Right-hand and left-hand coordinate system

- Properties of determinants
	- swapping rows makes determinant negative keeps magnitude
	- one row added to another row does not change determinant
	- If two rows or two columns are identical, then determinant is 0.
	- Determinant is a linear transformation if only one row is transformed.
	- det(AB)=det(A) det(B)
# Definitions
***Definition of a determinant using a $2\times 2$ matrix***. The determinant of a matrix $A$ is denoted $det(A)$ or $|A|$ and is defined for the $2\times 2$ matrix which will be extended for higher dimensions.

***Definition Classical Adjoint (also called Adjugate Matrix) of a matrix.***
# Theorems
***Theorem 4.1 (change in determinant with linear combinations of one row with others fixed)*** The function $det: M_{2\times 2}(F) \to F$ is a linear function of each row a $2 \times 2$ matrix when the other row is held fixed.  


***Theorem 4.2. (Invertibility characterized by the determinant).*** Let $A \in M_{2\times 2}(F)$. Then the determinant of $A$ is nonzero <u>if and only if</u> $A$ is invertible. Moreover, the inverse $A^{-1}$ takes the form:$$\frac{1}{\det(A)}\begin{bmatrix}
A_{22}&-A_{12} \\
-A_{21}& A_{11}
\end{bmatrix}$$

