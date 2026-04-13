---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-04-13
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
f
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
