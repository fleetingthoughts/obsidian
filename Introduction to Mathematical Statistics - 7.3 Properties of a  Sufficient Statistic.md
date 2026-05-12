---
tags:
  - statistics
  - probability
  - robert_hogg
date_created: 2026-05-09
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
After developing the definition of a sufficient statistic and ways to identify it, we now look at why sufficient statistics are so useful. In this section, we show that the sufficient statistic helps us determine the minimum variance unbiased estimator (MVUE). We deduce the properties of a sufficient statistic to achieve this goal:
1) The sufficient statistic to estimate a parameter isn't unique
2) The Rao-Blackwell theorem. The use of a sufficient statistic to reduce the variance of another statistic.
3) If a sufficient statistic and unique maximum likelihood estimator (MLE) exists for a parameter, then the MLE is a function of a sufficient statistic
4) A note on a common misconception of using any arbitrary statistic to refine a unbiased parameter emphasizing why we use a sufficient statistic

The first property we note is that a parameter doesn't have a unique sufficient statistic. Given a bijective function $g$ and a known sufficient statistic $Y_1$, then the statistic $Y_{2}=g(Y_1)$ is also a sufficient statistic which can be proven by the Neyman Factorization theorem. Since $Y_1$ is a sufficient statistic, then the likelihood of a random sample can be expressed using the factorization theorem:$$f(x_1,\theta)f(x_2,\theta)...f(x_n,\theta)=k_1(u_1(y_1);\theta)k_2(x_1,...,x_n)$$
Then applying the $Y_1=g^{-1}(Y_2)$ produces a factorization of the statistic $Y_2$ showing that it is also a sufficient statistic.

From [Theorem 2.3.1](Introduction%20to%20Mathematical%20Statistics%20-%202.3%20Conditional%20Distributions%20and%20Expectations.md), we get a sense of how we can improve a statistic by lowering its variance. This is formalized in ***Theorem 7.3.1 (Rao-Blackwell).*** The theorem states that we need the following:
1) A sufficient statistic $Y_1$ 
2) An unbiased estimator $Y_2$
With these two, in our search for the MVUE, we can refine our unbiased estimator by conditioning it with $E(Y_2|Y_1)$. The conditioning produces an improved unbiased estimator with a lower variance that is a function of our sufficient statistic. Usually it is impractical to find both 1) and 2) and we try to short cut a way to find an unbiased estimator. The Rao-Blackwell theorem assures us that there is some function of a sufficient statistic $\varphi(Y_1)$ that has a lower variance, so we instead restrict our search to the functions of a sufficient statistic that is unbiased. Later in chapter 7.4, we will show why restricting the search this way is fruitful.

In our search for the MVUE, we therefore restrict our search to functions of a sufficient statistic that are unbiased, and ***Theorem 7.3.2*** gives us a good place to start: all MLEs of a parameter are functions of a sufficient statistic. While MLEs are not unbiased in general, they are asymptotically unbiased meaning we can usually tweak the MLE in some way to make it unbiased. The next two sections 7.3 and 7.4 then show that in most instances (sufficient conditions to be provided) if we find a function $\varphi(Y_1)$ that is unbiased then it is the only unbiased estimator based on that sufficient statistic. In summary we have a formula to find the MVUE:
- Given a pdf $f(x;\theta)$ and a parameter to estimate, [find the MLE](Introduction%20to%20Mathematical%20Statistics%20-%206.1%20Maximum%20Likelihood%20Estimation.md).
- Determine the expectation of the MLE. The expectation is always asymptotically unbiased
- If we can modify the MLE in a way to make it unbiased, then it is likely the MVUE. It is not always the case that we can modify it in a closed form to make it unbiased.

A common misconception is to assume that by Rao-Blackwell's theorem the unbiased statistic can be conditioned with any arbitrary statistic that isn't necessarily sufficient. The issue is that the function $E(Y_2|Y_1)$ if $Y_1$ isn't sufficient isn't even a statistic because the conditional probability $f_{Y_2|Y_1}=u(X_{1},\dots X_{n},\theta)$ will be a function of the parameter as well so it won't even be a statistic. This causes all previous theorems to fall apart so that $E(Y_2|Y_1)$ cannot be used as an estimator of $\theta$ because it contains $\theta$ itself.

# Summary of concepts
- If there are two sufficient statistics.
# Definitions

# Theorems
***Theorem 7.3.1 (Rao-Blackwell. Refinement of an unbiased estimator into another unbiased estimator with a smaller variance using a sufficient statistic).*** Let $X_1,...X_n$ be a finite random sample with distribution $f(x;\theta)$. Let $Y_1=u(X_1,...,X_n)$ be a sufficient statistic for $\theta$ and $Y_2 = u_2(X_1,...X_n)$ be an unbiased estimator that is not necessarily a function of $Y_1$ alone. Then we have the following:
- $E(Y_2|Y_1)=\varphi(Y_1)$ is an unbiased estimator
- $Var(\varphi(Y_1))\le Var(Y_2)$

***Theorem 7.3.2 (Sufficient conditions for the MLE to be a function of a sufficient statistic).***