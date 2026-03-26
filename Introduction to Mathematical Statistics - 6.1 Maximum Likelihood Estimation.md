---
tags:
  - math
  - statistics
  - robert_hogg
date_created: 2026-03-25
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---

In section [Introduction to Mathematical Statistics - 4.1 Sampling and Statistics](Introduction%20to%20Mathematical%20Statistics%20-%204.1%20Sampling%20and%20Statistics.md), we looked at "maximum likelihood estimators" (mle) and had provided motivating examples with distributions where we already know the answer and show that the mle method produces estimators that produce our answer. In this chapter, we develop the theory to show how the mle method produces an estimator and how that estimator is consistent. Later chapters will show this estimator can be asymptotically optimal. The chapter is outlined as follows:
- Justification for how the maximum likelihood method gives a reasonable estimator
- A method to determine the mle of a transformation of our parameter assuming the random sample comes from the same distribution
- Demonstrate that the estimator produced by the mle method is consistent.

Recall that we have defined some concepts to formalize a criteria for a "good" estimator. Some of these include:
- unbiasedness: the idea that the estimator doesn't overestimate or underestimate given the "CURRENT" size
- consistency: the idea that if we take enough samples, the estimator will eventually match our estimator.
An illustration of this is the uncorrected sample variance compared to the Bessel corrected sample variance. The uncorrected sample variance is biased, but it is still a consistent estimator because if we take enough samples, the difference of 1 in the denominator "washes away" and it becomes pretty much identical to the unbiased Bessel corrected sample variance anyways.

In this chapter we show the justification for the method in obtaining this estimator and then show that this estimator has the desirable quality of consistency to our true sample mean. I will try to provide an intuitive understanding to understand the moral solution rather than dive into the proofs which is more fitting for an analysis book outside the scope of this one.

Some key assumptions in the mle method:
- We assume we already know the general form of the distribution of the random variable and all we're missing is the parameter $\theta$ 
- We also assume that the random variable satisfies what's called the <u>regularity conditions </u>in the definitions section
The mle method involves making use of a realized sample and determining the appropriate $\theta$ parameter so effectively, our random variable is not the "variable" anymore but rather $\theta$ is the variable of interest. The iid assumption guarantees that every observation has the same distribution with respect to $x$, but the regularity assumptions basically guarantee the same thing for $\theta$ since the parameter is now our "variable of interest". The Regularity assumptions basically guarantee 1) that the pdf actually changes with $\theta$ and is dependent on it so that we can use it as a variable and 2) that every random sample not only has the same function but has the same domain as well in $\theta \in \Omega$. What this does is it guarantees we can take derivatives and expect the same result no matter the observation. We will later see models where this isn't satisfied to illustrate the concepts better.

To give an intuitive understanding of the moral answer behind the likelihood method, any observation we make can be interpreted as follows: "the realizations we saw are there because they happened to be the most likely ones". The idea is then that the set of observations happened to have a parameter that maximized our chances of seeing it. The idea is then to find the joint pdf of our realizations and maximize it. This joint pdf of the independent random sample is called the likelihood function $L(\theta;x)$: $$L(\theta)=\prod_{i=1}^nf(x_{i};\theta)$$
Note that because we're looking at a realized sample, the only variable to maximize is $\theta$ and this maximum is in ***Definition 6.1.1*** called the <u>maximum likelihood estimator</u> (mle) 

***Theorem 6.1.1.*** gives us the theoretical justification for this method. Colloquially, the theorem is saying that as we take more observations, the parameter that maximizes the likelihood function is guaranteed to be the true parameter which we are trying to determine. Note that this tells us nothing about how far off our estimate might be if we take a finite sample size, but the theorem gives us the assurance that with enough effort finding the parameter that maximizes the likelihood function (called the mle) eventually gives us the true parameter 

Now that we have some assurance that the mle method will work eventually, we look at some useful properties of the mle. Namely we answer the question: "if we know the mle of the parameter for a realized sample can we determine the mle for a transformation of the random sample?". Can we determine the mle for $g(\theta)$? We are effectively trying to determine what maximizes $L(g(\theta))$. But note that $g(\theta)$ is just derived from the same sample space as $\theta$ so whatever maximizes $L(\theta)$ is what maximizes $L(g(\theta))$ as well. Do not be confused by the different notation, they are derived from the same sample space.
# Definitions
***Assumptions 6.1.1. (The Regularity Conditions).*** Regularity conditions 1-3 are:
1) The cdfs are distinct in that if $\theta \ne \theta' \implies F(x_{i};\theta)\ne F(x_{i};\theta')$. In other words, the cdf definitely changes if the parameter is different
2) The pdfs have a common support for all of $\theta$. This is an important one as there will be models that don't satisfy this
3) The true parameter $\theta_o$ is an interior point in the same set as $\theta\in \Omega$ 
***Definition 6.1.1 (The Maximum Likelihood Estimator).*** We say that a $\hat{\theta}=\hat{\theta}(X)$ is a maximum likelihood estimator of $\theta$ if it is the value where the likelihood function achieves its maximum, that is: $$\theta=Argmax[L(\theta;X)]$$
# Theorems
***Theorem 6.1.1 (The true parameter is the maximum of the likelihood function).*** Assume that $\theta_o$ is the true parameter and that $E_{\theta_o}[f(X_i;\theta)/f(X_i;\theta_o)]$ exists. Then under the regularity assumptions, we observe that: $$\lim_{ n \to \infty }P_{\theta_{o}}[L(\theta_{o}, X)>L(\theta,X)]\text{\quad for all }\theta \ne \theta_{o} $$
***Theorem 6.1.2 (Determine the mle of a function of a parameter when the mle of the parameter is known).*** Let $X_1,...,X_n$ be a random sample (i.e. iid) with a distribution $f(x_i;\theta)$ where $\theta \in \Omega$. Let a transformation $\eta=g(\theta)$ be a parameter of interest. If $\hat{\theta}$ is the mle, then $\hat{\eta}=g(\hat{\theta})$ is the mle of $\eta$

***Theorem 6.1.3.*** Assume that $X_1,...X_n$ satisfy the regularity conditions 1-3 and that we also have the following:
- $\theta_o$ is the true parameter
- Each $X_i$ has a distribution $f(x_i,\theta)$ with $\theta \in \Omega$ 
Then the differential equation: $$\frac{dL}{d\theta}=\frac{dl}{d\theta}=0$$
has a solution $\hat{\theta}$ that converges in probability to the true parameter, that is :$$\hat{\theta}\xrightarrow{P}\theta_{o}$$ 