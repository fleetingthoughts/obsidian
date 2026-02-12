---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#statistics"
  - robert_hogg
date_created: 2026-02-11
---
We look at a specific measure of the dependency between two random variables that are not independent

***Definition 2.5.1 (The Covariance).*** Let $(X,Y)$ have a joint distribution and the variances of $X$ and $Y$ be denoted by $\mu_1$ and $\mu_2$ and $\sigma_1$ and $\sigma_2$ respectively. The covariance is denoted and defined as follows:
$$Cov(X,Y) = E[(X-\mu_{1})(Y-\mu_{2})]$$
By the [linearity of the expectations](Introduction%20to%20Mathematical%20Statistics%20-%202.1%20Distributions%20of%20Two%20Random%20Variables.md), the covariance can be expressed as
$$Cov(X,Y) = E(XY)-\mu_1 \mu_2$$ to obtain a unitless coefficient, we use the following definition:
***Definition 2.5.2 (The correlation coefficient)***. The unitless correlation coefficient is denoted and defined as follows:
$$ \rho = \frac{Cov(X,Y)}{\sigma_{1}\sigma_{2}}$$
***Theorem 2.5.1 (The bounds of the correlation coefficient).*** For all jointly distributed random variables $(X,Y)$ whose correlation coefficient $\rho$ exists, then $-1\le \rho \le 1$ 

***Theorem 2.5.3 (a null covariance as a necessary condition for independent random variables).*** Given $(X,Y)$ random variables that are independent, the independence of the random variables is a sufficient condition for $Cov(X,Y) = 0$.

Proof of this follows from [theorem 2.4.4](Introduction%20to%20Mathematical%20Statistics%20-%202.4%20Independent%20Random%20Variables.md) on the expectation of the product of independent random variables. Note that for theorem 2.5.3, it is a sufficiency condition but a covariance of 0 is not sufficient for the random variables to be independent. There are dependent random variables with a covariance of 0. It is worth noting though as a corollary that <u>the contrapositive of theorem 2.5.3 IS TRUE, that is, if $\rho \ne 0$, then $X$ and $Y$ are necessarily dependent.</u>