---
tags:
  - "#linear_algebra"
  - "#math"
  - "#arnold_friedberg"
date_created: 2026-02-22
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
The chapter introduces linear combinations of vectors. The linear combination will play a central role in the theory of vector spaces and is defined as follows:

***Definition (Linear Combination).*** Let $V$ be a vector space and $S$ be a nonempty subset of $V$. A vector $v\in V$ is a linear combination of the vectors $u_i \in S$ if there exists a finite $n$ number of vectors $u_1,u_2,...u_n$ such that $v = \sum_\limits{i=1}^{n}a_iu_i$ where $a_i \in F$ is in the field of the vector space and is referred to as the coefficients of the linear combination

A central problem involving linear combinations is determining whether a vector can be expressed as a linear combination of a set of other vectors, that is, can we determine the coefficients of the linear combination in $v = \sum_\limits{i=1}^{n}a_iu_i$. Friedberg demonstrates algebraically by example, 3 operations we can perform in trying to solve for the coefficients:
1) interchanging the order of any two equations in the system
2) multiplying a equation by a nonzero constant
3) adding a constant multiple of any equation to another equation in the system
He also notes if in the course of these operations, if we encounter the contradiction $0=c$ for some constant $c$, then there is no solution so it is possible to determine if a vector cannot be expressed as a linear combination of other vectors. Friedberg leaves the formal solution to this problem to chapter 3.

To further lay the foundations to this problem, we define the properties of a nonempty subset, $S$  of a vector space $V$ related to linear combination:

***Definition (The Span of a set).*** The set of all linear combinations of the nonempty subset, $S$, of the vector space $V$, is called the span of $S$ and is denoted $span(S)$. We define $span(\emptyset)={0}$.

***Definition (Generating/Spans a vector space).*** The nonempty subset, $S$, of a vector space $V$ is said to span or generate $V$ if $span(S)=V$. That is if $S$ can span $V$, then any $v\in V$ can be expressed a linear combination of the vectors in $S$.

From this we state a theorem about the span of a subset and how it relates to the original vector space

***Theorem 1.5 (The span of a subset of vectors as a subspace of the original vector space).*** The span of any subset, $S$, of a vector space, $V$, is a subspace of $V$ that contains $S$. Additionally, any subspace of $V$ that contains $S$ must also contain $span(S)$. 
