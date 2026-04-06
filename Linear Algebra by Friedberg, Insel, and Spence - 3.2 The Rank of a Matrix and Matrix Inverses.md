---
tags:
  - linear_algebra
  - arnold_friedberg
  - math
date_created: 2026-03-26
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
Previously we've shown that matrices of matching dimensions are isomorphic to linear transformations, that is, we represent any linear transformation with a matrix and the the definitions of matrix addition and multiplication were defined specifically to match the multiplication (composition) and addition of linear transformations. To develop the tools for matrix operations is therefore to develop the tools for all linear transformations. 

And so, in this chapter we develop some of the tools around the rank for matrix vector space that can then be applied to linear transformations. The majority of the tools are developed around the rank of a matrix and what it represents:
- The analogy between the rank of a matrix and the rank of a linear transformation
- The matrix operations that let us preserve the rank of a matrix using invertible matrices
- The criteria used to determine the rank of a matrix
- Determine the rank of a matrix by its rank normal form
- Relationship between the subspace spanned by the rows of a matrix and its rank
- The relationship between an invertible matrix and the identity matrix.

We had previously defined the rank of a linear transformation, and now we define the rank of a matrix specifically to make it equivalent to the rank of a linear transformation represented by the matrix. The definition of a matrix is represented by the left matrix multiplication, but as we had shown in chapter 2, this is equivalent to the matrix representation of a linear transformation which is formalized in ***Theorem 3.3.***

We are now concerned with determining the rank of a matrix and what the rank of a matrix says about the matrix itself. ***Theorem 3.5*** provides the crucial link in showing that the rank of a matrix is the subspace spanned by the individual columns. The proof for for this is a proof by construction from the fact that a linear transformation is completely described by its transformations of the basis of a domain. Using specifically standard ordered basis of $F^n$, we can show that the image is exactly the linear combination of the columns.

The key to determine the rank of a matrix is therefore to determine how many independent columns it has. The way to do this is to see if we can convert the matrix into a form where we can easily recognize if the columns are independent. ***Theorem 3.6*** shows that any matrix can be reduced to its rank normal form and that we can obtain it by elementary row operations. The rank normal form is the goal and ***Theorem 3.5*** gives us the tools to obtain it buy stating that the rank is preserved if we matrix multiply by invertible matrices [which as shown in 3.1, the elementary matrices are invertible](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%203.1%20Elementary%20Matrix%20Operations%20and%20Elementary%20Matrices.md). Importantly, ***Theorem 3.6.*** shows by a tedious proof of induction that we can always obtain the rank normal matrix with elementary operations.

Some important conclusions from this result are as follows:
1) ***Corollary 1 to Theorem 3.6.*** the rank normal matrix $D$ of a matrix $A$ can take the form $D =BAC$ where $B$ and $C$ are the series of column and row operations respectively. 
2) From 1) taking the transposes reveals an equivalence condition for the rank of a matrix. As highlighted in ***Corollary 2 to Theorem 3.6***, the subspace spanned by the rows of a matrix are identical to the subspace spanned by the column of matrices. We can perhaps prove this from first principles, but the proof in the book was an application of [theorems matrix operations on invertible functions](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%202.4%20Invertibility%20and%20Isomorphisms.md)
3) If we have the additional condition that our matrix $A$ is invertible, then from 1), the form $D=BAC$ reduces simply to $I = A^{-1}A$ which implies that both the inversion of the matrix and the matrix itself are simply a product of elementary row operations
Point 3) in particular gives us a method to compute the inversion of an invertible matrix, we need to determine the series of row operations to bring it to the identity matrix and then apply the inverse of those operations to the identity matrix to determine the inverse.

As the collection of linear transformations between vector spaces is isomorphic to the vector space of matrices, we can compute the rank of matrices by examining the the image of the linear transformation. This is how the rank of a product of matrices is derived in ***Theorem 3.7***
# Definitions
For all definitions, $A \in M_{m \times n}(F)$ is a $m\times n$ matrix
- ***Definition of rank of a matrix (p.152).*** The rank of a matrix $A$ denoted $rank(A)$ is the rank of the linear transformation $L_A: F^n \to F^m$ 

# Theorems
- ***Theorem 3.3 (The rank of a linear transformation is equivalent to the rank of the matrix representing the linear transformation).*** Let $T: V \to W$ be a linear transformation between finite-dimensional vector spaces, and let $\beta$ and $\gamma$ be ordered bases for $V$ and $W$, respectively. Then $rank(T) = rank([T]_{\beta}^{\gamma})$ 

- ***Theorem 3.4 (Conditions for the preservation of rank in composite linear transformations)*** Let $A$ be a $m \times n$ matrix. Let $P$ and $Q$ be invertible $m \times m$ and $n \times n$ matrices respectively. Then the ranks of the multiplication of these matrices are as follows:
	1) $rank(AQ)=rank(A)$
	2) $rank(PA)=rank(A)$ 
	3) Therefore by 1) and 2), $rank(PAQ)=rank(A)$ 

- ***Corollary to Theorem 3.4*** Elementary row and column operationns on a matrix are rank-preserving.

- ***Theorem 3.5 (Determining the rank of a matrix).*** The rank of a matrix equals the maximum number of its linearly independent columns. In other words, the rank of a matrix is the dimension of the subspace generated by the span of its columns.

- ***Theorem 3.6 (Reduction of a matrix to its Rank Normal Form).*** Let $A$ be a $m \times n$ matrix of rank $r$. Then $r \le m$ or $r \le n$ and by means of elementary row and column operations, $A$ can be transformed into the following form called the <u>rank normal form</u>:$$
\begin{bmatrix}I_{r} & 0_{1}\\0_{2} & 0_{3}\end{bmatrix}$$
Where $0_i$ are zero matrices and so $D_{ii}=1$ for $i \le r$ and $D_{ij}=0$ otherwise. 

- ***Corollary 1 to Theorem 3.6 (The possibility to convert a matrix to its Rank Normal Form using invertible matrices)*** If $A$ is a $m \times n$ matrix of rank $r$. Then there exist invertible matrices $B$ and $C$ of sizes $m \times m$ and $n \times n$ such that $D = BAC$ where $D$ is the rank normal matrix of $A$.
- ***Corollary 2 to Theorem 3.6 (properties of a matrix derived from its rank normal matrix).*** 
	1) $rank (A^t)=rank(A)$
	2) By 1) the rank of any matrix equals the maximum number of its independent rows. That is the rank of a matrix is the dimension of the subspace spanned by its rows
	3) The rows and columns of any matrix generate subspaces of the same dimension equal to the rank of the matrix.
- ***Corollary 3 to Theorem 3.6.*** Every invertible matrix is a product of elementary matrices

- ***Theorem 3.7 (Various inequality relationships in the domain and codomains of the composition of linear transformations).*** Let $T:U \to W$ and $U: W\to Z$ be linear transformations on finite-dimensional vector spaces $V$, $W$, and $Z$ then:
	1) $rank(UT) \le rank(U)$
	2) $rank(UT) \le rank(T)$
	Let $A$ and $B$ be matrices such that the product $AB$ is defined. Then :
	3) $rank(AB)\le rank(A)$
	4) $rank(AB) \le rank(B)$ 



