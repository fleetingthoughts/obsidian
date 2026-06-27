---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-04-13
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
For this chapter, we restrict our attention to linear operators on a finite-dimensional vector space where the domain is the same as the codomain. We construct a theory to determine whether there is a matrix representation of our linear operator that is diagonal:
-  Does there exist a basis $\beta$ such that the linear operator $T$ has a diagonal matrix representation $[T]_{\beta}$. What are the criteria for the existence?
-  How can we compute such a basis?
These questions motivate the definitions of eigenvector and eigenvalues to reduce this problem to the problem of matrix algebra:
1) ***Reduce the diagonizability of a linear operator to a problem in matrix algebra***: We define the eigenvector and eigenspace so the following theorem is true: A linear operator is diagonizable if and only if its eigenvectors are a basis of the vector space
2) ***The form of the diagonal matrix***: The diagonal matrix must then consist of eigenvalues in its diagonals. Because they eigenvectors form a basis, this means there exists a change in coordinate matrix so the diagonal matrix is similar to the matrix representation of the linear operator in a different ordered basis
3) ***Existence condition for eigenvalues and the uniqueness***:  The eigenvalues are the solutions to the characteristic polynomial so the number of possible distinct eigenvalues depends on the degree of the characteristic polynomial
4) ***Existence condition for eigenvectors.*** The eigenvectors are the NON-ZERO vectors in the null space of the linear operator shifted by its eigenvalues.

# Results from exercises
- ***Exercise 8 (Definition of the determinant of a linear transformation and its independence from the ordered basis).*** The determinant of a linear transformation is defined by the determinant in its matrix representation but the matrix representation is not unique and changes depending on the chosen matrix representation. It is shown that the determinant of a linear transformation is independent of the choice of ordered basis:
	- All matrix representations are similar to each other.
	- Applying the multiplicative property of matrix determinants shows that change in ordered basis does not affect the determinant
- ***Exercise 9 (Eigenvalue existence condition for invertibility and its relationship to the eigenvalue of the original linear operator):***
	- The inverse of a linear operator exists if and only if 0 is not an eigenvalue.
	- If the eigenvalue of the linear operator is $\lambda$ (which can't be 0), then $\lambda^{-1}$ must be the eigenvalue of the inverse
- ***Exercise 12 (Definition of a scalar matrix. A matrix is diagonizable with only 1 eigenvalue if and only if it is a scalar matrix):
	- A scalar matrix is defined as a diagonal matrix with the same coefficient $\lambda$ for its diagonal entries, that is, $A$ is a scalar matrix if $A=\lambda I$ 
	- If it is determined that the matrix has only one eigenvalue, then it is diagonizable if and only if that matrix is a scalar matrix.
- ***Exercise 13 (Similar matrices have the same characteristic polynomial and the characteristic polynomial is independent of choice of basis).*** The characteristic polynomial of a linear operator is dependent on its matrix representation which is not unique, but this doesn't matter as the polynomial is the same for any choice of basis you have.
- ***Exercise 15 (A matrix and its transpose have the same characteristic polynomial and therefore have the same eigenvalues).***
- ***Exercise 16 (If $v$ is an eigenvector of a linear transformation $T$ or a matrix $A$, then it is also an eigenvector of powers of that matrix).
# Definitions
***Definitions (Diagonalizability of a linear transformation and a matrix).*** A linear operator $T$ on a finite dimensional vector space $V$ is called diagonalizability if there is an ordered basis $\beta$ for $V$ such that $[T]_{\beta}$ is a diagonal matrix. A square matrix $A$ is called diagonalizability if $L_A$ is diagonalizable.

***Definitions (Eigenvector and Eigenvalue of a linear transformation).*** Let $T$ be a linear operator on a vector space $V$. A nonzero vector $v\in V$ is called an eigenvector if there exists a scalar $\lambda$ such that $T(v)=\lambda v$. The scalar  $\lambda$ is called the eigenvalue corresponding to the eigenvector $v$.

***Definition (Characteristic polynomial of a matrix).*** The polynomial $f(t)=det(A-tI_n)$ is called the characteristic polynomial of a matrix $A$.

***Definition (Characteristic of a linear operator and determinant of a linear operator).*** Given a linear operator,$T$,  with matrix representation $A=[T]_{\beta}$, then the determinant of the linear operator is $det(A)$ and the characteristic polynomial of the linear operator is the characteristic polynomial of $A$.

# Theorems
***Theorem 5.1 (Conditions for diagonalizable linear transformation and the matrix representation of a diagonal matrix).*** A linear operator $T$ on a finite dimensional vector space $V$ is diagonalizable <u>if and only if</u> there exists an ordered basis $\beta$ of $V$ consisting of eigenvectors of $T$. Furthermore, the matrix representation, $[T]_{\beta}$, is a diagonal matrix where the diagonals are the eigenvalues corresponding to the eigenvector ordered basis $\beta$.

***Corollary to Theorem 5.1 (The diagonalizability of a matrix).*** A matrix $A \in M_{n\times n}(F)$ is diagonalizable if and only if there is an ordered basis $F^n$ consisting of eigenvectors of $A$. Furthermore, $A$ is diagonalizable if and only if it is similar to a diagonal matrix and is of the form $D=Q^{-1}AQ$ where $Q$ is the matrix whose columns are the eigenvectors and $D$ is the diagonal matrix of eigenvalues corresponding to those eigenvectors.

***Theorem 5.2 (Determining eigenvalue of a matrix).*** Let $A\in M_{n\times n}(F)$. Then a scalar $\lambda$ is an eigenvalue of $A$ if and only if $det(A-\lambda I_n)=0$.

***Theorem 5.3 (Properties of the characteristic polynomial and determining the number of possible eigenvalues).***

***Theorem 5.4 (Determining the eigenvector from the eigenvalue).***
