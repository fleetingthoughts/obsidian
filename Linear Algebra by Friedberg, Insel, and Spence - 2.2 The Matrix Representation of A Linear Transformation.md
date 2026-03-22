---
tags:
  - "#math"
  - "#linear_algebra"
  - "#arnold_friedberg"
date_created: 2026-03-12
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
We now ascribe mathematical objects to represent linear transformations: Matrices. We start out by defining some key terms:
- ordered basis: a sequence of vectors that form the basis of a vector space. For two ordered vector spaces $\beta = \{v_1,v_2,v_3\}$ and $\alpha = \{v_1,v_3,v_2\}$, we have that $\alpha \ne \beta$.
- Given any vector $x\in V$, it is known that $x = \sum_{i=1}^na_iv_i$ where $v_i$ is the basis for $V$. We describe the coefficients of that linear combination using the coordinate vector. The coordinate vector is always relative to a certain ordered basis. We call the vector of the coefficients relative to a specific ordering of the sequence of basis of the vector space the following: the coordinate vector of $x$ relative to ordered basis $\beta$ denoted $[x]_{\beta}=(a_{1},a_{2},\dots,a_{n})$.

We then define a way of producing a matrix that represents a linear transformation acting on a basis vector $v_j \in V$ to bring to a vector $w \in W$ which is completely described by its respective ordered basis that is: $$T(v_{j})=w = \sum_{i=1}^na_{ij}w_i$$
We then define the linear transformation as a matrix by the following algorithm that produces each column of $T$:
1) Determine an ordered basis of $W$ (call it $\gamma$) and $V$ (call it $\beta$).
2) For the 1st column of $T$  the transformation is as follows: $T(v_1)=\sum\limits_{i=1}^na_iw_i$ . The first column of the matrix representing $T$ will then be the column $(a_{11},...,a_{n1})^T$.
3) Repeat this for the $j$th vector in the ordered basis of $V$ to produce the $j$th column of the matrix representing $T$
The matrix generated this way is denoted $[T]^{\gamma}_{\beta}$. In summary, we apply the transformation to each ordered basis from the bottom right ordered basis, then determine the coefficients of the linear combination of the top right ordered basis.

This is leading to the fact that this matrix $[T]^{\gamma}_{\beta}$ when multiplied by a vector in the domain takes it to the range, but at this stage, we haven't defined matrix multiplication. We only have a defined this representation. 

With this algorithm, we note the following:
- The matrix will depend on the specific order of the basis we choose. The matrix that results from our particular choice of ordered basis $\gamma$ and $\beta$ is then denoted as $[T]^{\gamma}_{\beta}$ where the top symbol is for the image.
- There will be as many columns as there are basis vectors in the ordered basis of $V$. $col(T) = dim(V)$
- There will be as many rows as there are basis vectors in the range $row(T)=dim(W)$

The Kronecker delta is defined as $\delta_{ij}= 1$ if $i=j$ and 0 otherwise. We then denote the identity matrix of size $n\times n$ by $I_n$ and define it its entries by $(I_n)_{ij}=\delta_{ij}$ 

We also define the the sum of two different transformations as follows:

***Definition (sum of two linearly transformed vectors).*** Given vector spaces $V$ and $W$ with linear transformations $T: V \to W$ and $U: V\to W$, we denote the sum of a vector $x\in V$ transformed in these two different ways as follows: $$U(x)+T(x)=(U+T)(x)$$
We can then show that the sum and multiples of linear transformations are themselves linear
***Theorem 2.7 (Linearity of linear transformations themselves).*** Given two linear transformations $T, U: V\to W$ over a field $F$, we have that for any $a,b \in F$ 
- $(aT+bW)(x)$ is a linear transformation
- Therefore the the collection of all linear transformations satisfies the vector space axioms and is itself a vector space over $F$ denoted as $\mathcal{L}(V,W)$ 

With the way we defined the representation of linear transformations by matrices, we can now relate the vector space of matrices to $\mathcal{L}(V,W)$:
***Theorem 2.8 (matrix representation of linear combinations of linear transformations).*** Let $V, W$ be vector spaces with ordered bases $\beta$ and $\gamma$ respectively, then if we know the matrix representation of the two linear transformations $T,U: V\to W$ over a field $F$, then we can determine the linear combination of these transformations $(aT+bU)(x)$ for $a,b \in F$ and $x \in V$  as follows: $$[aT+bU]^{\gamma}_{\beta}= a[T]_{\beta}^{\gamma}+b[U]_{\beta}^{\gamma}$$
