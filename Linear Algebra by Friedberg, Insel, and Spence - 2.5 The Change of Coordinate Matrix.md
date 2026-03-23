---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-03-20
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
After a general discussion of matrices, and the properties of linear transformations and how they relate vector spaces, we now look at specific linear transformations that see lot of use. For this chapter, we look specifically at a linear transformation that stays within a vector space that changes the ordered basis called the change of coordinates.

***Theorem 2.22( The matrix representation of change in coordinates)*** demonstrates an invertible matrix that transforms a vector represented in the $\beta'$ ordered basis to a vector that is represented in the $\beta$ ordered basis. The matrix described in ***Theorem 2.22*** is called the change in coordinates matrix and it changes us from $\beta'$-coordinates to $\beta$-coordinates. Since this matrix is invertible, the inverse of the matrix takes us back to $\beta'$ coordinates.

Linear transformations that maps to the same vector space $T: V \to V$ are called linear operators of which the change in coordinates matrix is an example. By definition:
- The subspace of transformed vectors has the same dimensions as $V$ so it completely describes it
Given a linear operator $T$ in a vector space $V$ with two possible ordered basis $\beta$ and $\beta'$. We have the choice of $[T]_{\beta}$ or $[T]_{\beta'}$ but by definition, they both completely describe $V$ so they span the same vector space. ***Theorem 2.23*** derives the relationship between these two different transformations.

In summary, to change the coordinates of a given vector is to change the choice of ordered basis used to describe (and therefore the coordinate matrix). Now with both ***Theorem 2.22,*** we have a way to switch the same vector to a description by a different ordered basis and ***Theorem 2.23*** lets us change change the coordinates of transformations.
# Definitions
***Unofficial definition (Linear Operation).*** A linear transformation that keeps the vector within the same vector space is called a linear operation

***Definition (Similarity).*** Let $A$ and $B$ be square matrices. $B$ is similary to $A$ if there is an invertible matrix $Q$ such that $B=Q^{-1}AQ$ 
# Theorems
***Theorem 2.22 (The matrix representing the change in coordinates operation).*** Let $\beta$ and $\beta'$ be two ordered basis for a finite dimensional vector space $V$, and let $Q=[I_V]^{\beta}_{\beta'}$. Then:
1) $Q$ is invertible
2) For any $v \in V$, $[v]_{\beta'}$ =$Q[v]_\beta'$ 
***Theorem 2.23 (The relationship between the same linear transformations of different ordinary bases).*** Let $T: V\to V$ be a linear operator $V$ with two different ordered bases $\beta$ and $\beta'$. If $Q$ is the change in coordinate matrix that changes $\beta'$-coordinates into $\beta$-coordinates, then the same linear transformation but with different ordinary bases has the following relationship: $$[T]_{\beta'}=Q^{-1}[T]_{\beta}Q$$ 