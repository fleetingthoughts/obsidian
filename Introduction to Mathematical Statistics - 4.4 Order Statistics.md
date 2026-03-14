---
tags:
  - "#math"
  - "#robert_hogg"
  - "#statistics"
date_created: 2026-03-02
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
The point estimators and confidence intervals relies on an assumption of the general shape of the pdf of the random variable of interest. Here we look at an inference that does not assume a distribution: order statistics. In this section we discuss:
- What the ordered statistic is and how its derived from a random sample
- The general pdf and marginal pdf of the ordered statistic
- The ordered statistic of our random variable as a predictor for percentiles without assuming anything about the underlying distribution of our random variable of interest
- The use of ordered statistics of a random sample to derive distribution free confidence intervals of the percentiles.

Given a random sample $X_1,..X_n$ we denote the ordering with a new random variable $Y_i$ such that $Y_i<Y_j$ if $i<j$. This means $Y_1$ and $Y_n$ will be the smallest and largest respectively in a random sample of size $n$. We call $Y_i$ the order statistic of the random sample. The order statistic has a pdf that can immediately be determined:

***Theorem 4.4.1 (pdf of the joint distribution of the order statistic).***  The order static of an random sample of size $n$ from a distribution with a pdf of $f(x)$ has a joint pdf of:$$g(y_{1},\dots ,y_{n})=n!f(y_{1})f(y_{2})\dots f(y_{n})\text{\quad}y_{1}<y_{2}\dots<y_{n}$$
The $n!$ factorial occurs because any ordering we have can correspond to different permutations of our random sample. For our random sample of size $n$, there are $n!$ different ways to permute it. 

Since this is a random sample, each of the random variables are independent with each other and we can determine the marginal pdf of any particular $k$th order statistic:$$g_{k}(y_{k})=
\int_{a}^{y_{k}}\dots \int_{a}^{y_{2}}\int_{y_{k}}^b\dots \int_{y_{n-1}}^bn!f(y_{1})f(y_{2})..f(y_{n})dy_{n}\dots dy_{k+1}dy_{1}\dots dy_{k-1}$$
Where in this particular order of integration, we first integrate largest order static down to $y_{k+1}$ then we integrate from the smallest statistic to $y_{k-1}$. 
Once we observe that for the integration of the smaller order statistics we have the integrals:$$\int_{a}^x[F(w)]^{\alpha-1}f(w)dw=\frac{[F(x)]^{\alpha}}{\alpha}$$
And for the larger order statistics, the integration is:$$\int_{y}^b[1-F(w)]^{\beta-1}f(w)dw=\frac{[1-F(y)]^{\beta}}{\beta}$$
The result for the marginal pdf can be derived.$$g_{k}(y_{k})=\frac{n!}{(k-1)!(n-k)!}[F(y_{k})]^{k-1}[1-F(y_{k}]^{n-k}f(y_{k})\text{\quad} a<y_{k}<b$$
Where in this case we have $n-k$ larger order statistics and then $k-1$ smaller order statistics and $F(x)$ is the cdf of the original random variable (which we make no assumption on the distribution for our inferences in this section).

The ordered statistic random variable is useful because they serve as predictors for the percentiles and quantiles of a distribution. That is, we propose that the  $F(Y_k)$ will represent a percentile depending on how large our sample is.  For instance, given a sample if size $n=11$, the $Y_6$ ordered statistic can be shown to be a predictor of the median, $x_{0.5}$ (that is the median of the dataset is a predictor of $x$ such that $F(x)=0.5$). This can be shown by examining the expected value of $E(F(Y_k))$: $$E[F(Y_{k})]=\frac{k}{n+1} \text{\quad note k is always such that }k<n$$
And so any the $kth$ ordered statistic is an estimator of the $k/(n+1)$ percentile of the original random variable's pdf. Obviously, we can only estimate a finite number of percentiles depending on how large our sample size in (a sample size of 3 can only estimate the median!). Usually if we want to estimate the $pth$ percentile $\xi_p=F^{-1}(p)$, the most conservative estimate we can do is use the $Y_k$ ordered statistic where $k$ is the largest integer such that $k\le p(n+1)$. So for example in a sample size of 100, the 1st quartile will be $Y_{25}$ (since $25 \le 0.25(100+1)$).

We now describe 





- 
- Order statistics makes confidence intervals independent of the distribution of the original function by applying the principles of the bernoulli trial. Given a random sample, the probability that a random observation is above or below the desired quantile is essentially a success or failure bernoulli trial.
