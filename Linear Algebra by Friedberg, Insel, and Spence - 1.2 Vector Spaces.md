---
tags:
  - "#math"
  - "#arnold_friedberg"
  - "#linear_algebra"
date_created: 2026-02-16
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
We were motivated by physical quantities to describe vectors in [1.1 Introduction](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.1%20Introduction.md), but now we treat them strictly as mathematical objects (and these objects can describe more than just physical quantities which we will show in this section). We look at vectors as elements belonging to an algebraic structure called the vector space:

***Definition (Vector Space)***. A vector space (or linear space) $V$ over a field $F$, consists of a set where two operations (addition and scalar multiplication) are defined so that for any pair of elements $x$ and $y$ in $V$ and an element $a$ in $F$  
- $x+y$ results in a unique vector that is also contained in $V$ (closed under addition)
- $ax$ is contained in $V$ (closed under scalar multiplication)
As well, the following axioms holds for the elements in $V$:
1) Commutativity of addition
2) Associativity of addition
3) Existence of the null vector such that $x+0 = x$ 
4) Existence of inverse elements of addition.
5) Existence of the identity scalar
6) Compatibility of scalar multiplication
7) Distributivity with respect to vector addition
8) Distributivity with respect to field addition
It must be stressed that vectors are now treated strictly as mathematical objects: elements of a vector space. 

The remainder of this will introduce several examples of important vector spaces and show how a vector space is defined. The following must be stated to describe the vector space:
- The field that the vector space extends over
- How addition and scalar multiplication operations are defined to comply with our 8 axioms

1) The set of all $n$-tuples
2) The set of $m\times n$ Matrices
3) The set of functions $\mathbb{F}(S,F)$ that map a nonempty set $S$ to a field $F$. For any functions $f$ and $g$ in $\mathbb{F}(S,F)$ and an element $s\in S$ 
	- $f$ is equal to $g$ if $f(s)=g(s)$ for all $s \in S$
	- $(f+g)(s) = f(s)+g(s)$             (definition of addition)
	- $(cf)(s) = c[f(s)]$             (definition of scalar multiplication)
4) A subset of 3), but the set of all polynomials of degree $n \in \mathbb{N}$ with coefficients from a field $F$.
5) A sequence in $F$ is a function $\sigma$ that maps the positive integers to $F$: $\sigma(n) = a_n$ where $n\in \mathbb{N}$ and $a_n \in F$. For brevity, we denote such a sequence $(a_n)$. The vector space that contains all $(a_n)$ sequences in $F$, given any two sequences $(a_n)$ and $(b_n)$
	- $(a_n)+(b_n) = (a_n+b_n)$  (addition defined)
	- $t(a_n)=(ta_{n})$                  (scalar multiplication defined)

We conclude with a few elementary consequences of vector space axioms:
- The 0 vector is unique (proof in exercise).
- The inverse vector of $x \in V$ described in axiom 4) is unique (proof in exercise). This vector is called the additive inverse and is denoted $-x$ 

***Theorem 1.1. (Cancellation Law for Vector Addition).*** If $x,y,z$ are vectors in the vector space $V$ such that $x+z = y+z$, then $x=y$. 

The proof of this is short and follows from axioms 2), 3), and 4).

***Theorem 1.2 (Collection of other properties)*** Given any vector space $V$ over a given field $F$, $x \in V$ and $a \in F$:
1) $0x =0$ for each $x\in V$
2) $(-a)x=a(-x)= -(ax)$
3) $a0 = 0$ 

	
