---
tags:
  - linear_algebra
  - math
  - arnold_friedberg
date_created: 2026-03-26
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
To show how our concepts from chapter 2 can be applied to the solving of linear equations, we look to describe a general system of linear equations as a vector space and then apply our concepts:
- The matrix description of a system of linear equations and descriptors of its solution set by a linear transformation $A: F^m \to F^n$ where $A$ is necessarily a $m \times n$ matrix
- Determine the whether the homogenous system of linear equations has a solution using the concept of the null space
- Determine whether a solution is unique using the null space of the coefficient matrix
- Determine equivalency conditions for when the system is unique by the rank of the matrix
- Determine if a solution exists at all (if a system is consistent) by the rank of the matrix and rank of the augmented matrix.

As a corollary, this means if $A$ is a $m \times n$ matrix such that $m <n$ then since the dimensions of the domain is less than the dimensions of the codomain, by the rank-nullity theorem, the null space of the matrix is nonempty and therefore we have solutions for the homogenous equation.

An important reason to determine the nullity of the coefficient matrix is to determine the uniqueness of a solution. If we look at the nonhomogeneous system of equations where now we specify a non-zero vector to map to in the codomain, the solution is the span of the basis of the null-space plus the particular vector that does the mapping. This means if the nullity is nonzero, we do not have unique solutions for any given solution set.

As a final application of the rank-nullity theorem, we can determine when the solution is unique, in which case the rank of the null space has to be 0. For the nullity of $A$ to be 0, $A$ has to be a bijective linear transformation in which case it is a unique linear transformation and therefore invertible as well. The equivalence of uniqueness in solution and invertibility is specified in ***Theorem 3.9***.

# Definitions
- ***Names for the matrix form of a system of linear equations***. Given the following matrix representation of a linear system of equations, we define each component as follows: $$Ax = b$$
	- <u>System:</u> The entire equation
	- <u>Coefficient matrix of the system</u>: $A$
	- <u>Solution to the system</u>: $b\in F^n$ 
- ***Consistent and Inconsistent System*** A system is consistent if the set of solutions is nonempty. It is inconsistent otherwise
- ***Homogenous and Nonhomogeneous*** A system of linear equations is homogenous if the solution vector is the $0$ vector. Otherwise it is nonhomogeneous. Given a system of equations $Ax=b$, the system $Ax = 0$ is called the <u>homogenous system corresponding to the original system</u>
- ***Augmented matrix*** The augmented matrix of a system is the coefficient matrix, $A$, with the solution vector, $b$, added as an additional column and is denoted $(A|b)$
# Theorems
For all the theorems below, the system of linear equations considered is denoted $Ax=b$ where the coefficient matrix is $m \times n$ not necessarily square that maps $A: F^m \to F^n$  unless stated otherwise stated
- ***Theorem 3.8. (Relating the homogenous solution to the null space of the linear transformation).*** Let $K$ denote the solutions to the homogenous system $Ax=0$. Then $K$ is the null space of the linear transformation and is a subspace of the codomain $F^n$. As a null space, it has the dimensions by the rank-nullity theorem: $$dim(K)=dim(N(L_{A}))=n-rank(L_{A})=n-rank(A)$$
- ***Theorem 3.9. (Uniqueness of a solution to a set of linear equations based on the dimensions of the null space of the linear transformation).*** Assume the system of linear equations is consistent. Let $K$ be the solution set of a consistent system of linear equations  and $K_H$ be the solution set of the corresponding of the homogenous system $Ax=0$, then $K_H$ is a subset of the solution set $K$ and for any solution $s$ we must also have : $$K = s+K_{H}=\{s+k:k\in K_{H}\}$$

- ***Theorem 3.10. (Conditions for the uniqueness of a solution).*** If $A$ is invertible, then the system has exactly one solution namely $A^{-1}b$. Conversely, if the system has exactly one solution, then $A$ is invertible

- ***Theorem 3.11 (Criteria for consistency based on the rank of the linear transformation and the augmented matrix).*** The system of linear equations is consistent if and only if $rank(A)=rank(A|b)$ 

