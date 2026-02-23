---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#statistics"
  - "#robert_hogg"
date_created: 2026-02-15
---
The "standard" normal distribution is defined as the random variable $Z$ with the following properties: $$p(z)=\frac{1}{\sqrt{2\pi)}}exp(\frac{-z^2}{2}) \text{\quad ; \quad}M(t) = e^{t^2/2}\text{\quad ; \quad} E(Z) = 0\text{\quad ; \quad} Var(Z) = 1$$
The proof that this function is sufficient for a pdf is derived from the solution to the [Gaussian integral](Solution%20to%20the%20Gaussian%20Integral.md)
We are often more concerned with linear transformations of the normally distributed standard random variable, $X=bZ+a$. This transformed random variable has the properties
$$p(z)=\frac{1}{\sqrt{2\pi)}}exp(\frac{-\frac{1}{2}(x-a)^2}{b}) \text{\quad ; \quad}M(t) = exp(\mu t+\frac{1}{2}\sigma^2 t^2)\text{\quad ; \quad} E(X) = a\text{\quad ; \quad} Var(X) = b^2$$
Noting these properties, we refer to $X$ as a normally distributed random variable with parameter $\mu$ and $\sigma^2$ and denote it as $N(\mu,\sigma^2)$. Therefore, the standard normal distribution is $Z\sim N(0,1)$.

We note the following characteristics of the normal distribution:
1) Symmetry about $x=\mu$ 
2) the maximum of $p(x)$ is $1/\sigma \sqrt{2\pi}$ at $x=\mu$
3) The x-axis is a horizontal asymptote
4) The points of inflection are at $x= \mu \pm \sigma$ 

The chapter demonstrates the way that $P(X < x)$ is computed using complete knowledge of the solutions for the cdf of the standard normal distribution $P(Z <z)$. As $X$ is a bijective function of $Z$, $X$ can be transformed back into the standard random variable so that we [compute the probability of the known transformed random variable](Introduction%20to%20Mathematical%20Statistics%20-%201.7%20Continuous%20Random%20Variables.md). If $X = \sigma Z+\mu$ with the mean and standard deviation known, it is then equivalent to the probability of the standard random variable $Z=(X-\mu)/\sigma$: $$P(X<x) =P(\frac{(X-\mu)}{\sigma}<\frac{(x-\mu)}{\sigma}) = P(Z < \frac{(x-\mu)}{\sigma})$$
The cdf of any normally distributed random variable at a certain value can then be computed by finding the corresponding probability of the standard random variable. While this was traditionally used to compute the cdf using tables of solutions to the cdf of the standard random variable, there may be computational advantages to as we only need to know the solutions to one function as opposed to computing the solutions to infinitely many different normal distributions.

The chapter [proves a relationship](Proof%20of%20the%20transformation%20of%20a%20normally%20distributed%20random%20variable%20to%20a%20chi-squared%20distribution.md) between the normal distribution to the $\chi^2$-distribution

***Theorem 3.4.1 (Transformation of the Normal distribution to the $\chi^2$-distribution).*** If the random variable $X$ is $N(\mu,\sigma^2)$, then the transformed variable $V=(X-\mu)^2/\sigma^2$ is distributed as $\chi^2(1)$. 

The most important property of the normal distributions is that a linear combination of independent normally distributed random variables is itself a normal distribution. This is a distinction from the Poisson distribution and the Binomial distribution which do not allow for general linear combinations to retain their original distribution.

***Theorem 3.4.2.*** Let $X_1, X_2, ..., X_n$ be independent random variables with the corresponding normal distribution $N(\mu_i, \sigma^2_i)$ for each $X_i$. The random variable $Y=\Sigma^{n}_{i=1}a_iX_i$ where $a_i \in \mathbb{R}$, will then have the normal distribution $N(\Sigma^{n}_{i=1}a_i\mu_i,\Sigma^{n}_{i=1}a_i^2X_i)$ 

It can be shown from this theorem as a corollary that the sample average of independent $X\sim N(\mu, \sigma^2)$ random variable (i.e. $\bar{X} =\frac{1}{n}\Sigma^{n}_{i=1}X_i$)  is normally distributed $N(\mu, \sigma^2/n)$ 