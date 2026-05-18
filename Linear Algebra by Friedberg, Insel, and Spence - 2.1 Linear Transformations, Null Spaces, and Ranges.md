---
tags:
  - "#math"
  - "#linear_algebra"
  - "#arnold_friedberg"
date_created: 2026-03-10
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
***Definition (Linear Transformation).*** Let $V$ and $W$ be vector spaces over the same field F. We call a function $T : V\to W$ a linear transformation from $V$ to $W$ if for all vectors $x, y\in V$ we have:
1) $T(x)+T(y)=T(x+y)$
2) $T(cx)=cT(x)$

In general if the field is the set of real numbers then 1) implies 2) but some fields are independent of that. There are two important linear transformations $T$ that we define:
- The identity transformation $I(x) = x$
- The zero transformation $T(x) = \vec{0}$ 

We define two important sets of vectors derived from linear transformations $T: V\to W$
- The null space (or kernel) of a linear transformation $T$ is denoted $N(T)$ and it is the set of vectors $x\in V$ such that $T(x)= 0$. For example the null space of the identity matrix $N(I) = {0}$. <u>Note the kernel is a subset of</u> $V$
- The range, denoted $R(T)$ is the set of all the $T(x)$ vectors for $x \in V$. For example the range of the identity matrix is $R(I)= V$ or the entire vector space $V$. In other words $R(T)\subseteq W$. <u>Note the image is a subset of </u>$W$
By ***Theorem 2.1,*** the null space and range are subspaces which is proven by verifying the [3 requirements of a subspace](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.3%20Subspaces.md).

Since the range is a subspace, we are interested in determining a basis for it so that we can completely describe it. The basis of a null space is more complicated, but if we know the basis of the domain vector space, we can determine the basis of the range. ***Theorem 2.2*** states that the basis for the range <u>will be a subset of the set of transformed basis vectors from the domain</u>. So given a linear transformation, if we know the basis of the domain, we can completely determine describe the range since we can derive the basis for the range. 

While ***Theorem 2.2*** gives us a direct way to determine the basis for the range, we do not have a direct way of obtaining the basis for the null space. Fortunately, if we have information about the range, we can say something about the dimension of the null space by ***Theorem 2.3.*** To do so, we have to establish some preliminaries. The size of the null space and the image (i.e. its dimension) are important enough for us to give definitions. Given a linear transformation $T: V\to W$:
- The dimension of the $N(T)$ is called the nullity and is denoted $nullity(T)$.
- The dimension of $R(T)$ is called the rank and is denoted $rank(T)$.
We then establish the relationship between the rank and the nullity using ***Theorem 2.3 (Rank-nullity Theorem).***

The nullity and rank of a linear transformation are useful because they say something general about the linear transformation:
- A nullity of 0 is equivalent to the linear transformation being injective (***Theorem 2.4***).
- If the domain and codomain of the linear transformation have equal dimension, then by ***Theorem 2.3 (Rank-nullity),*** we can derive ***Theorem 2.5*** which states that all the following statements are equivalent:
	1) The linear transformation is injective
	2) The linear transformation is onto
	3) The range has the same dimension as the domain (by [Theorem 1.11](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.6%20Bases%20and%20Dimension.md)).

There is a special result that makes linear transformations especially important and useful for vector spaces. Given, the basis of a $n$-dimensional vector space $V$ and $n$ arbitrary vectors in another vector space $W$ then ***Theorem 2.6*** supplies us with the following existence and uniqueness theorem:
1) There exists a linear transformation that bijectively maps the each of the vectors in the basis $V$ to the $n$ arbitrary vectors in $W$
2) The linear transformation from 1) is unique. This means if we find two transformations $T$ and $S$ that satisfy 1, then $T(v)=S(v)$ for all $v\in V$
***Theorem 2.6*** is general because it applies to any $n$ vectors in the codomain, but we could alternatively try to map to the basis of $W$. There is only one linear transformation that maps the basis of $V$ to the basis of $W$ and in doing so, it completely maps $W$ with domain $V$. 

