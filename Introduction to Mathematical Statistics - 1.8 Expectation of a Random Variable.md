---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - math
  - statistics
  - robert_hogg
date_created:
---
We first define a key term

***Definition 1.8.1 (Expectation)***. If the random variable $X$ is a continuous random variable with a pdf $f(x)$ with the property 
$$\int |x|f(x)dx \lt \infty$$ then the expectation of $X$ is
$$E(X) = \int xf(x)dx $$ If $X$ is a discrete random variable with pmf $p(x)$ and the property
$$\sum_{x} |x|p(x) \lt \infty$$
then the expectation of the discrete random variable $X$ is
$$E(X)=\sum_{x} xp(x)$$
$E(X)$ must converge to an actual real number given the absolute convergence of the sums.

We can also compute the expectation of a transformation if it satisfies some properties:
***Theorem 1.8.1 (The expectation of a transformation of a continuous random variable).*** Let $Y=g(X)$ be a transformation of a continuous random variable
1) If the following property is satisfied $\int_{\infty}^{\infty} g(x)f_{X}(x)dx \le \infty$ then the expectation is
$$E(Y)=\int_{\infty}^{\infty} g(x)f_{X}(x)dx$$
The proof for the continuous case here requires some advanced real analysis.

Theorem 1.8.1 is sometimes referred to as the law of the unconscious statistician (naming attributed to Sheldon Ross's probability textbook) and is sometimes used as the definition of expectation instead of what we had for definition 1.8.1.

Armed with the tool to compute the expectation of a transformation of a random variable given that it converges, we can now determine the expectation of any linear combination of transformations of a random variable:

***Theorem 1.8.2 (The Linearity of Expectations).*** given transformations of $X$ , $g_1(x)$ and $g_2(x)$ with known expectations, then for any constants $k_1$ and $k_2$, the expectation of a linear combination of the transformations is follows:
$$E[k_{1}g_{1}(x)+k_{2}g_{2}(x)]= k_{1}E[g_{1}(x)]+k_{2}E[g_{2}(x)]$$
It is worth noting that the expectation of a constant, $c$, is simply the constant itself:
$$E(c)=c$$
