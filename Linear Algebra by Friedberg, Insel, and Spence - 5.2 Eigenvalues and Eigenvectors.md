---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-04-17
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
Chapter 5.1 developed necessary and sufficient conditions for diagonalizability in Theorem 5.1 with the existence of an ordered basis of eigenvectors. If the conditions are satisfied, then we know the form the matrix will take. 

The previous chapters has touched on how we can identify whether a matrix is diagonalizable, but we now fill in the gaps by developing a test to determine whether the matrix can be diagonalized, and what the eigenvectors are. This is done as follows:

The check to test whether a linear transformation $T$ is diagonalizable is as follows:
- The characteristic polynomial of $T$ splits
- For each eigenvalue $\lambda$ of $T$, the multiplicity of $\lambda$ is equal to $nullity(T-\lambda I)$. In other words, the multiplicity is equal to $n-rank(T-\lambda I)$ where $n$ is the rank of the vector space where $T$ operates.

# Summary and notes from exercises
- Computation of the $n$th power of a matrix, $A^n$ is more straightforward if it is diagonalizable for then we have $PAP^{-1}=P^{-1}AP=D$ and then $A^n$ can be computed as follows: $$A^n=PD^nP^{-1}$$
	So instead of $n$ matrix multiplication, we have the much easier powers of a diagonal matrix and two additional matrix multiplications


# Definitions

***Definition (Polynomial splitting over a field).*** A polynomial $f(t)$ is said to split over its field if the polynomial can be decomposed into a product of linear factors: $$f(t)-c(x-a_{1})(x-a_{2})\dots(x-a_{n}) \text{\quad for\quad}a_{i}\in \mathbb{R}$$
***Definition (Multiplicity or algebraic multiplicity).*** Let $\lambda$ be an eigenvalue of a linear transformation. The multiplicity or algebraic multiplicity of $\lambda$ is the largest number $k\in \mathbb{R}$ such that $(x-\lambda)^k$ is a factor of the characteristic polynomial of the linear transformation.

***Definition (Eigenspace).*** Let $T$ be a linear transformation on a vector space $V$. Let $E_\lambda=\{x\in V: \lambda x\}=N(T-\lambda I_{V})$ be defined. $E_\lambda$ is called the eigenspace of $T$ corresponding to the eigenvalue $\lambda$. Analogously,  $E_{\lambda}$ of a matrix $A$ is called the eigenspace of $L_A$.

# Theorems
***Theorem 5.5 (The set of eigenvectors are independent if they belong to different eigenvalues).***

***Corollary to Theorem 5.5 (Sufficient condition for existence of basis of eigenvectors).*** Let $T$ be a linear operator over an $n$-dimensional $V$ vector space. The transformation $T$ is diagonalizable if it has $n$ distinct eigen values.

***Theorem 5.6 (Necessary condition for diagonalizability using the characteristic polynomial).*** If a linear transformation is diagonalizable, the characteristic polynomial of linear transformation splits over the field $F$. The converse isn't necessarily true.

***Theorem 5.7 (Dimension of the eigenspace bounded by the multiplicity).*** Let $T$ be a linear operator with an eigenvalue $\lambda$  of multiplicity $m$. Then the dimension of the eigenspace corresponding to $\lambda$ has it dimensions bounded as follows: $1\le dim(E_{\lambda})\le m$.

***Theorem 5.8 (Test for diagonalizability and subsequent method to determine an ordered basis of eigenvectors )

