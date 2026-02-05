---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#statistics"
  - "#robert_hogg"
date_created: 2026-01-16
---
This chapter is a miscellaneous chapter that can be treated as an "appendix", but it will be a collection of inequalities (mathematical tools) that are applicable to statistics

We will first prove a theorem that establishes the existence of momentum-generating function once we establish the existence of a different one

***Theorem 1.10.1 (Existence of momentum-generating function)***. Let $X$ be a random variable and $m$ be a positive integer. If $E[X^m]$ exists, then for $k \le m$, $E[X^k]$ exists as well.

The proof is for the continuous case but is analagous to the discrete case. Note that theorem 1.10.1 implies that if a random variable has a finite variance, then its mean exists as well.

***Theorem 1.10.2 (Markov's Inequality).*** Let $u(X)$ be a nonnegative function of the random variable $X$. If $E[u(X)]$ exists, then for every positive constant $c$.
$$P[u(X) \ge c] \le \frac{E[u(X)]}{c}$$ 
The Markhov's inequality is a generalized form of the frequently used Chebyshev's Inequality

***Theorem 1.10.3 (Chebyshev's Inequality).*** Let $X$ be a random variable with finite variance, $\sigma ^2$  (therefore its mean $\mu$ exists as well by Theorem 1.10.1). Then for every $k \gt 0$.
$$P(|X-\mu| \gt k\sigma) \lt \frac{1}{k^2}$$
or equivalently
$$P(|X-\mu| \lt k\sigma) \gt 1- \frac{1}{k^2}$$
We will next discuss an inequality involving convex functions, but first, we define convex functions and establish some of their properties.

***Definition 1.10.1 (Definition of Convex Functions).*** A function $f$ defined on an interval $[a,b]$ is said to be convex if for all $x, y$ in $[a,b]$, and for $0 \lt \gamma \lt 1$:
$$f[\gamma x+ (1- \gamma)y] \lt \gamma f(x) + (1-\gamma) f(y)$$ Depending on the existence of the first and second derivatives of the function $f$, the following properties of the convexity of $f$ can be proved:
***Theorem 1.10.4. (Convexity Properties).***