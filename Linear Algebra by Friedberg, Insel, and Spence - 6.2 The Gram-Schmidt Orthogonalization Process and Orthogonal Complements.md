---
tags:
  - math
  - linear_algebra
  - arnold_friedberg
date_created: 2026-05-03
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
Using the inner product space defined in the previous chapter, we now relate them to orthogonal and orthonormal sets and deduce their significance to general vectors in an inner product space. The chapter is outlined as follows:
1) Determination of the coefficients of a vector that is in the span of a orthogonal subset of a vector space:
	- Orthogonality implies linear independence. Converse is not necessarily true
2) The Gram-Schmidt Process that constructs a orthogonal or orthonormal set of vectors with the same span as a set of linearly independent vectors.
	- Any finite dimensional vector space has a orthogonal basis.
3) General form of the coefficients of a vector in a vector space in terms of an orthogonal basis.


# Summary and important notes
- Linear independence does not imply orthogonality but the converse is true. See corollary to ***Theorem 6.3)
- Infinite dimensional vector do not necessarily have a orthogonal basis but finite ones do.

# Definition
***Definition (Orthonormal Basis).***

***Definition (Fourier coefficients).*** Let $\beta$ be an orthonormal basis to $V$. Then the Fourier coefficients of a vector $x\in V$ relative to an orthonormal basis $\beta$ is defined as the coefficients $\langle x, y \rangle$ for each $y\in \beta$.

***Definition (Orthogonal complement).*** Let $S$ be non-empty subset in a vector space $V$. The set of all vectors orthogonal to $S$ is called the orthogonal complement of $S$ and is denoted $S^{\perp}$. Namely $S^{\perp}=\{x\in V: \langle x, y \rangle = 0, \forall y \in S\}$ 

# Theorems
***Theorem 6.3 (Expansion of a vector in terms of orthogonal vectors).*** Let $V$ be an inner product space with an orthogonal non-zero subset $S=\{v_1,...,v_n\}$. A vector $y \in span\{S\}$ can then be expressed as a linear combination of the orthogonal subset in the following form: $$y=\sum_{i=1}^n\frac{\langle y, v_{i}\rangle}{||v_{i}||^2}v_{i}$$

***Corollary 1 to Theorem 6.3 (Vector expressed as the linear combination of orthonormal vectors).*** If $S$ is an orthonormal set, then the expression for a general vector in the span of the orthonormal set is simplified as $||v_i||=1$ 

***Corollary 2 to Theorem 6.3 (Orthogonal vectors are linearly independent).*** Let $V$ be an inner product space and $S$ be an orthogonal subset of $V$ with non-zero vectors, then $S$ consists of independent vectors.

***Theorem 6.4 (The Gram-Schmidt process. Transformation of a linearly independent set into an orthogonal set that has the same span).***

***Theorem 6.5 (Existence of an orthonormal basis and the form of the vector expressed as a linear combination of an orthonormal basis).*** Let $V$ be a inner product space with a orthonormal basis $\{v_1,...v_n\}$. Any vector $x\in V$ can then be expressed as a linear combination of the orthogonal basis in the following expression: $$x = \sum_{i=1}^{n}\langle x, v_i \rangle v_i$$ 

***Corollary to Theorem 6.5 (The form of the linear combination of a transformation of a vector that stays in the vector space of the domain).*** Let $V$ be an inner product space with an orthonormal basis $\{v_1,...v_n\}$ and $T: V\to V$ be a linear transformation that stays in the domain. Then the transformation $T(x)$ of a vector $x \in V$ can be expressed as a linear combination of the orthonormal basis as follows: $$T(x) = \sum_{i=1}^{n}\langle T(x), v_i \rangle v_i$$

***Theorem 6.6 (The possibility to decompose a vector into orthogonal components from any general subspace and its orthogonal complement).*** Let $W$ be a subspace of a finite dimensional inner product space $V$. For any general vector $y \in V$, the vector $y$ can be expressed as a sum $y= u +z$ with $u \in W$ and $z \in W^{\perp}$. Furthermore, if the subspace $W$ has an orthonormal basis $\{v_1,..,v_n\}$ then the Fourier coefficients of $u$ can be determined as follows: $$u=\sum_{i=1}^n \langle y, v_i \rangle v_i$$

***Corollary to Theorem 6.6 (The orthogonal projection of a vector as the best approximation of the vector in terms of vectors from a specific subspace).***

***Theorem 6.7 (The Steinitz exchange lemma for orthonormal vectors).***