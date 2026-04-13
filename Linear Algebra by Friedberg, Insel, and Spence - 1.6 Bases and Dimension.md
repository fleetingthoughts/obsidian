---
tags:
  - "#math"
  - linear_algebra
  - arnold_friedberg
date_created: 2026-02-28
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
In [Linear Algebra by Friedberg, Insel, and Spence - 1.5 Linear Dependence and Linear Independence](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.5%20Linear%20Dependence%20and%20Linear%20Independence.md), we had discussed conditions that a subset spanning a subspace must satisfy to be considered the smallest possible set: linear independence. We call this minimal set the basis of a vector space:

***Definition (Basis).*** A basis $\beta$ for a vector space $V$ is a linearly independent subset of $V$ that generates $V$. We also say the vectors of $\beta$ form a basis for $V$.

From this definition, we can derive the following result that is the main motivation for this definition. The definition of a basis was created so that we can satisfy ***Theorem 1.8*** and show that if a basis exists, then it completely defines the subspace.

Note that basis do not have to be a finite number and an infinite number of vectors can be required to span a subspace, but we are primarily concerned with bases with a finite number of vectors. ***Theorem 1.9*** gives us an entry point to determine whether a vector space has a basis, in other words, if there is a finite subset of vectors that generates a vector space, then the basis must exist. Colloquially, this can be restated as follow: "any finite set of vectors that spans a vector space can be reduced to the basis of that vector space."

The following will the most important theorem from which we derive some crucial corollaries is the Steinitz exchange lemma for which  [[Proof of the Steinitz exchange lemma]] involves ***Theorem 1.6*** which establishes that if the basis exists, then it is distinguished by the number of vectors in it. The unique property that every subspace has is the number of vectors in its basis, not the basis itself 

The fact that any basis of a vector space has the same number of vectors makes the # of vectors in a basis an intrinsic property of the vector space that we define as the dimension:

***Definition (Dimension of a Vector Space).*** A vector space, $V$, is called finite-dimensional if it has a basis containing a finite number of vectors and is infinite dimensional otherwise. The number of vectors required in a basis of $V$ is called the dimension of $V$ denoted as $dim(V)$.

As a basis completely describes a vector space and the # of vectors it contains is an intrinsic property of the vector space, the dimension of a vector space lets us relate finite-dimensional vector spaces to other subspaces or vector spaces:

To round off the discussion on the dimension of vector spaces, Friedberg provides an important application of these theorems to the [Lagrange Interpolating formula](Lagrange%20interpolating%20polynomial%20as%20a%20basis%20of%20the%20polynomial%20vector%20space.md) to prove that it provides the minimal number of functions to construct a polynomial that fits through a finite number of points, that is, the Lagrange interpolation formula is a basis of the polynomial vector space

# Summary
- Definition of a basis specifically to establish ***Theorem 1.8*** and find a way to completely describe a vector space
- Proving a basis exists: show that a finite subset of vectors can generate the vector space
- The Steinitz-exchange lemma establishes that any set of independent vectors can be extended to become a basis of a vector space this leads to some important corollaries:
	- The number of vectors in the basis is a distinguishing feature and is unique to a vector space.
- The power of this chapter: a vector space over a field is identified by the number of vectors in its basis defined as the dimension
- Because the dimension is a unique feature, vector spaces defined over the same field can be related to each other by their dimension. For example, if two vector spaces over the same field have the same dimension, then they are equivalent.
# Definitions
***Definition (Basis).*** A basis $\beta$ for a vector space $V$ is a linearly independent subset of $V$ that generates $V$. We also say the vectors of $\beta$ form a basis for $V$.

***Definition (Dimension of a Vector Space).*** A vector space, $V$, is called finite-dimensional if it has a basis containing a finite number of vectors and is infinite dimensional otherwise. The number of vectors required in a basis of $V$ is called the dimension of $V$ denoted as $dim(V)$.
# Theorems
***Theorem 1.8 (The ability of a basis to completely describe a vector space).*** Let $V$ be a vector space and $\{u_1,..u_n\} \in V$. Then $\beta = \{u_1,..u_n\}$ is a basis for $V$ if and only if every $v \in V$ can be uniquely expressed as a linear combination of vectors in $\beta$. 

***Theorem 1.9 (Property of Vector spaces with a finite basis).*** If a vector space $V$ is spanned by a finite set $S$, then some subset of $S$ is a basis for $V$.

***Theorem 1.10 (Replacement Theorem / Steinitz Exchange Lemma).*** Let $V$ be a vector space that is generated by $G$ containing $n$ vectors. Let $L$ be any linearly independent set of $m$ vectors in $V$. Then the following is implied:
- $m \le n$
- There exists a subset $H$ containing exactly $n-m$ vectors such that $L \cup H$ contains $n$ vectors and generates $V$

***Corollary 1 (the required number of vectors for a basis spanning a vector space).*** Let $V$ be a vector space having a finite basis. Then every basis of $V$ has the same number of vectors.

***Corollary 2 (How to identify or create a basis for a vector space).*** Let $V$ be a vector space with the dimension $dim(V)=n$:
1) Any finite generating set of $V$ contains at least $n$ vectors and a generating set that contains exactly $n$ vectors is a basis of $V$
2) Any linearly independent subset of $V$ that contains exactly $n$ vectors is a basis for $V$
3) Every linearly independent subset of $V$ can be extended to a basis for $V$, that is, if $L$ is a linearly independent subset of $V$, then there is a basis $\beta$ such that $L \subseteq \beta$ 

***Theorem 1.11 (Relating Vector spaces and subspaces to each other by their dimension).*** If $W$ is a finite dimensional subspace of $V$, then $dim(W)\le dim(V)$. Moreover, if $dim(W)=dim(V)$ then $W=V$.

***Corollary (How the basis of a vector space relates to the basis of its subspace).*** If $W$ is a finite-dimensional subspace of $V$, then the basis for $W$ can be extended by forming a union with some other vectors linearly independent from it to create a basis for $V$.