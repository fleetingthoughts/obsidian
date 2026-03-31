---
tags:
  - statistics
  - math
  - robert_hogg
date_created: 2026-03-27
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
The characteristic of a good estimator is one that minimizes variance so that we can be confident the predictor we have is close to the true parameter (if it is an unbiased estimator). In this chapter we look at the theoretical lowest variance any statistic can have called the Cramer-Rao lower bound that gives a numerical value on the error, and also the lowest variance an unbiased estimator can have. The lower bound is then applied to show that the maximum likelihood estimator can achieve this lower bound and is therefore consistent as we increase our sample size.

The chapter assumes the statistical problem of a known distribution with an unknown parameter :
- How to determine the Fischer information and score function of a random variable
- How to determine the Rao-Cramer lower bound on the variance of a statistic and whether the statistic is an efficient estimator.

Throughout this chapter, we have to make various regularity assumptions. Different theorems will require different levels of assumption. The derivation of a lot of the results are demonstrated by lucky manipulations that happen to tell us something about our pdf and so this is what we shall do. We first derive the Fischer Information and the score function by taking the derivative of the identity. Note that we'll have to assume regularity assumptions 1-5 so that we can make the differential manipulations. Taking the identity$$\begin{align}1 &=\int_{-\infty}^\infty f(x;\theta)dx  \\
0& = \int_{-\infty}^\infty \frac{\partial f(x;\theta)}{\partial \theta}dx \\
0& = \int_{-\infty}^\infty \ \frac{f(x;\theta)/\partial{\theta}}{f(x;\theta)}f(x;\theta)dx \\
0&= \int_{-\infty}^\infty \frac{\partial \ln f(x;\theta)}{\partial \theta}f(x;\theta)=E\left[\frac{\partial \ln f(x;\theta)}{\partial \theta}\right]
\end{align}$$
Now making use of regularity assumption 4) and 5) to take a 2nd derivative: $$\begin{align} 0&= \int_{-\infty}^\infty \frac{\partial^2 \ln f(x;\theta)}{\partial \theta^2}f(x;\theta)dx + \int_{-\infty}^\infty \left(\frac{\partial \ln f(x;\theta)}{\partial \theta}\right)^2f(x;\theta) \\
E\left[\frac{\partial^2 \ln f(x;\theta)}{\partial \theta^2}\right]&=-E\left[\left(\frac{\partial \ln f(x;\theta)}{\partial \theta}\right)^2\right]


\end{align}$$
Noting that these are expectations in the first and second moment, we can therefore compute the Fischer information denoted $I(\theta)$ by using these expectations and with the 2nd moment, we have choice but usually the left-hand side of the equality is easier to compute. The Fischer information is the variance of the score function which appears in the likelihood function.

Now with this interesting function, what we notice is that if we take any statistic that is a function of our unknown parameter on a realized sample. If we take the derivative of the expectation of that statistic, we can derive a lower bound for the variance called the Cramer-Rao Lower Bound (CRLB). ***Theorem 6.2.1*** shows how to compute the CRLB and its corollary shows what this simplifies to if the statistic is an unbiased estimator of our parameter such that its expectation is simply our unknown parameter $\theta$ itself.

The importance of the CRLB is that it gives us a numerical "ideal" for how low our variance can be and so for any statistic that is an estimator, we want its variance to be as low as possible so we want it to obtain the CRLB. Most notably, the CRLB also gives us a numerical estimate of how low our variance can be. The variance of an unbiased estimator in particular can only be as<u> low as the reciprocal of the Fischer information</u> We then give various efficiency metrics and terms to measure how close the variance of our statistic is to the CRLB in the 3 definitions ***Definitions 6.2.1-6.2.3***. I note the following significant things about this result:
- The CRLB is a function of the Fischer Information which in turn is a function of the derivative of the pdf itself. We can compute tables of formulae of the Fischer information for various distributions and therefore determine the formula for the CRLB for each distribution

In order to see how we can apply these results to the log-likelihood functions, we will not require a 6th regularity assumption in ***Assumption 6.2.2*** which allows us to take a triple derivative that is bounded. The mle's in a lot of the examples were computable in closed form but this is often not the case. Without a closed form, we don't have a function to manipulate to say something about its variance, but we are still able to show that the MLE estimators are asymptotically efficient. ***Theorem 6.2.2*** colloquially means that as we take more samples, the error (i.e. the difference between our estimator of the parameter and the true parameter) will be a normally distributed such and we achieve the lowest possible variance in the CRLB assuming our mle is unbiased.


While the asymptotic efficiency of an estimator is closely related to the consistency of an estimator, its important to note the differences and how they complement each other:
- An estimator can still converge to the true value even if it is not asymptotically efficient, that is an estimator can still be consistent even if it is not necessarily asymptotically efficient. Consistency implies nothing about the CRLB. The CRLB is a "stronger condition" then consistency by giving  a numerical estimate of the variance.
- The Cramer-Rao lower bound gives an estimate of how low the variance can be for a given sample size. It is a measure of what the variance is like "right now" while the consistency is a measure of "do we eventually reach our goal if we work hard enough and collect enough samples". 
- The CRLB can be used to show consistency IF we can show our estimator is asymptotically efficient such that its variance is its CRLB.
# Definition
For all definitions, the premise of our problem is that $X$ is our random variable of interest where we know the form of the distribution $f(x; \theta)$ but do not know one of its parameters $\theta$ where $\theta \in \Omega$ 

- ***Fischer Information (p. 363)*** Denoted $I(\theta)$, the Fischer information is the variance of the partial derivative of the natural logarithm of the pdf. There are two equivalent ways to compute the 2nd moment: $$I(\theta)=Var\left[\frac{\partial \ln f(X;\theta)}{\partial \theta}\right]$$
- ***Score Function (p. 364)*** The score function is the function of interest that the Fischer information takes the variance of $\frac{\partial \ln f(X;\theta)}{\partial \theta}$. 

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
