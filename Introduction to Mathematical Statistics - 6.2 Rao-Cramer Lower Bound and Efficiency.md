---
tags:
  - statistics
  - math
  - robert_hogg
date_created: 2026-03-27
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
The characteristic of a good estimator is one that minimizes
# Definition
For all definitions, the premise of our problem is that $X$ is our random variable of interest where we know the form of the distribution $f(x; \theta)$ but do not know one of its parameters $\theta$ where $\theta \in \Omega$ 

- ***Fischer Information (p. 363)***
- ***Score Function (p. 364)***

- ***Assumptions 6.2.1 (Additional Regularity Conditions).*** On top of the [previous 3 assumptions of regularity](Introduction%20to%20Mathematical%20Statistics%20-%206.1%20Maximum%20Likelihood%20Estimation.md), we add 2 more assumption for our theorems:
4) The pdf of our random variable is twice differentiable with respect to the unknown parameter $\theta$
5) The integral of the pdf $\int f(x;\theta)dx$ can b e differentiated twice under the integral sign as a function of $\theta$.

- ***Definition 6.2.1 (Efficient Estimator).*** Let $Y$ be an unbiased point estimator of our parameter of interest $\theta$. $Y$ is called an efficient estimator of $\theta$ if and only if $Var(Y)$ attains the Rao-Cramer lower bound.

- ***Definition 6.2.2 (Efficiency)*** In cases where we can differentiate with respect to a parameter under an integral or summation symbol, the ratio of the Rao-Cramer lower bound to the actual variance of any unbiased estimator is called the efficiency of that estimator

- ***Assumptions 6.2.2 (Additional Regularity Conditions).*** The fifth assumption of regularity:
6) The pdf of the random variable is three times differentiable as a function of $\theta$. Furthermore, the function is bounded in a way such that: $$\frac{\partial^3}{\partial \theta^3}\ln f(x;\theta)\le M(x) \text{\quad where \quad}E_{\theta_{o}}[M(x)]<\infty \text{\quad for all \quad}\theta_{o}-c<\theta<\theta_{o}+c$$
- ***Definition 6.2.3 (Asymptotic Efficiency, Asymptotically efficient, and ARE).*** Let $X_1,...X_n$ be a random sample of $X$. Assume $\hat{\theta_{1n}}=\hat{\theta_{1n}}(X_{1},\dots X_{n})$ is an estimator of $\theta_o$ such that $\sqrt{ n }(\theta_{1n}-\theta_{o})\xrightarrow{D}N(0,\sigma^2_{\hat{\theta}_{1n}})$. Then we define the following 3 things
	- <u>Asymptotic efficiency</u> of $\hat{\theta_{1n}}$ is denoted $e(\hat{\theta_{1n}})$ and is defined to be: $$e(\hat{\theta_{1n}})=\frac{\frac{1}{I(\theta_{o})}}{\sigma^2_{\hat{\theta_{1n}}}}$$
	- The estimator $\hat{\theta_{1n}}$ is said to be asymptotically efficient if the asymptotic efficiency is 1.
	- Let $\hat{\theta_{2n}}$ be another estimator of $\theta_o$, then the asymptotic relative efficiency (ARE) of $\hat{\theta_{1n}}$ to $\hat{\theta_{2n}}$ is the reciprocal ratio of their respective asymptotic variances: $$e(\hat{\theta_{1n}},\hat{\theta_{2n}})=\frac{\sigma^2_{\hat{\theta_{2n}}}}{\sigma^2_{\hat{\theta_{1n}}}}$$

# Theorem
For all theorems, the premise of our problem is that $X$ is our random variable of interest where we know the form of the distribution $f(x; \theta)$ but do not know one of its parameters $\theta$ where $\theta \in \Omega$ 

- ***Theorem 6.2.1 (Rao-Cramer Lower Bound).*** Assume a random sample of $X$ of size $n$ and assuming the regularity assumptions 1-5. Also assume we have a statistic that is a function of the random sample $Y= u(X_1,...X_n)$ and with the expectation of the statistic being a function of $\theta$ denoted $k(\theta)=E(Y)=E[u(X_1,...X_2)]$. Then the variance of the statistic has a lower bound based on the Fischer Information and size of the sample: $$Var(Y)\ge \frac{[k'(\theta)]^2}{nI(\theta)}$$
- ***Corollary to the Rao-Cramer Lower Bound (lower bound on the variance of an unbiased estimator).*** If the the statistic $Y$ is an unbiased estimator of $\theta$ (i.e. $E[Y]=k(\theta)=\theta$), then the lower bound is: $$Var(Y)\ge\frac{1}{nI(\theta)}$$

- ***Theorem 6.2.2 (Error on the mle by the determining its convergence in distribution).*** Assume all regularity assumptions 1-6 are satisfied and we have a random sample of size $n$ of our random variable $X$ with a true parameter $\theta_o$. If the Fischer information of the function is bounded for all possible values (i.e. $0<I(\theta_{o})< \infty$). Then the following consistent sequence of solutions of the mle equations, $\hat{\theta}$ satisfies: $$\sqrt{n}(\hat{\theta}-\theta_{o})\xrightarrow{D}N(0,\frac{1}{I(\theta_{o})})$$
- ***Corollary 1 to Theorem 6.2.2 (transformations of the estimator).*** If $g(x)$ is a continuous function of $x$ that is differentiable at $\theta_o$ such that $g'(\theta_o) \ne 0$. Then the following convergence in distribution is satisfied: $$\sqrt{n}(g(\hat{\theta})-g(\theta_{o}))\xrightarrow{D}N(0,\frac{[g'(\theta)]^2}{I(\theta_{o})})$$
- 
