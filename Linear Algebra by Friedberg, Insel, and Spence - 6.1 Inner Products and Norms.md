---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-05-01
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
We formalize and define a general mathematical operation imbued in a vector space that will have wider applications. As is common in mathematics, the results in a wide variety of fields such as perpendicularity, length, etc.. were explored first before they were reduced to a definition to produce a theoretical reduction. The theoretical reduction in this case is the dot product.

The following inner products were defined:
- The standard inner product on the $F^n$ vector space over the real or complex field.
- The vector space of real-valued functions defined as the integral.
- The Frobenius inner product defined for square matrices over the the real or complex field.
# Definitions
***Definition (Inner Product).*** Let $V$ be a vector space defined over a field $F$. The inner product is a function that assigns a scalar in $F$ to an ordered pair of vectors $x, y \in V$ denoted as $\langle x, y\rangle$. The inner product function has the following defined properties:
1) $\langle x+z, y\rangle= \langle x, y\rangle + \langle z, y\rangle$
2) $\langle cx, y\rangle=c \langle x, y\rangle$
3) $\bar{\langle x, y\rangle}=\langle y, x\rangle$
4) If $x \ne 0$ then the inner product of $x$ with itself, $\langle x, x\rangle$ is a positive real number.

***Definition (Inner Product Space).*** A vector space $V$ over $F$ that has an inner product generally defined is referred to as the inner product space. To be specific, the inner product space refers to the vector space itself. If $F$ is the complex or real numbers, then the vector space is called the complex and real inner product space respectively.

***Unofficial Definition(Standard Inner Product).*** The inner product space is called the standard inner product if it is on the $F^n$ vector space and over the field of real numbers (i.e. $F = \mathbb{R}$). The standard inner product is denoted $x\cdot y$ instead of $\langle x, y \rangle$ 

***Definition (Conjugate Transpose of a matrix).*** Let $A \in M_{m\times n}(F)$ be a matrix. The conjugate transpose of $A$ is the $n \times m$ matrix $A*$ such that $(A*)_{ij}=\bar{A}_{ji}$. The conjugate transpose of a matrix is also called the adjoint of a matrix. 

***Unofficial Definition (Different kinds of inner product spaces).***

***Unofficial Definition (Conjugate linear).*** If a mapping or function has the property that $f(cx)=\bar{c}f(x)$, that is, scalar multiplication pulls out a complex scalar, then it is said that the mapping or function is conjugate linear 

***Definition (Norm).*** Let $V$ be an inner product space. The norm of a vector $x$, denoted $||x||$  is then defined as the positive square root of the inner product with itself: $$||x||=\sqrt{\langle x,x\rangle}$$ 

***Definition (Orthonormal and Orthogonal Vectors).*** Let $V$ be an inner product space. Then we have the following definitions
- Two vectors $x, y$, are orthogonal to each other if $\langle x, y \rangle=0$. 
- A subset of $V$ is orthogonal if any two distinct vectors in $S$ are orthogonal. 
- A vector $x\in V$ is orthonormal if $||x||=1$. 
- A subset $S \subseteq V$ is called orthonormal if $S$ is orthogonal and consists of unit vectors.

***Definition (Normalizing).*** The process of scalar multiplying a vector by the reciprocal of its norm. The resulting product is a unit vector.
# Theorems
***Theorem 6.1 (Inner product space properties).*** Let $V$ be an inner product space. Then for $x, y, z \in V$ and $c \in F$, the following are equivalent:
1) $\langle x, y+z\rangle= \langle x, y\rangle + \langle x, z\rangle$
2) $\langle x, cy\rangle=\bar{c}\langle x, y\rangle$
3) $\langle x, 0\rangle=\langle 0, y\rangle=0$
4) $\langle x, x\rangle=0$ if and only if $x=0$
5) If $\langle x, y\rangle=\langle x, z\rangle$ for all $x\in V$, then $y=z$ 

***Theorem 6.2 (Properties of of the norm).*** Let $V$ be an inner product space over $F$. Then for all $x, y \in V$ and $c \in F$, the following are true:
1) $||cx||=|c|\cdot||x||$ 
2) $||x||=0$ if and only if $x =0$. In general $||x|| \ge 0$ 
3) Cauchy-Schwartz inequality:  $|\langle x, y \rangle|\le ||x|| \cdot ||y||$
4) Triangle Inequality: $||x+y||\le ||x|| + ||y||$
