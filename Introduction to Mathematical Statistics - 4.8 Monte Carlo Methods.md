---
tags:
  - math
  - statistics
  - robert_hogg
date_created: 2026-03-13
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---

The process of generating observations from a specified distribution or sample is referred to as the Monte Carlo methods. The method has received importance in modern statistics in the realm of inference due to developments in the following:
- Bootstrap resampling
- Modern Bayesian methods
The Monte Carlo method is usually demonstrated with discrete methods, but in continuous methods, a uniform random number generator is usually used. This requires a mechanism that actually generates a uniform distribution which has made developments. The use of a uniform random number generator, $U$  to determine the distribution of the random variable of interest, $X$ depends on the following theorem

***Theorem 4.8.1 (Use of a random number generator to determine the distribution). If U is a uniform random distribution (that is $P(U<u)=u$ for $u \in (0,1)$ ), then assuming our random variable of interest has the cdf $F(x)$, the distribution of X can be determined by $X=F^{-1}(U)$ which has a distribution of $F(x)$.

Theorem 4.8.1 gives us an algorithm to generate a realization of any distribution we want:
1) $X$ has a certain distribution $F(x)$
2) use a uniform random number to generate realization of $U$ such as $u_1,...u_n$
3) apply the inverse of $F(x)$ to each realization to obtain our desired distribution. Applying $F^{-1}(u_1),...,F^{-1}(u_n)$ produces the realization $x_1,...x_n$ with an $F(x)$ distribution.