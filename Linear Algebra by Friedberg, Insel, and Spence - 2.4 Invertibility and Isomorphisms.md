---
tags:
  - math
  - linear_algebra
date_created: 2026-03-16
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---

Now that matrix operations have been defined in a way that lets us represent any linear transformations, we are now in a position to look at the inverse of linear transformations and show that matrices can be used in general to relate any general vector spaces that satisfy the criteria of isomorphism.

The chapter has quite a few definitions and the theorems have simple derivations that require you to carefully think through the definitions. For all proofs we assume vector spaces $V$, and $W$ and linear transformations $T: V \to W$ 


# Linearity of the inverse of a linear transformation
***Definition (Inversion of a linear transformation).*** Given $T: V \to W$ a matrix $U: W \to V$ is its inverse if $TU = I_W$ and $UT = I_V$. The inverse $U$ is denoted as $T^{-1}$

***Theorem 2.17 (the inverse of a linear).*** If $T$ is linear, and invertible, than $T^{-1}$ is linear.

***Corollary.*** If $T$ is an invertible linear transformation of $V$ to $W$ then $dim(V)=dim(W)$.

# Matrix representation of the inverse of a linear transformation
We defined invertibility of a linear transformation, now we define the invertibility of a matrix and show how the inverse of a matrix is a matrix representation of the inverse

***Definition (Inversion of a matrix).*** Given a $n\times n$ matrix $A$, the matrix is invertible if there exists a $n\times n$ matrix $B$ such that $AB=BA=I_{{n}}$

***Corollary.*** The matrix $A$ is invertible if and only if its left multiplication $L_A$ is invertible. 

Unofficial theorem: The inverse of an invertible matrix is unique

***Theorem 2.18 (Invertibility of a linear transformation is equivalent to the invertibility of its matrix representation).*** A linear transformation is invertible <u>if and only if</u> its matrix representation $[T]^{\gamma}_{\beta}$ is invertible, that is there exists a $T^{-1}$. Furthermore, the matrix representation of the linear transformation is $[T^{-1}]^{\beta}_{\gamma}= ([T]^{\gamma}_{\beta})^{-1}$ .

# The use of matrices to represent isomorphic vector spaces

***Definition (isomorphic vector spaces and isomorphism).*** Two vector spaces $V, W$ are considered isomorphic if there exists a linear transformation $T: V \to W$ such that $T$ is invertible. Such a linear transformation is called the "isomorphism from $V$ to $W$".

***Theorem 2.19. (Equivalence criteria for isomorphism).*** Two finite-dimensional vector space $V$ and $W$ are isomorphic <u>if and only if</u> $dim(V)=dim(W)$.

This lets us use the $n$-tuple vector space $F^n$ to relate to any vector space since it is isomorphic with any vector space with a dimension of $n$.

***Theorem 2.20 (Relationship between linear transformations and $m \times n$ matrices).*** 
