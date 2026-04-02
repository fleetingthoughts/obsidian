---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-04-02
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
# Definitions
***Definition of a determinant using a $2\times 2$ matrix***. The determinant of a matrix $A$ is denoted $det(A)$ or $|A|$ and is defined for the $2\times 2$ matrix which will be extended for higher dimensions.
# Theorems
***Theorem 4.1 (change in determinant with linear combinations of one row with others fixed)*** The function $det: M_{2\times 2}(F) \to F$ is a linear function of each row a $2 \times 2$ matrix when the other row is held fixed.  


***Theorem 4.2. (Invertibility characterized by the determinant).*** Let $A \in M_{2\times 2}(F)$. Then the determinant of $A$ is nonzero <u>if and only if</u> $A$ is invertible. Moreover, the inverse $A^{-1}$ takes the form:$$\frac{1}{\det(A)}\begin{bmatrix}
A_{22}&-A_{12} \\
-A_{21}& A_{11}
\end{bmatrix}$$

