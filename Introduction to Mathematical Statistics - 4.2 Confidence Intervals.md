---
tags:
  - "#statistics"
  - robert_hogg
  - "#math"
date_created: 2026-02-24
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
We continue with the problem of determining the parameters to full describe the distribution of a random variable who's general distribution shape we know about (e.g. we know its a binomial but what's the probability of success, that is the parameter $p$). In 4.1, we looked at point estimators of this parameter and discussed the mle method, but as the mle itself is a function of random variables, the point estimator itself is a random variable and has a distribution, and so, on top of getting a point estimate, we now want a measure of the range of possibilities the mle can take. One such measure is the confidence interval:

***Definition 4.2.1 (Confidence Interval).*** Let $X_1,X_2,...X_n$ be a random sample (i.e. IID) on a random viable $X$ with the pdf $f(x;\theta), \theta \in \Omega$. Let $0 <\alpha<1$ be specified. Let $L = L (X_1,X_2,...X_n)$ and $U = U(X_1,X_2,...X_n)$ be two statistics. We say that the interval $(L,U)$ is a $(1-\alpha)$ confidence interval for $\theta$ if: $$1-\alpha = P[ \theta \in (L,U)]$$
A nuance that should be noted is that the interval $(L,U)$ is itself random and the confidence interval is defined as the probability that these two random variables will result in an interval that contains our parameter. Once $L$ and $U$ area realized $l$, and $u$, it is not correct to say that there is a $1-\alpha$ chance that $\theta \in (l,u)$. The key is that there is a $1-\alpha$ chance that our interval will contain $\theta$ rather than $\theta$ being contained in our realized values. This distinction is communicated by saying that one is $1-\alpha$ "confident" that $\theta$ is in the realized confidence interval as opposed to saying "there is a $1-\alpha$ probability that $\theta$ is in the realized confidence interval."

One method to generate confidence intervals is the pivot method. This is not defined in Hogg's text so I take one from DeGroot and Schervish

***Definition (Pivot)***. Let $X_1,X_2,...X_n$ be a random sample distribution that depends on parameter $\theta$ and let $V(X_{1},X_{2},\dots,X_{n},\theta)$  be a statistic. $V$ is called a pivot random variable if the distribution is the same for all $\theta$.