# Conceptual summary and nuances
- ***Linear algebra is about one kind of function.*** The linear algebra studied is restricted to a special kind of function of vectors: linear transformations. All the theorems in this book will apply to this special kind of function.
- ***All linear transformations have the same output for the zero vector.*** Any linear transformation of the zero vector must result in the zero vector
- ***The transformation of the basis vector uniquely determines the linear transformation.*** The image of a linear transformation is completely determined by its transformation of the basis of the domain. In other words, the basis of the image is $T(v_i)$ where each $v_i$ is a basis vector of the domain.
- The nullity tells us whether a transformation is injective
- Injectivity and surjectivity are separate properties to develop except in the special case where the codomain (NOT THE RANGE) has the same dimension.
- ***The power of knowing the transformation rule of the basis vectors of a domain.***
	- Knowing the transformation of the basis vectors completely describes the range ***Theorem 2.2***. 
	- Knowing the mapping of the basis vectors uniquely determines the linear transformation by ***Theorem 2.6***. Conversely if we know which output vectors we want each basis to map to, then the linear transformation uniquely exists.
# Computational summary
1) ***Determine the basis of the range.*** By ***Theorem 2.2***, we can generate a spanning set for the range so by [Theorem 1.6](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.6%20Bases%20and%20Dimension.md) a basis for the range exists and its a subset of spanning set:
	1) Determine the basis for the domain
	2) Apply the transformation to each vector in the basis. This will be a spanning set of our range
	3) Find a linearly independent subset of the spanning set of the range. The new subset will be a basis for the range.
# Notes from questions
- Question 13: It can be shown that the converse of ***Theorem 2.2*** is true in that if $T(v_i)$ is a basis of the codomain then the $v_i's$ must be a basis of the domain if the dimensions of the codomain and domain are equal or if $T$ is one-to-one.
# Definition
**Definition (Linear Transformation).*** Let $V$ and $W$ be vector spaces over the same field F. We call a function $T : V\to W$ a linear transformation from $V$ to $W$ if for all vectors $x, y\in V$ we have:
1) $T(x)+T(y)=T(x+y)$
2) $T(cx)=cT(x)$

# Theorem
***Theorem 2.1 (The kernel and image of a linear transformation are subspaces).*** Let $V,W$ be vector spaces and the transformation $T: V\to W$ be a linear transformation. Then $N(T)$ and $R(T)$ are both subspaces.

***Theorem 2.2. (The span of the image of a transformation derived from the basis of the domain vector space).*** Given vector spaces $V,W$ and a linear transformation $T: V \to W$, if $V$ has the basis $\beta = {v_1,...v_n}$, then the they form a spanning set for $T(x)$ for $x \in V$ is $T(\beta)= span\{T(v_1),...,T(v_n)\}$.

***Theorem 2.3 (Dimension Theorem/ The Rank-Nullity Theorem).*** Let $V, W$ be vector spaces with $T: V\to W$ be a linear transformation then:$$rank(T)+nullity(T)=dim(V)$$
***Theorem 2.4 (Conditions for the injectivity of a transformation).*** The transformation is one-to-one (injective) if and only if $N(T)=\{0\}$. In other words, the transformation is one-to-one if the null space only contains the 0 vector.

***Theorem 2.5 (Equivalency of various criteria on the image).*** Given two subspaces $V$ and $W$ with equal dimension and a linear transformation $T: V\to W$, the following are equivalent and imply each other:
- $T$ is one-to-one (injective)
- $T$ is onto (surjective)
- $rank(T)=dim(V)$
- $dim(R(T)) = dim(W)=rank(T)$

***Theorem 2.6 (Conditions for the uniqueness of a linear transformation).*** Let $V$ and $W$ be vector spaces over a field with basis $\{v_1,...,v_n\}$ and $\{w_1,...w_n\}$ respectively. Then there exists exactly one linear transformation $T: V\to W$ such that $T(v_i)=w_i$ for $i=1,2,..,n$

