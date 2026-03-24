---
tags:
date_created: 2026-03-23
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
This section discusses one of the most fundamental theorems to statistics that was touched on chapter 4 and in the $\triangle$-method which stated that the following statistic converged in distribution to the normal distribution $\sqrt{n}(X_n-\theta) \xrightarrow{D}N(0,\sigma^2)$.

This section lists a proof of the central limit theorem (CLT) using the mgf, and then goes through several examples to illustrate the application of the CLT and other concepts such as:
1) The ability to substitute $\sigma$ with the sample variance with the Bessel correction due to its convergence in probability to $\sigma^2$ 
2) Example 5.3.4: the use of continuity corrections to imitate continuity with a discrete random variable when we have to determine probabilities on non-countable sample spaces.
3) The use of the results from the $\triangle$-method that showed $\sqrt{n}(g(X_n))-g(\theta)) \xrightarrow{D} N(0,\sigma^2(g'(\theta))^2)$ which allows us to determine the distribution transformations of the sample average

The CLT can equivalently be stated as $\sqrt{n}(\bar{X}-\mu) \xrightarrow{D}N(0,\sigma^2)$. Since the chapter is short, I can address each of the outline points as follows:
1) Since the sample variance converges to $\sigma^2$, we can then apply Slutsky's theorem: the multiplication of a random variable that converges in probability and a random variable that converges in distribution results in a convergence in distribution to a multiple of the distribution
2) fd
3) We can apply the results from the $\triangle$-method in chapter 5.2.2 to determine the transformation of the sample averages and the mean. Namely substituting $\theta=\mu$ and $X_{n}=\bar{X_{n}}$ we then have: $$\sqrt{n}(g(\bar{X_{n}}))-g(\mu)) \xrightarrow{D} N(0,\sigma^2(g'(\mu))^2)$$
And so for instance we can try to determine a transformation for example that gives us a specific variance by choosing a specific $g(\mu)$ such that it has a derivative that causes the statistic to approximate to a normal distribution with the desired variance (i.e. we will have to solve a differential equation to determine the particular $g$ function that does so).

# Definitions
# Theorems
***Theorem 5.3.1 (Central Limit Theorem).*** Let $X_1,..., X_n$ denote the observations of a random sample from a distribution with mean $\mu$ and positive variance $\sigma^2$. Then the following random variable converges in distribution to $N(0,1)$:$$Y_n=\frac{(\sum_{i=1}^nX_{i}-n\mu)}{\sigma\sqrt{n}}=\frac{\sqrt{n}(\bar{X_{n}}-\mu)}{\sigma}$$
