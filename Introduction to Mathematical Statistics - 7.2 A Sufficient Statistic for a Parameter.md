---
tags:
  - math
  - statistics
  - probability
  - robert_hogg
date_created: 2026-04-29
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
For the past few chapters, we've performed inferences and hypothesis testing on statistics that were arbitrarily conjured up as if they were known to be good statistics to look at. We now clear up the arbitrariness by examining one of the properties of statistics called sufficiency when estimating the unknown parameter of a random variable with a known distribution. The next chapters will explore why sufficiency is a desirable property when estimating a parameter.

We first provide an intuitive notion of sufficiency before providing the technical definition of sufficiency and the book provides examples of two different ways to determine whether a statistic is sufficient:
- Directly determine whether a statistic is sufficiency from the definition of sufficiency
- Using Neyman's factorization theorem to determine sufficiency without knowing the pdf of the statistic.

Sufficient statistic is one where the random variable is independent of the statistic. The reason why this is valuable is it means all the information in the statistic used to estimate the parameter is contained in the $u(x_1,...,x_n)$ statistic and the particular details about the $x_i$ do not matter. 


# Definitions

***Definition 7.2.1 (Sufficient Statistic).*** Let $X_1,..,X_n$ be a random sample with the realization $x_1,...,x_n$ with pdf $f$ with parameter $\theta$ and $Y=u(X_1,...X_n)$ be a statistic with the pdf $f_Y$. The statistic $Y$ is called a sufficient statistic for $\theta$ if the conditional probability of $P(X_{1}=x_{1},\dots,X_{n}=x_{n}|Y=u(x_{1},\dots x_{_{n}}))$ is independent of $\theta$: $$\frac{f(x_1;\theta)...f(x_n;\theta)}{f_Y(u(x_1,...x_n);\theta)}=h(x_1,...,x_n)$$
# Theorems

***Theorem 7.2.1 (Neyman's Factorization Theorem).*** Let $X_1,..,X_n$ be a random sample with the realization $x_1,...,x_n$ with pdf $f$ with parameter $\theta$ and $Y=u(X_1,...X_n)$ be a statistic. The statistic $Y$ is a sufficient statistic if the likelihood function of the random sample can be factored into two nonnegative function $k_1, k_2$: 
$$f(x_1;\theta)f(x_2;\theta)...f(x_n;\theta)=k_1(u(x_1,...x_n);\theta)k_2(x_1,..x_n)$$
where $k_1$ is a function of the statistic and $\theta$ and $k_2$ is independent of $\theta$.
