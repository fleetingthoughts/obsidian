---
tags:
  - "#math"
  - "#linear_algebra"
  - arnold_friedberg
date_created: 2026-02-26
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
As subspaces necessarily contain an infinite number of vectors, we must find a way to describe them. One way is to determine if a finite subset of vectors spans the entire subspace. If such a set of vectors exist then they fully describe the vector space by letting us construct any vector in the subspace by forming linear combinations or check if a candidate vector is in subspace by determining whether it is a linear combination of our finite subset. Determining whether a set of vectors that spans the subspace is the smallest possible set will be central problem that will be the focus of this chapter and expanded in subsequent chapters. The goal is to represent the infinite subspace with the smallest finite # of vectors, that is, there can be no "redundant" vectors. Such redundant vectors will be vectors that can be represented as a linear combination of other vectors. Our search for this minimum # of vectors that spans the subspace therefore cannot have the following property defined as linear dependence

***Definition (Linear Dependence).*** A subset, $S$, of vector space $V$ over some field $F$ will be called linearly dependent if there exist a finite number of distinct vectors $u_1,u_2,...u_n \in S$ and non-zero scalars $a_1,a_2,...a_n$ such that $$a_1u_1 + a_2u_2+...+a_nu_n = 0$$
The case where all the coefficients are 0 is called the trivial representation of 0 and is always the case with any subspace which satisfies the existence of the zero vector axiom. By definition, a linearly dependent $S$ will have a nontrivial representation of the 0 vector. The subset of vectors that we desire will therefore satisfy a condition we define as linear independence:

***Definition (Linear Independence).*** A subset, $S$, of the vector space $V$ that is not linearly dependent is called linearly independent.

The question of finding the smallest number of vectors that spans a subspace will therefore be related to determining whether a set of vectors is dependent or not. For if a set of vectors $S = \{u_1,..u_n\}$ spans a subspace $span(S)=W$ contains a vector $u_i$ that is linearly dependent on the others, then we can create a new subset of $S' \subset S$ that  does not contain the linearly dependent $u_i$ and it will still span $W$ for $span(S')=span(S)=W$. This brief little example demonstrates another general way of determining whether a set of vectors is linearly independent which we state as a theorem:

***Theorem 1.7 (Subset criteria of linearly independent vectors).*** Let $S$ be an independent subset of a vector space $V$, and let a vector $v\in V$ not be in $S$.  Then $S \cup \{v\}$ is linearly dependent if and only if $v\in span(S)$.

Colloquially, a way of restating this theorem is to say that given a set of vectors $S$, if no subset of $S$ can span it, then it is considered independent.


The following is true for any vector space:
- The empty set is linearly independent. Linearly dependent sets must be nonempty.
- A set containing a single nonzero vector is linearly independent for if it was dependent then it must just be the 0 vector
- A set is linearly independent if the only representation of 0 is a trivial representation

We derive some theorems immediately from the definitions of dependence and independence. Colloquially, the theorem and its corollary says 
- A subset of linearly independent vectors is also independent
- The superset of a linearly dependent set is also linearly dependent.

***Theorem 1.6 (Determining dependence of a superset based on the subset).*** For a vector space $V$, if $S_1 \subseteq S_2 \subseteq V$  and $S_1$ is a linearly dependent set of vectors, then $S_2$ is linearly dependent as well

***Corollary (Determining independence of a subset by the superset).*** or a vector space $V$, if $S_1 \subseteq S_2 \subseteq V$  and $S_2$ is a linearly independent set of vectors, then $S_1$ is linearly independent as well.

# Summary
- The empty set is defined to be non-empty
- We defined properties of linear dependence and linear independence
- A subset of linearly independent vectors is independent
- A superset of linearly dependent vectors is dependent.