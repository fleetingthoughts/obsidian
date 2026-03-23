---
tags:
  - "#math"
  - "#linear_algebra"
  - arnold_friedberg
date_created: 2026-03-14
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
In 2.2, we had demonstrated how the representation of linear transformations by matrices can describe the sum of two different transformations of a vector. We now discuss the representation of a composition of linear transformations which leads to a definition of matrix multiplication to represent it. Throughout this chapter $V$, $Z$, and $W$ will be vector spaces over $F$ and $T V\to W$ will be linear transformations $T$ and $U$ that take vector in $V$ to vectors in $W$.

We first propose the reason why we're interested in the representation of a composition of linear transformations. To denote a composition of linear transformations, say the transformation by $T$ first and then taking the resulting image and transforming it with $U$ is represented as $U(T(x))$. As ***Theorem 2.9 (Linearity of composition of linear transformations)*** demonstrates, this composition is itself linear which motivates us to find some operation between the component matrices that results in the final compositional matrix. We also show in ***Theorem 2.10*** that a composition of matrix have the following properties in common with the usual algebraic operations of real numbers:
- Right and left distributive properties
- Associativity of transformations
- Existence of multiplicative identity
- Commutativity and associativity of scalar multiplication
Notice that we do not have commutativity between linear transformations. 

The fact that compositions of linear functions are themselves linear transformations means we can be motivated to represent compositions with a matrix derived from the composite matrices. W<u>e define a form of matrix multiplication specifically so that composition of linear transformations result in a linear transformation that can be derived by their matrix multiplication</u> as derived in ***Theorem 2.11.*** In defining matrix multiplication this way, we satisfy all the properties of linear transformations derived in ***Theorem 2.9***:
- 
- ***Theorem 2.16***: Associativity of matrix multiplication


# Definitions
- Left multiplication matrix denoted $L_A:F^n \to F^m$ where $L_A$ has a $m \times n$ matrix representation. 
# Theorems
- ***Theorem 2.9 (The linearity of composition of linear transformations).*** Given a linear transformation $T:V \to W$, and $U: W \to Z$ , the transformation $UT:V \to Z$ is linear
- ***Theorem 2.10 (Properties of compositions of linear transformations). Given $T, U_1, U_2 \in \mathcal{L}(V)$. Then we have the following properties
	1) Right and left distributive properties:  $T(U_1+U_2)=TU_1+tU_2$ and $(U_1+U_2)T = U_1T+U_2T$. (Notice that we do not imply commutativity here
	2) Associative properties: $T(U_1U_2)=(TU_1)U_2$ 
	3) Existence of the identity: $TI=IT=T$
	4) Commutativity and associativity of scalar multiplication: $a(U_1U_2)=(aU_1)U_2=U_1(aU_2)$ 
- ***Theorem 2.11 (Derivation of the matrix representing the composition of linear transformations by the definition of matrix multiplication).*** Let $\alpha, \beta, \gamma$ be the ordered bases for $V, W, Z$ respectively and let $T:V \to W$ and $U: W\to Z$. Then the resulting composition $UT: V\to Z$ is represented by matrix multiplication: $[UT]^{\gamma}_{\alpha}=[U]^{\gamma}_{\beta}[T]^{\beta}_{\alpha}$
- ***Theorem 2.13 (Determination of the columns of a composition of linear transformations).*** Let $A$ be a $m\times n$ matrix and $B$ be a $n \times p$ matrix. let $u_j$ and $v_j$ denote the $j$th column of $AB$ and $B$ respectively:
	1) Determination of a column of $AB$: the column $u_j=Av_j$
	2) $v_j=Be_{j}$ where $e_j$ is the $jth$ standard vector of $F^p$  

- ***Theorem 2.14 (Representation of the transformation of a vector by matrix multiplication).*** Given a linear transformation $T: V\to W$, such that for any $v\in V$ we have $T(v) = w \in W$. If $\beta$ and $\gamma$ are the ordered basis, then we have the matrix multiplication
$$[w]_{\gamma}=[T(v)]_{\gamma}=[T]_{\beta}^{\gamma}[u]_{\beta}$$ 