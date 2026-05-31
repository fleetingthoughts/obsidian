---
tags:
  - math
  - real_analysis
  - richard_courant
date_created: 2026-04-08
parent: "[[Introduction to Calculus and Analysis I]]"
---
1) Order of magnitude as a relation between two functions to compare speed of growth as the variable $x$ tends to a value or infinity.
2) A measure of this order of magnitude is the limit of the ratio between the two functions.
3) The folly of trying to standardize the order of magnitude of a function relative to polynomials for there exists functions that are beyond all such measures: 
	1) The exponential function $a^x$  with $a> 1$ is of higher order than $x$ as $x\to \infty$. 
	2) The exponential function $a^x$ with $a>1$ is of higher order than any power of $x$.
	3) The logarithm is of lower order than any arbitrarily small positive power of $x$.
4) The limit for the order of magnitude can be defined in 2 different ways:
	1) Limit as $x$ goes unbounded:  $x \to \infty$
	2) Limit as we tend to, typically, an asymptotic point $x\to x_o$
5) We use the big "O" and little "o" notation to describe the order of magnitude relation between two functions $f(x)$ and $g(x)$:
	1) $f=o(g)$ means $f$ grows at a <u>lower order of magnitude</u> than $g$. In other words, the quotient $f/g$ for our limit if interest in 4) is 0.
	2) $f=O(g)$ means $f$ grows at the same order of magnitude than $g$. In other words, the limit of the quotient $f/g$ tends to a finite number that is bounded.
