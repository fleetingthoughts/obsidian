---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.2 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-26
---
Prove: the matrix $A$ is similar to an upper triangular matrix if and only if the characteristic polynomial of $A$ splits.
#### Notes
**Skeleton Proof:**

**Forward Direction ($\Rightarrow$):**
1. **Assume:** $A$ is similar to an upper triangular matrix $U$. Therefore, there exists an invertible matrix $Q$ such that $A = Q U Q^{-1}$.
2. **Similarity Property:** Similar matrices share the same characteristic polynomial, meaning $f_A(t) = f_U(t) = \det(U - tI)$.
3. **Evaluate Determinant:** Because $U$ is upper triangular, $U - tI$ is also upper triangular. The determinant of an upper triangular matrix is simply the product of its diagonal entries: $f_A(t) = \prod_{i=1}^n (U_{ii} - t)$.
4. **Conclude:** Because the characteristic polynomial can be written entirely as a product of linear factors, it splits over $F$.

**Reverse Direction ($\Leftarrow$):**
*(This direction relies on mathematical induction on the dimension $n$.)*
1. **Base Case:** For $n=1$, every $1 \times 1$ matrix is trivially upper triangular. Assume the theorem holds for dimension $n-1$.
2. **Extract Eigenvector:** Assume the characteristic polynomial of $A$ splits. This guarantees $A$ has at least one root (eigenvalue) $\lambda_1$ and a corresponding eigenvector $v_1$.
3. **Change of Basis:** Extend $\{v_1\}$ to form a complete basis for $F^n$. The matrix representation of the transformation in this new basis takes the block form $M = \begin{pmatrix} \lambda_1 & * \\ 0 & B \end{pmatrix}$, where $B$ is an $(n-1) \times (n-1)$ matrix.
4. **Evaluate Sub-Matrix:** The characteristic polynomial of $M$ is $f_M(t) = (\lambda_1 - t) f_B(t)$. Since $A$ and $M$ are similar, $f_M(t)$ splits, which forces $f_B(t)$ to also split. 
5. **Apply Induction & Conclude:** By the inductive hypothesis, because $f_B(t)$ splits, $B$ is similar to an upper triangular matrix $U'$. Lifting the similarity transformation of $B$ back to the full $n \times n$ space proves $A$ is similar to an upper triangular matrix.
<!--SR:!fsrs,2026-10-01T03:23:15.429Z,0,2.3065,2.11810397,1,1,0,1,2026-10-01T03:13:15.429Z-->

Proof of the converse:
- Proceed by mathematical induction on $n$.
- For the general case, the splitting polynomial guarantees at least one eigenvalue; let $v_1$ be an eigenvector of $A$.
- Extend $\{v_1\}$ to a basis $\{v_1, v_2, \dots, v_n\}$ for $F^n$.
- Let $P$ be the $n \times n$ matrix whose $j$th column is $v_j$, and consider the similarity transformation $P^{-1} A P$.
- This transformation yields a block matrix with the eigenvalue in the top-left and an $(n-1) \times (n-1)$ block in the lower-right; apply the inductive hypothesis to this smaller block to complete the upper-triangularization of $A$.

