---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#robert_hogg"
  - "#statistics"
date_created: 2026-02-09
---
In [Introduction to Mathematical Statistics - 2.1 Distributions of Two Random Variables](Introduction%20to%20Mathematical%20Statistics%20-%202.1%20Distributions%20of%20Two%20Random%20Variables.md), we had shown how to obtain the univariate random variable from a joint distribution when the other variable is allowed to be anything. We now consider the case where the other variable assumes a specific value or range of values resulting in the conditional probability distribution of the original joint distribution.

We first discuss the discrete case. Assuming the joint distribution function of the discrete random variables $p_{X_1,X_2}(x_1,x_2)$ with their respective marginal distributions $p_{X_1}(x_1)$ and $p_{X_2}(x_1)$, we wish to find the probability at $x_2$ given an $x_1$. We the define this conditional probability distribution function in a way that can be reduced to our [original definition of the conditional probability](Introduction%20to%20Mathematical%20Statistics%20-%201.4%20Conditional%20Probability%20and%20Independence.md):
$$P(X_{2}=x_2 |X_{1}=x_1)  = \frac{P(X_2 = x_2, X_1=x_1)}{P(X_1 = x_1)}$$
$$p(x_2 |x_1) = \frac{p_{X_{1}X_{2}}(x_2,x_1)}{p_{X_{1}}(x_1)}$$

We denote the function on the left-hand of the inequality as $p_{X_2|X_1}(x_2|x_{1})$ or $p_2(x_2)$ . Note that it is a univariate function in $x_2$. It can be shown that this is a probability distribution function as it must necessarily be nonnegative by the numerator and denominator of its definition being assumed as positive and its sum over all possible $x_2$ equates to 1.

In the continuous case, we find that for the conditional probability distribution of $X_2$ given a fixed $X_1$:
$$f_{X_2|X_1}(x_2|x_1) = \frac{f_{X_2,X_1}(x_1,x_2)}{f_{X_1}(x_1)}$$
and this similarly satisfies the conditions of the pdf by being non-negative and summing to 1 over $x_2$. The conditional pdf on the left-hand of the equality can be abbreviated to $f_2(x_2)$.

As it is a proper pdf, the expectation of the conditional pdf, $f_2(x_2)$  can be determined and is referred to as the conditional expectation of a function, $u(X_2)$ given $X_1 =x_1$.
$$E[u(X_2)|x_1]=\int_{-\infty}^{\infty}u(x_2)f_2(x_2)dx_2$$Notice that in reality, the conditional expectation is a function of the "fixed" $x_1$ so instead of being a constant, it is actually a random variable itself. The conditional variance can also be analogously and it too is a function of the fixed random variable. 

We derive some useful properties of the conditional expectation and variance.

***Theorem 2.3.1. (Properties of the expectation and variance of conditional expectation and conditional variance).*** Let $(X_1,X_2)$ be a random vector such that the variance of the $X_2$ (should be the marginal distribution) is finite so then by [Theorem 1.10.1, the expectation must exist as well](Introduction%20to%20Mathematical%20Statistics%20-%201.10%20Important%20Inequalities.md). Then we have:
1) $E[E(X_2|X_1)]=E(X_2)$ (note that $E(X_2|X_1)$ is the expectation of $X_2 = x_2$  a function of $X_1$)
2) $Var[E(X_2|X_1)] \le Var(X_2)$ 
The proof for 1) can be determined straight from the definitions of the expressions of the left-hand and right-hand side of the equalities.

Theorem 2.3.1 can be interpreted and applied as follows. If we wanted to determine the mean of the random variable $X_2$ we can look to sample $X_2$ or $E(X_2|X_1)$, but we would lean more to the latter because by 2) the variance is smaller and can lead to a better estimation. The downside is we're likely doing more testing because we're sampling random samples of $X_2$ for multiple different $X_1 = x_{1}$ .