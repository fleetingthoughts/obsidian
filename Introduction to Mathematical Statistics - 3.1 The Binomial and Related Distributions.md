---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#statistics"
  - "#robert_hogg"
date_created: 2026-02-13
---
We explain 3 distributions related to the Bernoulli l distribution and demonstrate their mean and variance. Its important to distinguish the <u>Bernoulli distribution</u> from the <u>Binomial distribution</u>. I often get the terms mixed up but the Binomial distribution is derived from the Bernoulli distribution. We first begin with the Bernoulli distribution.

The Bernoulli random variable maps a Bernoulli trial that views an event as either a success or a failure. The Bernoulli Random variable, $X$, maps success to the real number 1 and failure to the real number 0, so the Bernoulli random variable is a discrete random variable with two numbers in its support. If the probability of a success occurring is $p$, then the pmf is:
$$p(x) = p^x(1-p)^{1-x}$$ It can then be shown the expectation is $p$ and the variance is $p(1-p)$. Using this distribution, we can then look at the sequence of Bernoulli trials:
1) Binomial random variable: $X =$ total # of successes in $n$ Bernoulli trials. Requires the parameter $n$ (1 parameter)
2) Negative Binomial Random Variable: $Y$ = total # of failures before the $r$th success (i.e. x+r-1 trials since the last trial has to be a fixed success). Note that although it technically has two variables, the # of successes is treated as a fixed parameter. (1 parameter)
$$p_{Y}(y)=\binom{y+r-1}{r-1}p^r(1-p)^{y}= \binom{y+r-1}{y}p^r(1-p)^{y}$$
3) Hypergeometric distribution: $X$ = # of successes from a random sample of size $n$ from a total population of $N$ containing $D$ successes. As such, the hypergeometric distribution requires 3 parameters $(N,D,n)$. 
4) Multinomial distribution: generalization of the binomial distribution to a trial with multiple outcomes (non-binary event).

Some interesting notes on the properties of each of these distributions:

# Binomial Distribution
The mgf of the binomial distribution is as follows:
$$M(t) = \Sigma_x e^{tx}p(x)$$$$M(t) = \Sigma_x (e^{t}p)^x(1-p)^{n-x}$$ Applying the [Binomial Theorem](Binomial%20Theorem.md), we then obtain:
$$M(t) = (e^tp+(1-p))^n$$ We then apply the [properties of the moment generating function](Introduction%20to%20Mathematical%20Statistics%20-%201.9%20Some%20Special%20Expectations.md) to derive the mean and variance:
$$\mu = M'(0)= np$$
$$Var(X) = M''(0)-M'(0) = np(1-p)$$
