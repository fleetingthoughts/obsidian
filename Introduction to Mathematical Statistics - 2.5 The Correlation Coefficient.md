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

Proof of this follows from [theorem 2.4.4](Introduction%20to%20Mathematical%20Statistics%20-%202.4%20Independent%20Random%20Variables.md) on the expectation of the product of independent random variables. ***Theorem 2.4.4*** is a sufficiency condition but is not necessary. A covariance of 0 is not sufficient for the random variables to be independent. There are dependent random variables with a covariance of 0. It is worth noting though as a corollary that the contrapositive of ***Theorem 2.5.3*** is true, that is, if $\rho \ne 0$, then $X$ and $Y$ are necessarily dependent.

# Computation summary
- To compute the covariance using the joint distribution $f(x,y)$ from the definition, we'll need to compute three expectations:
	1) $E(X)=\mu_{1}$
	2) $E(Y)=\mu_2$
	3) $E(XY) = \int_{\infty}^{\infty}xyf(x,y)dx dy$ 
# Concepts from Exercises
***Exercise 2.4.8 (Computation of the mean, variance of the individual variables and the covariance using the cumulant).*** The cumulant is the logarithm of the moment generating function $M$. For a joint distribution $f(x,y)$, the cumulant is defined as $\psi(t_1,t_2)=\ln[M(t_1,t_2)]$. The partial derivatives of the cumulant can directly compute the mean, variance and covariance more directly than partial derivative of the moment generating function $M$ as the partial derivatives of the mgf produce moments of the random variable instead. 
$$
\begin{array}{|l|l|l|}
\hline \text{To Find...} & \text{Use This Derivative} & \text{Notation} \\
\hline \text{Mean of } X & \frac{\partial \psi}{\partial t_1} \Big|_{t=0} & \mu_X \\
\hline \text{Mean of } Y & \frac{\partial \psi}{\partial t_2} \Big|_{t=0} & \mu_Y \\
\hline \text{Variance of } X & \frac{\partial^2 \psi}{\partial t_1^2} \Big|_{t=0} & \sigma^2_X \\
\hline \text{Variance of } Y & \frac{\partial^2 \psi}{\partial t_2^2} \Big|_{t=0} & \sigma^2_Y \\
\hline \text{Covariance} & \frac{\partial^2 \psi}{\partial t_1 \partial t_2} \Big|_{t=0} & \sigma_{XY} \\
\hline
\end{array}
$$
