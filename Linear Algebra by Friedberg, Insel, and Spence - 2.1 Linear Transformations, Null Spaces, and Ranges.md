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
- The zero transformation $T(x) = 0$ 
We define two important sets of vectors derived from linear transformations $T: V\to W$
- The null space (or kernel) of a linear transformation $T$ is denoted $N(T)$ and it is the set of vectors $x\in V$ such that $T(x)= 0$. For example the null space of the identity matrix $N(I) = {0}$. <u>Note the kernel is a subset of</u> $V$
- The range, denoted $R(T)$ is the set of all the $T(x)$ vectors for $x \in V$. For example the range of the identity matrix is $R(I)= V$ or the entire vector space $V$. In other words $R(T)=w \in W$. <u>Note the image is a subset of </u>$W$
***Theorem 2.1 (The kernel and image of a linear transformation are subspaces).*** Let $V,W$ be vector spaces and the transformation $T: V\to W$ be a linear transformation. Then $N(T)$ and $R(T)$ are both subspaces.

Since the range is a subspace, we can determine a set of vectors that spans it therefore completely describing the vector space:

***Theorem 2.2. (The span of the image of a transformation derived from the basis of the domain vector space).*** Given vector spaces $V,W$ and a linear transformation $T: V \to W$, if $V$ has the basis $\beta = {v_1,...v_n}$, then the basis for $T(x)$ for $x \in V$ is $T(\beta)= {T(v_1),...,T(v_n)}$.

Colloquially, if we know the basis of the vector space that is the domain of a linear transformation, then the basis of the image is the transformation on our known basis.

The size of the null space and the image (i.e. its dimension) are important enough for us to give definitions. Given a linear transformation $T: V\to W$:
- The dimension of the $N(T)$ is called the nullity and is denoted $nullity(T)$.
- The dimension of $R(T)$ is called the rank and is denoted $rank(T)$.

We then establish the relationship between the rank and the nullity:
***Theorem 2.3 (Dimension Theorem/ The Rank-Nullity Theorem).*** Let $V, W$ be vector spaces with $T: V\to W$ be a linear transformation then:$$rank(T)+nullity(T)=dim(V)$$
We discuss some interesting properties of the linear transformation and its rank and nullity.

***Theorem 2.4 (Conditions for the injectivity of the null space).*** The null space is one-to-one (injective) if and only if $N(T)={0}$ 

***Theorem 2.5 (Equivalency of various criteria on the image).*** Given a linear transformation $T: V\to W$, the following are equivalent and imply each other:
- $T$ is one-to-one (injective)
- $T$ is onto (surjective)
- $rank(T)=dim(V)$
- $dim(R(T)) = dim(W)=rank(T)$

 We now distinguish an especially important linear transformation that relates two vector spaces.
***Theorem 2.6 (Conditions for the uniqueness of a linear transformation).*** Let $V$ and $W$ be vector spaces over a field with basis $\{v_1,...,v_n\}$ and $\{w_1,...w_n\}$ respectively. Then there exists exactly one linear transformation $T: V\to W$ such that $T(v_i)=w_i$ for $i=1,2,..,n$

Colloquially, there is only one linear transformation that maps the basis of $V$ to the basis of $W$ and in doing so, it completely maps $W$ with domain $V$. This is because the image $R(T)=span(T(v_1),..,T(v_2))=W$ 