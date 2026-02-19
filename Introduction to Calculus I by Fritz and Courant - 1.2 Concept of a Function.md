---
tags:
  - "#math"
  - "#richard_courant"
  - "#real_analysis"
  - "#calculus"
date_created: 2026-02-17
parent: "[[Introduction to Calculus and Analysis I]]"
---
A review of some fundamentals for real analysis. The relevant concepts that this chapter goes over:
- monotonic functions and one-to-one mapping
- Even functions $f(-x)=f(x)$
- Odd Functions: $f(-x)=-f(x)$

***Continuity of a Univariate Function (p.33)*** The function $f(x)$ is continuous at $f(x_o)$ if for any arbitrary $\epsilon >0$, there exists a $\delta >0$ such that:
$$|f(x)-f(x_o)|<\epsilon \text{\quad when\quad}|x-x_o|<\delta$$
Continuity can be thought of in terms of a neighborhood of a point as follows: for any arbitrary $\epsilon$-neighborhood $J$ of point $y_0=f(x_0)$ (i.e. the interval $(y_o-\epsilon, y_o+\epsilon)$), we can find a $\delta$-neighborhood of $x$ that $J$ maps to. Note that the reverse mapping is not necessarily true. We cannot find a $\delta$ 

The author goes through examples to prove the continuity of a function. In general, the strategy will be to describe an upper bound or equality of the function in terms of $|x-x_o|$. 

The $\delta$ in the definition of continuity is referred to as the "modulus of continuity", and we define different types of continuity on the way way $\delta$ changes with $\epsilon$.

***Definition of Uniformly Continuous (p.41).***
	- Uniformly continuous and uniform modulus of continuity.
	- Lipschitz-Continuous
	- Holder Continuous
- Intermediate Value Theorem
- Conditions for the continuity of inverse functions

Monotonic functions always have a one-to-one mapping. 

Vague expressions like "arbitrarily small" are now replaced with more specific formulations like "for any positive value".
