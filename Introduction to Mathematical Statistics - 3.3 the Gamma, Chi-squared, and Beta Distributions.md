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
Suppose we wanted to determine the probability that a device will fail at a certain time, $x$. We want to find the pdf, $f(x)$ and cdf, $F(x)$, of a random variable $X$ that maps the failure to the real number time of failure. We look at this in terms of differential equations by looking at the rate of failure, $r(x)$ at time $x$:
$$r(x) = lim_{\delta \to \infty}\frac{P(x<X<x+\delta|X\ge x)}{\delta}$$
$r(x)$ is referred to as the hazard function and by the definition of conditional probabilities, this is simply

$$r(x) = \frac{1}{1-F(x)}lim_{\delta \to \infty}\frac{P(x<X<x+\delta}{\delta}$$
$$r(x) =\frac{f(x)}{1-F(x)}$$
Solving this differential equation yields:
$$1-F(x)=e^{-\int r(x)dx +c}$$
If the hazard rate is simply a constant $r(x)=1/\beta$, then the pdf is simply a $\Gamma(1,\beta)$ distribution.

The gamma function also occurs in Poisson processes. The Poisson random variable, $X_t$, denotes the number of events in our $(0,t]$ interval of interest. We now try to determine the inverse: the amount of time, $w$, until the $k$th event occurs. This random variable is denoted as $W_k$. We then note that the probability that $W_k >w$ if and only if the we only have $k-1$ events occur in the $(0,w]$ time interval, or in other words:
$$P(W_k>w) = P(X_w\le k-1)=\Sigma_{x=0}^{k-1}\frac{(\lambda w)^{-x}e^{-\lambda w}}{x!}$$
It can then be proved (exercise 3.3.5) that this is precisely the $\Gamma(\alpha = k, \beta = 1/\lambda)$ distribution
# $\chi^2$-distribution
This is a brief section as the $\chi^2$-distribution is a special case of the gamma function with $\alpha = r/2$ for a positive integer $r$ that is called the degrees of freedom and $\beta=2$

$$\chi^2(x) = \Gamma(r/2,2)$$
This distribution has the following properties:
- $M(t) = (1-2t)^{-r/2}$ , for $t<1/2$
- $\mu = r$
- $\sigma^2 = 2r$
Usually for brevity, the $\chi^2$-distribution with $r$ degrees of freedom is written as $\chi^2(r)$

The following result is used a lot:
***Theorem 3.3.2 (Moments of a $\chi^2$-distribution).*** Let $X$ have a $\chi^2(r)$ distribution. If $k>-r/2$, then $E(X^k)$ exists and is given by:
$$E(X^k)=\frac{2^k\Gamma(r/2+k)}{\Gamma(r/2)}$$
# The $\beta$-distribution






