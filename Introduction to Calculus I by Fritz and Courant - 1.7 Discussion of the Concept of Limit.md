---
tags:
  - "#math"
  - "#calculus"
  - "#richard_courant"
  - "#real_analysis"
date_created: 2026-02-21
parent: "[[Introduction to Calculus and Analysis I]]"
---
The limit is defined exactly as in Abbot's [Understanding Analysis - 2.2 The Limit of a Sequence](Understanding%20Analysis%20-%202.2%20The%20Limit%20of%20a%20Sequence.md). Courant notes that $N(\epsilon)$ is effectively a function of the chosen $\epsilon$ and as a "rule" it is an increasing function. Courant further notes the following which is just a review from[Understanding Analysis 2nd ed. - Abbot, Stephen](Understanding%20Analysis%202nd%20ed.%20-%20Abbot,%20Stephen.md):
- The limit of a sequence is unique
- A sequence that does not converge is divergent. Convergence/divergence are binary complements.
- A convergent sequence is necessarily bounded.
- The operations and addition between the limits of sequences is equivalent to the limit of the of the new sequence formed by the element-wise addition and multiplication (see [Linear Algebra by Friedberg, Insel, and Spence - 1.2 Vector Spaces](Linear%20Algebra%20by%20Friedberg,%20Insel,%20and%20Spence%20-%201.2%20Vector%20Spaces.md) for the definition of additive and scalar multiplication operations on sequences to create a vector space). This is elaborated better in [Understanding Analysis - 2.3 The Algebraic and Order Limit Theorems](Understanding%20Analysis%20-%202.3%20The%20Algebraic%20and%20Order%20Limit%20Theorems.md).
- Intrinsic tests that do not require a priori knowledge of the value of the limit:
	- A sequence that is bounded and monotone is sufficient for convergence (see [Understanding Analysis - 2.4 The Monotone Convergence Theorem and a First Look at Infinite Series](Understanding%20Analysis%20-%202.4%20The%20Monotone%20Convergence%20Theorem%20and%20a%20First%20Look%20at%20Infinite%20Series.md))
	- Cauchy's Criteria for convergence (see [Understanding Analysis - 2.6 The Cauchy Criterion](Understanding%20Analysis%20-%202.6%20The%20Cauchy%20Criterion.md))

An interesting application of concept of the limit is to the definition of $e$ and $\pi$ as a limit of a sequence. A lot of the derivations and proofs make extended use of the properties of a convergent geometric series $S_{n}$ $$\begin{align}\lim_{n \to \infty } S_{n} &=1+q+q^2+\dots q^n\\ 
& =\lim_{n \to \infty } \frac{1-q^n}{1-q} \\ 
&=\frac{1}{1-q}\text{;\quad for |q|<1}
\end{align}$$
# e. The Number $e$ as an Infinite Sum (p. 77)
We consider the definition of Euler's number as an infinite sequence: 
$$e = \lim_{ n \to \infty } S_{n}=1+\frac{1}{1!}+\frac{1}{2!}+\frac{1}{3!}+\dots+\frac{1}{n!}$$
The existence of the limit is proven by observing that $S_n$ is an increasing sequence (note we consider the series as an infinite sequence of its partial sums). and it is bounded above by the geometric series $S_n \le \sum^n_{i=1}\frac{1}{2^i}$

The expression for $e$ as an infinite sequence has computational value as we can approximate its value by partial sums $S_m$ and we can estimate the error on this partial sum again using a geometric series as an upper bound: $$\begin{align}\lim_{n \to \infty } S_{n} &=S_{m}+\frac{1}{m+1!}+\frac{1}{m+2!}+\dots+\frac{1}{n!}\\
& =S_{m}+\frac{1}{m+1!}[1+\frac{1}{m+2}+\frac{1}{(m+2)(m+3)}+\dots+\frac{1}{(m+2)(m+3)..(n)}]\\ 
&\le S_{m}+\frac{1}{m+1!}[1+\frac{1}{m+1}+\frac{1}{(m+1)^2}+\dots+\frac{1}{(m+1)^{n-m}} \\
\end{align}$$
And then noting that the geometric series converges:
$$\sum_{i=0}^{\infty}\frac{1}{(1+m)^i}=\frac{1}{1-(\frac{1}{(1+m)})}=\frac{m+1}{m}$$
We then have the estimate on the error for $S_m$: $$S_{m}\lt \lim_{ n \to \infty } S_{n}\lt S_m+\frac{1}{m}\frac{1}{m!}$$
Note that we can use this result to prove $e$ is irrational by contradiction assuming $e=\frac{p}{n}$ for $p, n \in \mathbb{I}$:$$\begin{gather}
S_{m} \lt \frac{p}{m} \lt S_{m}+\frac{1}{m}\frac{1}{m!}
\\(m!)S_{m} \lt p(m-1)! \lt (m!)S_{m}+\frac{1}{m}
\\(m!)S_{m} \lt p(m-1)!\lt (m!)S_{m}+1
\end{gather}$$
The last line states that $p(m-1)!$ lies between two successive integers which is impossible.

The author then shows how [[Equivalence Jacob Bernoulli's representation of Euler's number to Euler's representation]] is equivalent to the $S_n$ infinite series using the binomial theorem
# f. The Number $\pi$ as a Limit (p. 80)

This proof is quite a bit geometric and I leave it for later.
