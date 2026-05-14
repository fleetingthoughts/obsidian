---
tags:
  - math
  - richard_courant
  - calculus
date_created: 2026-05-13
parent: "[[Introduction to Calculus and Analysis I]]"
---
The strategy of using the integral to represent a wide class of functions was advantageous because the existence of an integral is guaranteed by the continuity of the integrand but it is not a necessary condition. We hone in on the integral as a function and relax the condition of continuity to extend it to a wider class of functions.
1) The integral is defined on closed intervals that is in the domain of the integrand. We find a way to integrate an area where the integral is undefined at finite points or on open intervals. 
2) Define the improper integral as a limit of the integral function so we can treat integration over an open interval as an integration over a closed interval consistent with the original definition of the Riemann integral.
3) Boundedness and continuity in an open interval is sufficient for the improper integral to converge.
4) Determine consistency of the value of the improper integral with the original definition of the Riemann integral over a closed integral. If bounded and continuous except at finite points, the improper integral has the same value as Riemann sum with arbitrarily defined endpoints:
	- The improper integral defined by taking limits as the integration bounds approach the endpoints where it is undefined.
	- The proper Riemann integral on the closed integral obtained by assigning arbitrary values to those endpoints.
5) Tests for convergence of an improper integral with an integrand that diverges at an endpoint
	- The integral converges if the integrand becomes infinite of a lower order than the first
6) Test for convergence of an improper integral over infinite interval of integration.
	- The integral over an infinite interval of integration converges if the integrand decreases at a higher order than the first
7) Examples of important improper integrals
	1) The gamma function. Its relation to factorials when it is a function of natural numbers
	2) The Dirichlet integral. The reason for its convergence and absolute divergence
	3) Fresnel integrals

The Riemann integral is defined over a closed interval where the integrand is well-defined, and we are motivated to determine the effects of extending the definition to open intervals or a finite number of undefined points. Geometric intuition and appeal to area shows that the Riemann integral can have a value for areas with finite discontinuities, but a rigorous proof requires measure theory that is beyond the scope of this book so we take it for granted that it is possible. We propose a definition of the integral with an interval of integration with finite discontinuities or undefined points, show that this definition is consistent with the definition of the Riemann integral with arbitrarily defined endpoints. We take for granted from measure theory that this Riemann integral with arbitrary endpoints is consistent with the value of the Riemann integral of finite discontinuities, we then show our definition is consistent with the Riemann integral.

The improper integral $F$ over the open interval $(a,b)$ is defined by a sequence of its limits of integration that approach $a$ and $b$:  $$F=\lim_{ \epsilon \to 0}\int^{\beta_{\epsilon}}_{\alpha_{\epsilon}}f(x)dx \text{\quad; } \lim_{ \epsilon \to 0 } a_{\epsilon}=a; \text{\quad} \lim_{ \epsilon \to 0}b_{\epsilon}  $$ The improper integral is said to converge to $F$ as $\epsilon \to 0$ and is independent of the particular choice of $\alpha_{\epsilon}$ and $\beta_{\epsilon}$. 

The definition treats the integral of an open interval as the limit of a sequence of proper integrals integrated over a closed interval. It is proven by Cauchy's convergence test that the improper integral converges if we have the following:
- The integrand $f(x)$ is continuous in $(a,b)$.
- The integrand is bounded such that $|f(x)| \le M$

It is known that the Riemann integral exists if the integrand is continuous and the invariant to whatever we choose for $f(a)$ and $f(b)$. This Riemann integral with arbitrarily defined endpoints can be shown to have the same value as our improper integral, and so our definition is consistent with the definition of the Riemann integral and its results.

While the improper integral exists over an open interval if the integrand is bounded and continuous in an open interval, we look at the conditions for the integral to converge under two different scenarios:
1) The integrand becomes infinite in the open interval that has a finite length
2) Integration over an interval of infinite length
Our test for each is as follows:
- For 1), the integral converges if the integrand becomes infinite of a lower order than the first: $$|f(x)| \le \frac{M}{(b-x)^{\mu}} \text{\quad for }\mu<1 $$
- The integral vanishes at infinity to a higher order than the first: $$|f(x)|\le \frac{M}{x^v} \text{\quad for }v>1$$


- The values at the endpoints do not matter and the limit of the integral function and the Riemann sum yield the same value independent of actual value at the endpoints.
	- Equivalency of open and closed interval definition of Rieman limit if the integrand is bounded and continuous within the interval
- Same is true for finite number of points of discontinuity

# Definitions
***Improper Integral.***

# Theorems
***Eqivalence in definition between the proper Riemann sum with arbitrarily defined endpoints and the improper integral.***

***Criterion for convergence over infinite interval of integration.***