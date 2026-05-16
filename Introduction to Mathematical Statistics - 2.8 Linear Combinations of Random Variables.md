---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#robert_hogg"
  - "#math"
  - "#statistics"
date_created: 2026-02-12
---
We extend our results  to the special case of random variables that are a linear combination of other random variables:
1) How to determine the expectation of a random variable that is a linear combination of random variables.
2) How to determine the variance and covariance of a random variable that is a linear combination of other random variables.

We look at the special case of linear combinations of random variables, $T$ 
$$T = \Sigma^{n}_{i=1}a_iX_i$$and look at how to compute their means and variances if we know something about the original random variables $X_i$ that constitute it. ***Theorem 2.8.1*** shows that the expectation of $T$ is the same linear combination of the expectation which is proven by the additivity of the integral and linearity of expectations.


We'll often find that if the random variables are independent and identically distributed, then the linear combination will fall in the same family of distributions but with specific conditions. For instance, a linear combination of Poisson random variables is not a Poisson distribution itself.

***Theorem 2.8.2. (Covariance of a linear combination of random variables).*** Given another random variable, $W$, that is a linear combination of random variables $W = \Sigma_{i}^{n}b_iY_i$ , if $E(X^2)$ and $E(Y^2)$ are both finite [then by a theorem, their means must exist](Introduction%20to%20Mathematical%20Statistics%20-%201.10%20Important%20Inequalities.md) and we can determine $Cov(T,W)$
$$Cov(T,W) = \Sigma_{i}^{n} \Sigma_{j}^{m}a_ib_jCov(X_i,Y_j)$$
To compute the covariance, we have to compute $i \times j$ covariances. Using this result, we can prove the variance of a linear combination of random variables as the variance of a variable is just the covariance with itself

***Corollary 2.8.2 (Variance of a linear combination of random variables)*** The variance of $T$ is simply the covariance with itself:
$$Var(T) = Cov(T,T) = \Sigma_{i}^{n} a_{i}^{2}Var(X_i)+2\Sigma_{i<j}a_ia_jCov(X_i,X_j)$$
And if the individual random variables are independent, then their covariances are 0 and this simplifies to:

***Corollary 2.8.2 (Variance of a linear combination of independent random variables)***
$$Var(T) = \Sigma_{i}^{n} a_{i}^{2}\sigma_{i}$$
Our motivation to relate a random variable to its linear combination is to analyze random samples. ***Definition 2.8.1*** defines random samples as a set of random random variables that are identically distributed and independent from each other. The assumption of both identical distribution and independence is common when sampling randomly from a population. Its important to realize two things about random samples:
- They are characterized by their size which indicates the number of samples (i.e. the number of random variables).
- Each of these random variables has the same mean because they come from the same distribution
- Each of these random variables has the same variance because they come from the same distribution

Applying ***Theorems 2.8.1-2.8.2*** and their respective corollaries we obtain the mean and variance of some important functions of random samples called statistics:
- ***Example 2.8.1 (The mean of the mean is the mean while the variance scales down).*** Given a random sample $X_1,..X_n$ with the mean $E(X_i)=\mu$ and variance $Var(X_i)=\sigma^2$  the same mean defined as $\bar{X}\frac{1}{n}\sum\limits_{i=1}^n X_i$  has the same mean, but the variance scales down with the number of samples: $$E(\bar{X}) = \mu \text{\quad ; \quad} Var(\bar{X})=\frac{1}{n}\sigma^2$$
- ***Example 2.8.2 (The sample variance is an unbiased estimator of the true variance).*** Given a random sample $X_1,...X_n$ of size $n$ each with the same mean and variance of $\mu$ and $\sigma^2$ , the sample variance $S$ is a function of the random sample defined as follows and its expectation is the variance of the distribution: $$S=\frac{1}{n-1}\sum_{i=1}^n (X_i-\bar{X}) \text{\quad;\quad} E[S]=\sigma^2$$ Naively, one may be tempted to use $1/n$ as the coefficient for the sum, but it is $\frac{1}{n-1}$ that results in an unbiased estimator of the variance. The sample variance is also called the Bessel corrected sample variance

# Definitions
***Definition 2.8.1.*** If the random variables $X_1, X_2,.. X_n$ are independent and identically distributed (i.e. they all have the same distribution), then we say that these random variables constitute a random sample of size $n$ from that common distribution. A random sample is synonymous then with a group of random variables that are IID.
# Theorems
***Theorem 2.8.1 (The mean of linear combination of random variables).*** The mean of $T$ is linear combination of the of the, $n$, mean of the individual random variables with their respective coefficients:
$$E(T) = \Sigma_{i}^{n}a_i\mu_i$$
***Theorem 2.8.2 (Covariance of a linear combination of random variables).*** Given another random variable, $W$, that is a linear combination of random variables $W = \Sigma_{i}^{n}b_iY_i$ , if $E(X^2)$ and $E(Y^2)$ are both finite [then by a theorem, their means must exist](Introduction%20to%20Mathematical%20Statistics%20-%201.10%20Important%20Inequalities.md) and we can determine $Cov(T,W)$
$$Cov(T,W) = \Sigma_{i}^{n} \Sigma_{j}^{m}a_ib_jCov(X_i,Y_j)$$

***Corollary 1 to 2.8.2 (Variance of a linear combination of random variables)*** The variance of $T$ is simply the covariance with itself:
$$Var(T) = Cov(T,T) = \Sigma_{i}^{n} a_{i}^{2}Var(X_i)+2\Sigma_{i<j}a_ia_jCov(X_i,X_j)$$

***Corollary 2 to 2.8.1 (Variance of a linear combination of independent random variables)***
$$Var(T) = \Sigma_{i}^{n} a_{i}^{2}\sigma_{i}$$
