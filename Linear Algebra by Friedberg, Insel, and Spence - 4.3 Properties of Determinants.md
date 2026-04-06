---
tags:
  - linear_algebra
  - arnold_friedberg
date_created: 2026-04-06
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
As the chapter title suggests, this chapter goes over two properties of determinants and also Cramer's rules:
1) The determinant of a product of a matrix can be computed if we know the determinant of the individual factor matrices
2) The determinant is invariant to the transpose operation.

The proof for each is outlined as follows:
- 

The chapter then concludes with a way that lets us relate the determinant to the solutions of linear equation in Cramer's rule (***Theorem 4.9***). The rule has no computational value as computing determinants is expensive, but it gives us a mathematical relationship for proofs. For instance, given a system $Ax=b$  if $det(A)=1$  and the constant vector $b$ and the entries of $A$ are all integers, then the solution vector $x$ must consist of integers only since the determinant is computed by the summations of the products of the entries
# Definitions

# Theorems
***Theorem 4.7 (Determinant of a product of matrices).*** For any $A, B \in M_{n\times n}(F)$, $det(AB)=det(A)det(B)$ 

***Theorem 4.8 (The determinant of the transpose of a matrix).*** For any $A \in M_{n\times n}(F)$, $det(A^t)=det(A)$.

***Theorem 4.9 (Cramer's rule).*** Let $Ax=b$ be a system of $n$ linear equations with $x= (x_1,...x_n)^T$ be the $n$ unknowns, so that $A$ must be $n\times n$ square. If $det(A) \ne 0$ then this system has a unique solution, and for each $x_k$ for $k= 1,2,..,n$ we can determine it by:
$$x_k = \frac{det(M_k)}{det(A)}$$
Where $M_k$ is the original matrix $A$ but with the $k$-th column replaced by the constant vector $b$.

# Invoked Theorems
- ***Corollary 3 to Theorem 3.6.*** Every invertible matrix is a product of elementary matrices
- ***Corollary 2 to Theorem 3.6 (properties of a matrix derived from its rank normal matrix).*** 
	1) $rank (A^t)=rank(A)$
	2) By 1) the rank of any matrix equals the maximum number of its independent rows. That is the rank of a matrix is the dimension of the subspace spanned by its rows
	3) The rows and columns of any matrix generate subspaces of the same dimension equal to the rank of the matrix.
- ***Theorem 4.6 (Determinant is invariant to multiples of an existing row added to another row).*** If $A\in M_{n\times n}(F)$ and $B$ is a matrix obtained from $A$ by adding a multiple of one row to another row, then $det(B)=det(A)$ 

- ***Corollary to Theorem 4.6.*** If a $n \times n$ matrix has a rank less than $n$, then its determinant is 0.


