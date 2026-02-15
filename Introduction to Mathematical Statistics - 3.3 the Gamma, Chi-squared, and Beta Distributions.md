---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#statistics"
  - "#robert_hogg"
date_created: 2026-02-14
---
We discuss 3 related functions:
1) The $\Gamma$ - function
2) The $\chi^2$-function
3) The $\beta$ - function
# The Gamma function
We discuss some of the mathematical properties of the gamma function:
- its factorial-like property
- the mean and its variance
But then we also discuss its applications and how it arises in some basic questions about failure and time until certain event occurs:
- The Hazard function: when something can be expected to fail given a certain elapse in time
- Waiting time in a Poisson Process: probability in the time one must wait until $k$th event occurs given a Poisson process
- The special case of the $\Gamma$-function, $\Gamma(r/2)$ with the parameter $\beta=2$ called the $\chi^2$ -function
- The $\beta$-distribution derived from the $\Gamma$-distribution and its generalization to multiple variables called the Dirichlet distribution

The gamma function is a function of $\alpha$, and is defined by
$$\Gamma(\alpha)=\int_0^{\infty}y^{\alpha-1}e^{-y}dy$$
The integral must exist for $\alpha > 1$ and in the base case $\Gamma(1)=1$. 

An interesting property of the $\Gamma$-function is that it is solved by parts and behaves like a factorial

$$\Gamma(\alpha)=\int_0^{\infty}y^{\alpha-2}e^{-y}dy=(\alpha-1)\Gamma(\alpha-1)$$
This integration by part continues until we arrive at the "base case" $\Gamma(1)=1$ and so for positive integers greater than 1:
$$\Gamma(\alpha)=(\alpha-1)!$$
This relationship gives us a reason to suggest that $0!=1$ and lets us extend factorials to real numbers. 

The $\Gamma$-function is a part of the $\Gamma$-distribution that has two parameters $(\alpha,\beta)$. A random variable, $X$ has a $\Gamma(\alpha,\beta)$ distribution if its pdf is the following for
$$f(x) = \int_0^{\infty}\frac{1}{\Gamma(\alpha)\beta^{\alpha}}x^{\alpha-1}e^{\frac{-x}{\beta}}$$
The support of this pdf is on $(0,\infty)$. This function has the following parameters worth noting:

1) $\mu=\alpha\beta$
2) $\sigma^2=\alpha\beta^2$
3) The moment generating function is as follows:$$M(t)=\frac{1}{(1-\beta t)^{\alpha}}$$for $t<\frac{1}{\beta}$
And as with so many other functions, the linear combination of independent random variables will result in another gamma function:
***Theorem 3.3.1 (Linear combination of independent random variables with a $\Gamma$-distribution).*** Given a set of random variables, $X_i$, with a $\Gamma(\alpha_i,\beta)$ distribution (i.e. identical $\beta$ but different $\alpha$), if $Y =\Sigma^n_{i=1}X_i$ , then $Y$ has a $\Gamma(\Sigma^n_{i=1}\alpha_i,\beta)$ distribution.
# Cases where the $\Gamma$-distribution arises




