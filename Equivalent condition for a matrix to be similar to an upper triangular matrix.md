---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: the matrix $A$ is similar to an upper triangular matrix if and only if the characteristic polynomial of $A$ splits.
#### Notes
Proof that if the characteristic polynomial splits, then it is similar to an upper triangular matrix:
- By hypothesis, there exists an invertible matrix $Q$ and an upper triangular matrix $U$ such that $A = Q U Q^{-1}$.
- Similar matrices share identical characteristic polynomials.
- The characteristic polynomial of the upper triangular matrix $U$ is the product of its diagonal linear factors $(u_{ii} - t)$.
- Therefore, the characteristic polynomial of $A$ consists solely of linear factors, establishing that it splits.

Proof of the converse:
- Proceed by mathematical induction on $n$.
- For the general case, the splitting polynomial guarantees at least one eigenvalue; let $v_1$ be an eigenvector of $A$.
- Extend $\{v_1\}$ to a basis $\{v_1, v_2, \dots, v_n\}$ for $F^n$.
- Let $P$ be the $n \times n$ matrix whose $j$th column is $v_j$, and consider the similarity transformation $P^{-1} A P$.
- This transformation yields a block matrix with the eigenvalue in the top-left and an $(n-1) \times (n-1)$ block in the lower-right; apply the inductive hypothesis to this smaller block to complete the upper-triangularization of $A$.

