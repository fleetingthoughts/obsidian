---
tags:
  - "#math"
  - "#real_analysis"
  - "#calculus"
date_created: 2026-03-05
parent: "[[Introduction to Calculus and Analysis I]]"
---
In this chapter, Courant defines the integral as a function called the indefinite integral and differentiates it from the definite integrals that were discussed up to this point. The condition and the specific type of continuity of the indefinite integral is derived based on specific conditions.

Up to this point, the integral discussed had a fixed function, and lower and upper limit of integration resulting in a definite value if the limit exists which it must if the function is continuous under the interval of integration. We now allow one of these parameters to vary, namely the upper limit. The integral then becomes a function $\phi (x)$  of the upper limit and is referred to as the indefinite integral of a function $f(x)$ denoted as follows: $$\phi (x) = \int_{\alpha}^{x}f(u)du$$
Some nuances in those notation and things to note are the following:
- As the integral depends on several parameters, the indefinite integral can change depending on what we fix our lower limit $\alpha$ to.
- Remember $du$ is just a notation of the variable to be summed much like $i$ or $j$ in the $\sum$ summations. It simply denotes the symbol to be summed over. 
- Any particular definite integral can be defined in terms of a indefinite interval with a specific $\alpha$ lower limit: $$\int_{b}^{a}f(u)du = \int_{\alpha}^{a}f(u)du +\int_{b}^{\alpha}f(u)du = \phi(a)-\phi(b)$$
- For the above reason, we can also determine any other indefinite integral with a different lower limit in terms of another indefinite integral. Say $\phi (x) = \int_{\alpha}^{x}f(u)du$, then an indefinite integral with a lower limit of $\beta$ is then : $$\int_{x}^{\beta}f(u)du=\int_{\alpha}^{x}f(u)du+\int_{\beta}^{\alpha}f(u)du  = \phi(x)-\phi(\beta)$$
and so since $\alpha$ and $\beta$ were predetermined fixed numbers, all indefinite integrals differ only by a constant assuming the function is continuous over all these intervals of integration.

We can easily determine the continuity of the indefinite integral by invoking the mean value theorem. The difference between $\phi(x)$ and a point $\phi(x_o)$ is given by: $$\phi(x)-\phi(x_o) = \int_{x_{o}}^xf(u)du = f(\xi)(x-x_{o})$$
And so, the mean value theorem guarantees that we can make $|\phi(x)-\phi(x_o)|<\epsilon$ arbitrarily small for any $\epsilon >0$ by making the modulus of continuity $\delta = |x-x_o| < \epsilon/f(\xi)$ and in fact the relationship is of direct proportionality so any indefinite integral is <u>Lipschitz continuous </u> over any closed interval where $f$ is continuous over it (thus guaranteeing the MVT).

