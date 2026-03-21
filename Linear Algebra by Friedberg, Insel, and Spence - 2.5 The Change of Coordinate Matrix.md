---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-03-20
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
After a general discussion of matrices, and the properties of linear transformations and how they relate vector spaces, we now look at specific linear transformations that see lot of use. For this chapter, we look specifically at a linear transformation that stays within a vector space that changes the ordered basis called the change of 
coordinates.

# Definitions
***Unofficial definition (Linear Operation).*** A linear transformation that keeps the vector within the same vector space is called a linear operation

***Definition (Similarity).*** Let $A$ and $B$ be square matrices. $B$ is similary to $A$ if there is an invertible matrix $Q$ such that $B=Q^{-1}AQ$ 
# Theorems
***Theorem 2.22 (The matrix representing the change in coordinates operation).*** Let $\beta$ and $\beta'$ be two ordered basis for a finite dimensional vector space $V$, and let $Q=[I_V]^{\beta}_{\beta'}$. Then:
1) $Q$ is invertible
2) For any $v \in V$, $[v]_{\beta'}$ =$Q[v]_\beta'$ 
***Theorem 2.23 (The relationship between the same linear transformations of different ordinary bases).*** Let $T: V\to V$ be a linear operator $V$ with two different ordered bases $\beta$ and $\beta'$. If $Q$ is the change in coordinate matrix that changes $\beta'$-coordinates into $\beta$-coordinates, then the same linear transformation but with different ordinary bases has the following relationship: $$[T]_{\beta'}=Q^{-1}[T]_{\beta}Q$$ 