---
tags:
  - "#math"
  - "#linear_algebra"
  - "#arnold_friedberg"
date_created: 2026-02-20
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
***Definition of Subspaces.*** A subset $W$ of a vector space $V$ over a field $F$ is called a subspace of $V$ if $W$ is a vector space over $F$ with operations of additions and scalar multiplication defined for $V$

By this definition $V$ and $\{0\}$ are subspaces of $V$ , that is the set containing only the zero vector is a subspace of any vector space and any vector space is a subspace of itself.

To determine whether a proposed subspace meets the definition, we only need to verify the following:
1) The subspace is closed under addition
2) The subspace is closed under scalar multiplication
3) The subspace has a zero vector
The other properties (commutativity and associativity of vector addition; and left/right distributive property of scalar multiplication) are not required as they were already in place when we defined the operations of addition and multiplication for the vector space and so the subspace that ISNA subset of the vector space is defined to have the same operations. The axiom of the additive inverse does not need to be checked as the other 3 conditions already imply it:

***Theorem 1.3 (redundancy of the additive inverse condition)***. The subspace $W$ of vector space $V$ has an additive inverse if and only if the subspace is closed under addition, scalar multiplication, and it has the 0 vector.

Notice that this is an equivalency theorem so the sufficiency and necessity both need to be shown and its also made easier by the fact that we assumed $W$ is a subspace (which is a vector space itself) so we already implicitly assumed it is closed under addition and scalar multiplication. I think the theorem can be simplified but I think its still worth leaving in "closed under addition" and "closed under scalar multiplication" even though they are part of the definition of $W$ to remind me that they are conditions that need to be checked
The rest of this chapter provides examples of subspaces:
- The set of $n \times n$ matrices with a trace of 0

The next theorem shows how we can form new subspaces from known subspaces

***Theorem 1.4 (Intersection of Subspaces)***. Any intersection of subspaces of the vector space $V$ is a subspace of $V$. 

The proof follows by checking if the set $W$ that is the intersection of other subspaces $(C_{i})$  satisfies the 3 conditions:
- Every subspace has the 0 vector so their intersection will have the 0 vector. $W$ therefore has the 0 vector
- If $W$ has two vectors $x$ and $y$ then every $C_i$ also contains $x$ and $y$ and must also contain $x+y$ as well therefore their intersection $W$ contains $x+y$
- If $W$ has a scalar $c$ and a vector $x$, then since it was the intersection of the $C_i's$, every $C_i$ also contains $c$ and $x$ and by 2), they must contain $cx$ as well so their intersection $W$ contains $cx$ and is closed under multiplication.

In general, unions of subspaces do not result in subspaces themselves because they are not necessarily closed under addition. It is shown in Exercise 19 that the union of subspaces result in a subspace if and only if one of the subspaces contains the other