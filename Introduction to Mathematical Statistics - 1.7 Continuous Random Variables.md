---
dv_parent: "[Introduction to Mathematical Statistics - 1 Probability and Distributions](Introduction%20to%20Mathematical%20Statistics%20-%201%20Probability%20and%20Distributions.md)"
---
tag: #math #statistics #robert_hogg
parent:: [Introduction to Mathematical Statistics - 1 Probability and Distributions](Introduction%20to%20Mathematical%20Statistics%20-%201%20Probability%20and%20Distributions.md)

We could get an intuitive sense of what variables should be discrete random variables by determining whether the sample space is countable or finite, but we look to the actual property of the CDF to distinguish a continuous random variable

***Definition 1.7.1 (Continuous Random Variables).*** A random variable is a continuous random variable if its cumulative distribution function is a continuous function for all $x \in R$.

This definition seems to be a consequence of the fact that if the sample space isn't countable and it is "greater" than it must extend to the set of all real numbers as there's no continuum of cardinality between the set of natural numbers and real numbers. 

If the continuous random variable is absolutely continuous, then we can integrate its probabilities to obtain the CDF.

The <u>support </u> of the continuous random variable $x \in X$ is analogous to the definition for discrete variables where it all the points $x$ such that $p(x) \gt 0$ . By definition of the CDF, we can derive two properties of the pdf:
1) $p_x(x) \ge 0$ 
2) $\int_{\infty}^{\infty} p_x(t)dt = 1$ 
Outside of the scope of this book but it can be shown solely that if a function satisfies both these properties than it is a pdf for a continuous random variable 

## 1.7.1 Quantiles
We define some ways to characterize thresholds within the CDF
***Definition 1.7.2 (Quantile).*** Given a number $0\lt p \lt 1$, the quantile of order $p$ of the distribution of a random variable $X$ is a value $\gamma$ such that $P(X \lt \gamma) \le p$ and $P(X \lt \gamma) \ge p$. It is also known as the (100p)th percentile of $X$ 

## 1.7.2 Transformations
Transformations of a random variable are themselves random variables and we can determine what the pdf or CDF becomes if we know the pdf of the original random variable. Unlike with the discrete random variable, the continuous random variable is defined by its CDF. Usually we have the CDF of the continuous random variable instead and try to relate it to the transformed random variable.

***Theorem 1.7.1 (Determining the pdf of the transformation of a random variable).*** Let $X$ be a continuous random variable with the pdf $f_X(x)$ and support on $S_X$. Let $Y = g(X)$, where $g(x)$ is a 1-1 differentiable function, on $S_X$. Then the pdf of $Y$ is the following:
$$ f_{Y}(y)=f_{X} (g^{-1}(y))|\frac{dx}{dy}|$$
Compare the result against the transformed random variable for a [discrete random variable](Introduction%20to%20Mathematical%20Statistics%20-%201.6%20Discrete%20Random%20Variables.md) and notice how we do not have the $|\frac{dx}{dy}|$ term. Intuitively in the discrete case, we are..well summing up discrete values, but in the continuous case, we are summing up an entire "space" and must take into account the stretching that occurs when we transform the variable. Because the support for a discrete distribution consists of a set of discrete points each with a probability _mass_.  A transformation which maps the points one-to-one to another set of discrete points won't affect the probability _mass_ measure no matter if the points are spread further apart or pushed close together (unless they are _folded_ onto one another). However, the support for a continuous distribution consists of a continuous interval whose points have probability _density_.  So a transformation which maps that interval one-to-one may involve _stretching or squeezing_, and hence affect the probability density of the new interval. The chain rule is how we account for this.

Proof. Apply the chain theorem:
$$ F_{Y}(y)=P(Y \le y) = P(g(X)\le y) = P(X \le g^{-1}(y)) = F_{X}(g^{-1}(y))$$
Therefore to obtain the PDF of $Y$ is then: $$f_Y(y) = \frac{d}{dy}F_Y(y) = \frac{d}{dy}F_{X}(g^{-1}(y)) = f_{X}(g^{-1}(y)\frac{d}{dy}g^{-1}(y)$$
or more summarily:
$$f_Y(y)=f_X(g^{-1}(y))\frac{dx}{dy}$$ 
The absolute value arises from us restricting the transformation to be invertible. The absolute value may just be for obvious convenience because it is necessarily positive. The last term of the theorem $|\frac{dx}{dy}|$ which is equal to $\frac {d}{dy}g^{-1}(y)$ is referred to as the Jacobian of the transformation $x = g^{-1}(y)$ 

From this proof, we establish the algorithm to find the transformed variable $Y = g(X)$:
1) Find the support of $Y$ based on $X$
2) Solve for $x$ in terms of $y$; therefore obtaining $x = g^{-1}(y)$ 
3) obtain $\frac{dx}{dy}$
4) obtain the pdf of $Y$ which is $f_Y(y)=f_X(g^{-1}(y))\frac{dx}{dy}$ 
