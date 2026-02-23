---
tags:
  - "#math"
  - "#arnold_friedberg"
  - "#linear_algebra"
date_created: 2026-02-16
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
Motivated by the concept of vectors applied to experimental quantities such as velocity and distance in the previous chapter, we now treat these vectors as mathematical objects themselves that can in turn have applications beyond our initial motivations to describe quantities in physics.

In the previous chapter, we had established [8 axioms](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.1%20Introduction.md) that vectors followed to describe experimental results. We now use these axioms to formally describe the algebraic structure that will contain our vector mathematical objects
***Definition of a Vector Space (p. 6).*** A vector space $V$ over a field $F$ is consists of a set on which addition and scalar multiplication are defined so that any vectors in the set are closed under addition or scalar multiplication, that is, for any vector $x$ and $y$ and element $a$ in $F$, $x+y$  and  $ax$ produces a vector that is contained in $V$. Furthermore, the following 8 conditions are satisfied:
1) Commutativity of vector addition
2) Associativity of vector addition
3) The existence of the null vector $0x=x$ 
4) The existence of the inverse of a vector $x$ by addition denoted $-x$ 
5) The existence of the identity scalar 1
6) The associativity of scalar multiplication
7) Left distributive property of scalar-to-vector multiplication
8) Right distributive property of scalar-to-vector multiplication
It is worth emphasizing that vectors now go beyond descriptions of experimental quantities in the previous chapter and are now just elements in a vector space. 

We now spend the rest of the chapter describing important examples of vector spaces. Note that for every vector space, we have to specify two things:
1) What is the general form of the elements in the vector space, that is, what are the vectors
2) How is addition and scalar multiplication defined

The examples are as follows, and I will go into detail on specific ones:
1) The set of all $n$-tuples over any $F$ field. This set is denoted $F^n$ :
	- Vectors are $(a_1,a_2,...a_n)$ where $a_i \in F$ 
	- Vector addition defined by element-wise addition and scalar multiplication defined by scalar multiplication of each individual elemnt
2) The set of all $m\times n$ matrices with entries from the field $F$ denoted as $M_{m\times n}(F)$ 
3) The vector space of functions
	- Let $S$ be any nonempty set and $F$ be any field, thet set of all functions that maps $S$ to $F$ is a vector space if defined as follows. Vector $f$ is of the form $f(s)$ and two vectors, $f$ and $g$ are considered equal if $f(s)=g(s)$ for all $s\in S$.
	- Vector addition defined as $(f+g)(s) = f(s)+g(s)$ and scalar multiplication defined as $(cf)(s)=c[f(s)]$
4) The vector space of polynomials over field $F$ denoted $P(F)$. Essentially a subspace of the vector space of functions.
5) The vector space of sequences. Essentially an extension of the $n$-tuples.

We now state some properties of the operations between vectors and scalars in a vector space. The proof for each of these is a short application of our original 8 axioms.

***Theorem 1.1 (Cancellation Law for Vector Addition).*** If $x$, $y$, and $z$ are vectors in the vector space $V$, such that $x+z=y+z$, then $x=z$
***Corollary 1.*** The vector 0 described in axiom 3 is unique
***Corollary 2***. The inverse vector by addition is unique

***Theorem 1.2*** For any vector $x$ and scalar $a\in F$ in the vector space $V$, the following properties hold:
1) $0x=0$
2) $(-a)x=-a(x)=a(-x)$
3) $a0=0$ 


