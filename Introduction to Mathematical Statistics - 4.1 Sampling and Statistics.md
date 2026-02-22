---
tags:
  - "#math"
  - "#robert_hogg"
  - "#statistics"
date_created: 2026-02-21
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
Chapter 4 provides various definitions to frame two problems regarding a random variable $X$ of interest and briefly provides a method to deal with both:
1) $f(x)$ or $p(x)$ is completely unknown. (the pdf/pmf is unknown)
2) The form of $f(x)$ or $p(x)$ is known down to a parameter $\theta$ that may be a vector (i.e. multiple parameters)

We deal first with the 2nd of these problems and examples of these include:
-  $X \sim binom(n,p)$ where $n$ is known but $p$ is unknown
- $X \sim N(\mu, \sigma^2)$ where both the average and variance are unknown
- $X\sim \Gamma(\alpha, \beta)$ where $\alpha$ and $\beta$ are both unknown
This problem is often denoted as "$X$ has a density function $f(x;\theta)$ or $p(x;\theta)$  where $\theta \in \Omega$ ". Where $\Omega$ is some specified set. So for example, for a binomial distribution, the parameter is $p$ in the set $\Omega = \{\theta| \theta \ge 0\}$ .

We now provide some definitions when we go through the process of taking samples from our sample space of our random variable $X$

***Definition 4.1.1 (Random Sample and Sample size).*** If the random variables $X_1,X_2,..X_n$ are independent and identically distributed random variables (iid), then these random variables constitute a random sample with sample size $n$ from a common distribution.

In other words, a random sample is a sequence of iid random data points. [Random sample is effectively synonymous with "IID"](https://en.wikipedia.org/wiki/Independent_and_identically_distributed_random_variables).

***Definition 4.1.2 (Statistic and Realization).*** If the random variables $X_1,X_2,..X_n$ are independent and identically distributed random variables (iid). Then $T = T(X_1,X_2,...X_n)$ is a random variable called a statistic. When the $X_i$ take on a specific value $x_i$, they are said to be realized and so the statistic $T(x_1,x_2,...x_n)=t$ is realized to $t$.

A statistic is then effectively a transformations of our random sample and realizations are effectively when we make actual observations of the sample space and note down their values.
# Solving problem 2)
Returning to our problem with 2), the method we introduce what's called a <u>point estimator</u>: statistics that predict a specific value of our unknown parameter $\theta$ (this is in contrast to range estimates later). We call realizations of point estimators the <u>estimate</u> of $\theta$. There are multiple kinds of point estimators, but we look at the most simple one, unbiasedness:

***Definition 4.1.3 (Unbiasedness)***. Let $X_1,X_2,..X_n$ denote a sample on a random variable $X$ with pdf $f(x;\theta), \theta \in \Omega$. Let $T =T(X_1,X_2,...X_n)$. $T$ is an unbiased estimator of $\theta$ if $E(T)=\theta$ 


The inferential method we introduce is the statistic called the maximum likelihood estimator (mle). Assuming our random sample of sample size $n$  consists of iid random variables with an assumed pdf $f(X)$ , then the likelihood of any realization we have is then the [joint probability of independent random variables](Introduction%20to%20Mathematical%20Statistics%20-%202.4%20Independent%20Random%20Variables.md): $$L(\theta) = L(\theta; x_1,x_2,...x_n) =  \prod_{i=1}^nf(x_{i})$$
The $L(\theta)$ function is called the likelihood function and notice that is solely a function of our unknown parameter when we have a realization. We then treat the problem of determining $\theta$ as trying to find the $\hat{\theta}$ that maximized our chance of observing this realization. $$\hat{\theta}=Argmax[L(\theta)] \text{\quad(the maximum likelihood estimator)}$$
This then becomes a calculus problem of finding the maximum that may involve partial derivatives if $\theta$ is a vector involving multiple parameters. It must be noted that $\hat{\theta}$ effectively becomes the statistic that is the point estimator for $\theta$ and so we must check if the mle is an unbiased estimator. It is common to instead compute the point that maximizes the logarithm of the likelihood function as it converts the product of probabilities in the likelihood function into a sum. Additionally, the logarithm is a strictly increasing function so whatever maximizes $L(\theta)$ is also the maximum for $l(\theta)=ln[L(\theta)]$:

$$\hat{\theta}= \{\theta | \frac{dl}{d\theta} = 0\} \text{\quad where\quad} l(\theta)=ln[L(\theta)]$$
The book then goes through some examples showing what the mle is for a realized sample from various distributions. I list the ones that have an unbiased estimator and in each of these cases, the mle is simply the sample average which is an unbiased estimator for the random sample (i.e. iid by definition 4.1.1):
- ***Example 4.1.1*** Exponential distribution $\Gamma(1,\beta)=\frac{1}{\theta}\exp(\frac{-x}{\theta})$. $$l(\theta)=\ln \prod_{i=1}^n \frac{1}{\theta}e^{-x_{i}/\theta}=-n \ln(\theta)+\theta^{-1}\Sigma_{i=1}^{n}x_{i}) \text{\quad;\quad}\frac{dl}{d\theta}=-n\theta^{-1}+\theta^{-2}\Sigma_{i=1}^{n}x_{i} \text{\quad;\quad}\hat{\theta}=\bar{X}$$
And we find that the mle is the sample average and $E(\hat{\theta})=E(\bar{X})=E(X)$ and so it is an unbiased estimator of the exponential function
- ***Example 4.1.1 (Binomial Distribution).*** $X\sim binom(n,\theta)$ $$\hat{\theta}=\bar{X}$$
- ***Example 4.1.2 (Normal Distribution).*** $X\sim N(\theta_1, \theta_2)$ $$\hat{\theta_{1}}=\bar{X} \text{\quad;\quad}\hat{\theta_{2}}=\frac{1}{n}\Sigma^n_{{i=1}}(X_{i}-\bar{X})^2$$
An example where the mle is not an unbiased estimator is for the uniform distribution.

Methods like the mle method that assume a particular distribution in which we must estimate the parameter are called <u>parametric tests</u> so called I assume because they involve estimating a parameter. In general, <u>methods that answer problem 2) are parametric tests</u>
# Solving problem 1)

We now introduce a method to answer problem 1). As these do not assume a distribution so we're not estimating any particular parameters of the distribution, <u>methods that solve problem 1) are called nonparametric tests</u>







