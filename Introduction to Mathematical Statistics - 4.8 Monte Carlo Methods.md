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

***Theorem 4.8.1 (Inverse Transform Sampling: Use of a random number generator to determine the distribution). If U is a uniform random distribution (that is $P(U<u)=u$ for $u \in (0,1)$ ), then assuming our random variable of interest has the cdf $F(x)$, the distribution of X can be determined by $X=F^{-1}(U)$ which has a distribution of $F(x)$.

Theorem 4.8.1 gives us an algorithm to generate a realization of any distribution we want:
1) $X$ has a certain distribution $F(x)$
2) use a uniform random number to generate realization of $U$ such as $u_1,...u_n$
3) apply the inverse of $F(x)$ to each realization to obtain our desired distribution. Applying $F^{-1}(u_1),...,F^{-1}(u_n)$ produces the realization $x_1,...x_n$ with an $F(x)$ distribution.

The Inverse transform sampling is also applied to approximation of integrals. Any integral can be written as $$\int_{a}^{b}g(x)dx=(b-a)\int_{a}^{b}g(x)\frac{1}{b-a}=(b-a)E[g(X)]$$
What this implies is that we seek the expectation of a transformation of a uniform random variable with the distribution $f_x(X)=\frac{1}{b-a}$. This gives us our target distribution that we generate realized samples with the Monte Carlo method. We can then use these realized estimates to compute the expectation of the transformation. Here Theorem 4.8.1 is applied to 
- use a random number generator $f_U(U)=1$ for $u \in (0,1)$
- Apply $F^{-1}_x(U)=(b-a)U$ producing our realized samples of $x_1,...x_n$ with a new uniform distribution.
- Apply the fact that the average is an unbiased estimator of the expectation: Use the average of the transformation of these realized samples $g(x_1),...,g(x_n)$ which gives us an unbiased estimator of $E(g(X))$ 

Note that the Monte Carlo method so far described is contingent on us being able to determine the inverse of the desired cdf from which we wish to generate realized samples. If we know the pdf, but the cdf is not obtainable in closed form for us to develop an inverse we apply an algorthm that requires a few things. First we'll need:
- a target distribution with a known pdf $f(x)$ from which we cannot compute a cdf in closed form.
- a uniform(0,1) random number generator
- a known distribution $g(Y)$ that we can easily compute the CDF for so that we can generate it by applying the Inverse Transform Sampling theorem such that it bounds our target pdf:$$f(x)\le Mg(x)\text{\quad}-\infty<x<\infty$$
then we can apply the following algorithm:
***The Accept-Rject Algorithm. Let $f(x)$ be the desired pdf. Suppose that $Y$ is a random variable with pdf $g(y)$ with cdf we can compute in closed form, $U$ is a random variable with the distribution $uniform(0,1)$ that is independent of $Y$. The following algorithm generates realized samples of the distribution $f(x)$:
1) Generate $Y$ and $U$
2) If $U \le \frac{f(Y)}{Mg(Y)}$ then let $X=Y$ be our realized sample. Discard otherwise and repeat step 1)
3) Every $X$ generated this way will have the distribution $f(x)$ 
A couple things to note:
- The probability of acceptance of a realized sample $X=Y$ is $\frac{1}{M}$ so to make our algorithm as efficient as possible we need the smallest bound.
- Constants in a pdf of our target $f(x)$ and $g(y)$ can be ignored for it gets subsumed in our bound $M$.
