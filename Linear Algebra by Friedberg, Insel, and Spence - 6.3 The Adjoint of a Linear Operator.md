---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-05-06
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
We establish preliminaries about the adjoint of a linear operator and how the past three concepts of dot product, linear operator, and adjoint linear operator all relate to each other. The preliminaries and relations will help us solve two critical problem in statistics called the least squares approximation, and the minimal solution of a non-unique consistent solution.
# Definitions
***Definition (Minimal Solution).*** Given a consistent system of linear equations $Ax=b$ that has no unique solution. A solution vector $s$ is called the minimal solution if it satisfies $||s|| \le ||u||$ for all other solutions $u$ the system of equations.

# Summary of concepts
- The existence, uniqueness, and linearity of the adjoint of a linear transformation is guaranteed for a finite dimensional inner product space, but the existence is not guaranteed in an infinite dimensional inner product space

# Summary of computational
- ***Computation of the adjoint of a linear transformation.*** 
	1) Determine the matrix representation of the original linear transformation
	2) The adjoint of the matrix in 1) is the matrix representation of the adjoint linear transformation
- ***Determine the least squares approximation.*** If a system of linear equations $Ax=y$ has no solutions, we can determine of the vector $x_o$ that is the "closest" answer. To determine the closest solution we need the following:
	1) $A\in M_{m\times n}(F)$ 
	2) The rank of the matrix in 1) is equal to the number of columns $rank(A)=n$
	3) A vector that is a tuple with the same # of elements as rows of $A$, that is, $y \in F^m$ 
	The closest solution is then the following: $$x_o=(A^*A)^{-1}A^*y$$
- ***Determine the unique minimal solution for a consistent system of equations with multiple solutions.*** 
# Theorems
***Theorem 6.8 (The linear transformation expressed a dot product with a unique vector).***

***Theorem 6.9 (A linear transformation's relationship to its adjoint).***

***Theorem 6.10 (The matrix representation of the adjoint transformation in terms of the matrix representation of the original linear transformation).***

***Theorem 6.11 (Properties of the adjoint linear operator).***

***Corollary to Theorem 6.11 (Extension of 6.11 to matrices as opposed to linear operators).***

***Lemma 1 (relation between the dot product vector with a transformed vector and the dot product with the adjoint transformation).***

***Lemma 2 (The $A^*A$ has the same rank as $A$).

***Corollary to Lemma 2 (Sufficient condition for the invertibility of $A^*A$).***

***Theorem 6.12 (Existence of the least squares vector and determination of the vector if the rank is equal to number of columns).*** 

***Theorem 6.13 (The existence of a minimal solution for a system of linear equations that has no unique solutions and computation of the minimal solution).***