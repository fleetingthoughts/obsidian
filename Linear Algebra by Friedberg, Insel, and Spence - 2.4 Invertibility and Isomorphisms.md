---
tags:
  - math
  - linear_algebra
date_created: 2026-03-16
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---

Now that matrix operations have been defined in a way that lets us represent any linear transformations, we are now in a position to look at the inverse of linear transformations and show that matrices can be used in general to relate any general vector spaces that satisfy the criteria of isomorphism. The chapter is outlined as follows:
- Definition of invertible linear transformation, properties of invertible linear transformation and the criteria for invertibility
- Definition of invertible matrix and how it shares all the same properties as invertible linear transformations that let us carry over our results and matrix operations
- The generalization of the fact that vector spaces can be represented by matrices: isomorphism
# Invertibility and the linearity of the inverse of a linear transformation
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

***Theorem 2.20 (Relationship between linear transformations and $m \times n$ matrices).*** Given a vector space $V$ and $W$ with dimensions $n$ and $m$ respectively and with ordered bases $\beta$ and $\gamma$ respectively, then the function $\Phi_{\beta}^{\gamma}: \mathcal{L}(V,W)\to M_{m\times n}(F)$ defined by $\Phi_{\beta}^{\gamma}(T)=[T]_{\beta}^{\gamma}$ for $T \in mathcal{L}(V,W)$ 

Colloquially, what theorem 2.20 says is that the collection of linear transformations from vector spaces of dimensions $n$ to vector spaces of dimension $m$ is isomorphic with the vector space of $m \times n$ matrices. The function $\Phi$ is one that takes the linear transformations and ascribes a $m \times n$ matrix to it, and it is a bijective function (invertible and an isomorphism). 

Since the vector space of linear transformations is isomorphic with $m \times n$ matrices, then that means $\mathcal{L}(V,W)$ is finite dimensional $mn$.

# Standardization of the representation of a vector space using the $n$-tuple vector space $F^n$.
In summary, any linear transformation can be uniquely represented by matrices with respect to a certain ordered base (note that the matrix that can map vector space to another vector space is technically not unique but we force it to by using a specific order of bases). In the beginning of [2.2 The Matrix Representation of A Linear Transformation](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%202.2%20The%20Matrix%20Representation%20of%20A%20Linear%20Transformation.md), we had defined the the coordinate vector with respect to an ordered basis, but now with the concept of isomorphism, we can see that process of mapping a vector $v\in V$ to a coordinate vector with respect to an ordered basis is just an isomorphism that maps $V\to F^n$ where $n=dim(V)$. We now discard that previous definition and proceed with one rooted in our theorems by defining it as a particular linear transformation linear transformation and as a result, we can prove that it is an isomorphism (see ***Theorem 2.21***). This demonstrates we can always represent any vector in a vector space uniquely with an equal dimension $F^n$-tuple.

***Definition (standard representation of a vector space with respect to an ordered basis).*** The standard representation of $V$ with respect to an ordered basis $\beta$ is the function $\phi_{\beta}=V\to F^n$ defined by $\phi_{\beta}(x)=[x]_{\beta}$ for each $x \in V$. The linear transformation $\phi$ has been called the coordinate mapping or coordinate isomorphism too. 

***Theorem 2.21 (Isomorphism of the function that standardizes the representation of a vector space).*** The $\phi_{\beta}$ from the definition directly above is an isomorphism (i.e. it is bijective).
