---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-03-30
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
Chapter 3.3 was about uniqueness and existence of a solution to a system of linear equations using its rank and if a solution exists, what general form does it have. Now we look at determining what that solution is:
1) Method to determine a solution by a linear transformation to an easier form that preserves the solution set. The linear transformation to be used are elementary row operations.
2) The goal of 1) is to obtain an easier form to solve the equation. This final form is called the reduced row echelon form.
3) What the row reduced echelon form of the augmented matrix tells us about the original matrix
4) What does the rank of a matrix tell us about the row reduced echelon form of the matrix.

The goal of Gaussian elimination is to obtain the row reduced echelon form and the theorems in this chapter provide the justification for why Gaussian Elimination is justified:
1) Gaussian elimination obtains the row reduced echelon form as formalized in ***Theorem 3.14*** which makes it easier for us to compute the general solution which is of the form in ***Theorem 3.15***.
2) Gaussian elimination is a a series of elementary row operations that preserves the solution set as matrix multiplication by an invertible matrix preserves the solution set as formalized in ***Corollary to Theorem 3.13.***
3) The row reduced echelon form is unique as stated in ***Corollary to 3.16.*** so the sequence of operations we perform to obtain it does not matter.

As well as providing us the solution set, the row reduced echelon form tells us something more general about the original system $Ax=b$ :
4) Obtaining the row reduced echelon form lets us determine the rank of $A$  as stated in ***Theorem 3.15.***
5) The row reduced echelon form lets us determine which columns of $A$ are linearly independent as stated in ***Theorem 3.16.***
To expound on 5), we also have conversely that if we know $rank(A)$ then we can determine the rank of the augmented row reduced echelon form and the number of standard basis vectors it should have ($r$ of them).

# Definitions
***Definition (Equivalent).*** Two systems of linear equations are called equivalent if they have the same set of solutions.

***Definition (Reduced Row Echelon Form).*** A matrix is said to be in reduced row echelon firm if the following three conditions are satisfied
1) Any row containing nonzero entries precedes any row in which all the entries are 0 (if any)
2) The first nonzero entry in each row is the only non zero entry in its column
3) The first nonzero entry in each row is 1 and it occurs in a column to the right of the first nonzero entry of the preceding row

# Theorems
***Theorem 3.13 (Preservation of system solutions by an isomorphism).*** Let $Ax=b$ be a system of $m$ linear equations with $n$ unknowns and let $C$ be an invertible matrix. Then the system $(CA)x=Cb$ has the same solution set as $Ax=b$ 

***Corollary to Theorem 3.16.*** A matrix $B$ obtained from $A$ by elementary row operations will have a system $Bx=b$ that is equivalent to $Ax=b$.

***Theorem 3.14.*** Gaussian elimination transforms any matrix into its reduced row echelon form.

***Theorem 3.15 (The general solution to the system of equations and the rank of the system).*** Let $Ax=b$ be a system $r$ nonzero equations in $n$ unknowns. Suppose $rank(A)=rank(A|b)$ and that $(A|b)$ is in reduced echelon form. Then we can deduce the following properties:
- $rank(A)=r$
- The general solution is of the form $s = s_0 +t_1u_1+t_2u_2+...+t_{n-r}u_{n-r}$ where $\{u_1,...u_{n-r}\}$ are the solution set of the homogenous system and $s_0$ is the solution to the original system that does not solve the homogenous system. 
***Theorem 3.16 (What the rank tells us about the reduced row echelon form).*** Let $A$ be a $m\times n$ matrix of rank $r$, where $r>0$, and let $B$ be the reduced row echelon form of $A$. Then from the rank of $A$, we can deduce the following:
- The number of nonzero rows in $B$ is $r$
- for each $i=1,2,...,r$ there are $r$ number of  $e_i$ standard basis vectors in $B$
- The columns of $A$ numbered $j_1,j_2,...,j_r$ are linearly independent
- For each $k = 1,2,...,n$ if column $k$ of $B$ is $d_1e_1+d_2e_2+...+d_re_r$, then column k of $A$ is $d_1a_{j1}+d_2a_{j2}+..+d_ra_{jr}$ 

