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

The essence of the pivot method is to make use of a statistic, $V$ with a known distribution who's values do not depend on the parameter, $\theta$ , so that we can compute a $P(V= v_1)$ and $P(V=v_2)$ such that $P(v_1 < V <v_2) = 1-\alpha$ (our desired confidence level) and then algebraically manipulating it $V$ by applying some function $f$ to isolate the desired parameter, that is, $f(V) = \theta$ so we can find $P(f(v_1)< \theta < f(v_2))$ where $(f[v_1], f[v_2])$ is our desired confidence interval. I believe this requires our statistic $V = V(X_1,X_2,.. X_n, \theta)$ to be a bijective function so that it is invertible. In summary the algorithm to determine the confidence interval from a random sample $(X_n)$ of a parameter of a random variable with a known distribution but unknown parameter is as follows:
1) Determine a pivot quantity $V(X_1,X_2,... X_n, \theta)$. This is the hardest part that requires creativity. Note that once the random sample is realized, this just becomes a function of $\theta$, 
2) Choose a confidence level $1-\alpha$ 
3) Determine the cdf of the pivot statistic $V$ and find the critical values $a$ and $b$ such that $P(a \le V(\theta) \le b) = 1-\alpha$
4) Invert $V$ to isolate for $\theta$ so we find $P[V^{-1}(a) \le \theta \le V^{-1}(b)] = 1-\alpha$. The confidence interval will then be $(V^{-1}(a), V^{-1}(b)))$ 
Note that it is key the pivot variable's distribution does not depend on $\theta$ so that we can execute step 3).

Hogg then goes through some worked examples to illustrate the pivot method and shows pivot statistics that can be used to determine parameters for random variables belonging to certain distribution
- Example 4.2.1: the $T = (\bar{X}-\mu/(S/\sqrt{n})$ statistic is a pivot statistic for a $X\sim N(\mu, \sigma^2)$ where we do not know the mean or the variance. $T$ only depends on the degrees of freedom, but in a realized sample, this value is known.
The $T$-statistic being a pivot variable depended on the normality of the random variable, however by a theorem to be proven later in Chapter 5, we can show that if we have a large enough sample size, $T$-statistic of ANY random variable that isn't normal will approximate to a normal distribution so that we can use the $Z$-distribution directly.

***Theorem 4.2.1 (Central Limit Theorem).*** Let $X_1, X_2, ...X_n$ denote observations from a random sample with a finite variance and therefore a mean. Then the distribution of the random variable $W_n = (\bar{X}-\mu)/(\sigma/\sqrt{n})$ converges to the $N(0,1)$ distribution as $n\to \infty$. Similarly, this result holds if $\sigma$ is not known and is replaced with the sample standard deviation $S$ where $S^2= (n-1)^{-1}\sum_{i=1}^{n}(X_i-\bar{X})^2$ 

Because we this $W_n$ statistic (which is basically the $T$-statistic) converges to $N(0,1)$, we can technically use the $Z$-distribution (i.e. $N(0,1)$) to directly approximate confidence intervals, but the t-distribution is still preferred because it is a wider therefore resulting in a larger and more conservative confidence interval for we do not know how fast the random variable can converge to $N(0,1)$.  

# 4.2.1 Confidence Intervals for Difference in Means

# 4.2.2 Confidence Intervals for Difference in Proportion of Means
