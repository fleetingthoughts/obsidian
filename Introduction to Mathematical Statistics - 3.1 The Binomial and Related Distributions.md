---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#statistics"
  - "#robert_hogg"
date_created: 2026-02-13
---
We explain 3 distributions related to the Bernoulli l distribution and demonstrate their mean and variance. Its important to distinguish the <u>Bernoulli distribution</u> from the <u>Binomial distribution</u>. I often get the terms mixed up but the Binomial distribution is derived from the Bernoulli distribution. We first begin with the Bernoulli distribution.

The Bernoulli random variable maps a Bernoulli trial that views an event as either a success or a failure. The Bernoulli Random variable, $X$, maps success to the real number 1 and failure to the real number 0, so the Bernoulli random variable is a discrete random variable with two numbers in its support. If the probability of a success occurring is $p$, then the pmf is
$$p(x) = p^x(1-p)^{1-x}$$ It can then be shown the expectation is $p$ and the variance is $p(1-p)$. Using this distribution, we can then look at the sequence of Bernoulli trials:
1) Binomial random variable: $X =$ total # of successes in $n$ Bernoulli trials. Requires the parameter $n$ (# of trials) and $p$ (the probability of success) $$p(x) = \binom{n}{x} p^x(1-p)^{n-x} \text{\quad ; \quad} \mu =np \text{\quad ; \quad} Var(X)=np(1-p)=\sigma^2 \text{\quad ; \quad} M(t) = \Sigma_x e^{tx}p(x)$$
   The mgf follows from a simple application of the Binomial Theorem.
 

2) Negative Binomial Random Variable: $Y$ = total # of failures before the $r$th success (i.e. y+r-1 trials since the last trial has to be a fixed success). Note that although it technically has two variables, the # of successes is treated as a fixed parameter. (1 parameter)
$$p_{Y}(y)=\binom{y+r-1}{r-1}p^r(1-p)^{y}= \binom{y+r-1}{y}p^r(1-p)^{y}$$
3) In the special case of the Negative Binomial distribution where we're only interested in the probability of failures until the 1st success (i.e. $r=1$), it is referred to as the geometric distribution $$p(y)=p(1-p)^y$$ 
4) Hypergeometric distribution: $X$ = # of successes from a random sample of size $n$ from a total population of $N$ containing $D$ successes. As such, the hypergeometric distribution requires 3 parameters $(N,D,n)$. $$p(x) = \frac{\binom{N-D}{n-x} \binom{D}{x}}{\binom{N}{n}} \text{\quad;\quad} \mu = n\frac{D}{N} \text{\quad ; \quad} Var(x) = n\frac{D}{N}\frac{N-D}{N}\frac{N-n}{N-1}$$$
   With the mean and variance of
5) Multinomial distribution: generalization of the binomial distribution to a trial with multiple outcomes (non-binary event).

Some interesting notes on the properties of each of these distributions:

The author then proves using the mgf that the sum of independent random variables with a binomial distribution and the same probability of success, will have a binomial distribution itself

***Theorem 3.1.1. (Sum of independent binomially distributed random variables with the same p).*** Suppose $X_1,X_2,...,X_n$ are independent random variables that are distributed as $binomial(n_i,p)$, then $Y=\Sigma^{n}_{i=1}X_i$ will have the distribution $binomial(\Sigma^{n}_{i=1}n_i,p)$

To give an intuitive understanding of this result, the sum of the binomially distributed random variables in 3.1.1 is effectively combining all the Bernoulli trials conducted. If person A conducted $x$ amount of Bernoulli trials, and person B conducted $y$ amount of Bernoulli trials and we combined their data, it is effectively the same as one person doing $x+y$ Bernoulli trials.
