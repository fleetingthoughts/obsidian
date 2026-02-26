---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#robert_hogg"
  - "#math"
  - "#statistics"
date_created: 2026-02-12
---
We look at the special case of linear combinations of random variables, $T$ 
$$T = \Sigma^{n}_{i=1}a_iX_i$$ and look at how to compute their means and variances if we know something about the original random variables $X_i$ that constitute it.

***Theorem 2.8.1 (The mean of linear combination of random variables).*** The mean of $T$ is linear combination of the of the, $n$, mean of the individual random variables with their respective coefficients:
$$E(T) = \Sigma_{i}^{n}a_i\mu_i$$
We'll often find that if the random variables are independent and identically distributed, then the linear combination will fall in the same family of distributions WITH CONDITIONs. For instance, a linear combination of Poisson random variables is not a Poisson distribution itselfTh

***Theorem 2.8.1. (Covariance of a linear combination of random variables).*** Given another random variable, $W$, that is a linear combination of random variables $W = \Sigma_{i}^{n}b_iY_i$ , if $E(X^2)$ and $E(Y^2)$ are both finite [then by a theorem, their means must exist](Introduction%20to%20Mathematical%20Statistics%20-%201.10%20Important%20Inequalities.md) and we can determine $Cov(T,W)$
$$Cov(T,W) = \Sigma_{i}^{n} \Sigma_{j}^{m}a_ib_jCov(X_i,Y_j)$$
This means to compute the covariance, we have to compute $i \times j$ covariances.

***Corollary 2.8.1 (Variance of a linear combination of random variables)*** The variance of $T$ is simply the covariance with itself:
$$Var(T) = Cov(T,T) = \Sigma_{i}^{n} a_{i}^{2}Var(X_i)+2\Sigma_{i<j}a_ia_jCov(X_i,X_j)$$
And if the individual random variables are independent, then their covariances are 0 and this simplifies to:

***Corollary 2.8.1 (Variance of a linear combination of independent random variables)***
$$Var(T) = \Sigma_{i}^{n} a_{i}^{2}\sigma_{i}$$
Our motivation for all this math is to analyze random variables called random samples

***Definition 2.8.1.*** If the random variables $X_1, X_2,.. X_n$ are independent and identically distributed (i.e. they all have the same distribution), then we say that these random variables constitute a random sample of size $n$ from that common distribution. A random sample is synonymous then with a group of random variables that are IID.

In several examples, the author derives the results for statistics of random samples that will be used repeatedly:
- Sample mean, $\bar{X}$ defined as a specific linear combination of the random sample
- $E(\bar{X})= \mu$. Later we'll show this follows the definition of an unbiased estimator of a parameter, in this case, the mean of the random variable
- $Var(\bar{X})=\frac{\sigma^2}{n}$. Note that this aligns with our intuitive notion that the "deviation" of the sample mean from the true mean decreases as we take more samples. Also, unlike the sample mean, we cannot calculate $Var(\bar{X})$ strictly from the random sample so we need another statistic we can use to estimate the variance.
Seeing that the sample mean is a unbiased estimator of the true mean, we try to find a similar statistic that serves as an unbiased estimator. One is the sample mean with the Bessel Correction.

