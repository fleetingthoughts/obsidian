---
tags:
  - math
  - statistics
  - robert_hogg
date_created: 2026-03-18
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
This section looks at convergence property of random variables and uses it to describe the consistency of a predictor. The section is outlined as follows:
- Definition of convergence in probability
- Conditions governing how random variables converge to the values they predict: the Weak Law of Large Numbers
- Convergence as a condition to show the conditions which a predictor approaches the value its predicting.
Statistical inferencing aims at approximating as best we can, the parameters and variables of interest. To describe how well our inferences estimate, we must make use of convergence properties. The two essential converges are convergence in probability and distribution and this section focuses on the former and show how this property produces a desirable property in our estimators

***Definition 5.1.1*** defines convergence in probability in terms of a sequence. Convergence in probability essentially shows the value that the sequence will take for large enough $n$. If they have identical values, then the probabilities will be the same. A couple things to demonstrate convergence in probability:
- $a_n \xrightarrow {P} a$ is equivalent to showing that $\lim\limits_{ n \to \infty } a_n = a$. 
- Chebyshev's theorem can be used in the 2nd definition of Convergence in probability. Chebyshev's theorem produces an upper bound for the probability of the random variable which we can be used to see if the probability can be "squeezed" to 0 (squeeze theorem).
An application of the Chebyshev's theorem to prove convergence is used in the Weak Law of Large Numbers (WLLN) which shows that the sample average converges to the true average as we increase the sample size to infinity. Because the Chebyshev's inequality assumes a finite 2nd moment ($\sigma$ gets used in the inequality), it is called the "weaker" version compared to a stronger law outside the scope of this book that proves the same thing assuming only the existence of the first moment of the random variable.

The reason we defined this convergence in probability is because there are two properties in point estimators that we are focused on: unbiasedness and consistency. Consistency defined in ***Definition 5.1.2 (Consistency)*** is a property of an estimator to converge in probability to the parameter it estimates as the sample size increases. Essentially our estimator can become arbitrarily close to the parameter. The Weak Law of Large Numbers showed that the sample average is a consistent estimator of the true average using Chebyshev's inequality. We can use Chebyshev's again to show the Bessel corrected sample variance (it also holds for the uncorrected too) is a consistent estimator of $\sigma^2$ as well. The proof will require us to show that the second moment converges in probability: $$\frac{1}{n-1}\sum_{i-1}^nX_{i}^2 \xrightarrow{P}E(X^2)$$
Do note that by invoking Chebyshev's inequality to prove above, we have to assume the 4th moment is finite (analogous to how the WLLN assumes the 2nd moment).


# Definitions
***Definition 5.1.1 (Convergence in Probability).*** Let $(X_n)$ be a sequence of random variables, we say that the sequence converges in probability to another random variable $X$, if for any arbitrary $\epsilon >0$:$$\lim_{ n \to \infty } P(|X_n-X|<\epsilon)=1$$
This is denoted $X_n \xrightarrow{P} X$. The above probability is equivalently stated as :
$$\lim_{ n \to \infty } P(|X_n-X|>\epsilon)=0$$
The above formulations allows us to use Chebyshev's inequality.

***Definition 5.1.2.*** Let $X$ be a random variable with the pdf $F(x, \theta)$ where $\theta \in \Omega$. Let $X_1,...,X_n$ be a random sample of $X$, with $T_n$ being a statistic on this sample of size $n$. The statistic $T_n$ is called a consistent estimator of $\theta$ if it converges in probability to the parameter: $T_n \xrightarrow{P} \theta$ 
# Theorems
***Theorem 5.1.1 (Weak Law of Large Numbers).*** Let $(X_n)$ be a sequence of iid random variables having common mean $\mu$ and variance $\sigma^2<\infty$. Let $\bar{X_n}=n^{-1}\sum\limits_{i=1}^nX_i$. Then $(X_n)$ converges in probability to $\mu$:
$$\bar{X_n}\xrightarrow{P} \mu$$

***Theorems 5.1.2-5.1.4 (Fundamental properties of convergence in probability).*** Sequences of random variables that converge in probability have the usual algebraic properties, that is assuming $(X_n) \xrightarrow{P} X$ and $(Y_n)\xrightarrow{P} Y$, we have:
- $X_n+Y_n \xrightarrow{P} X+Y$
- $aX_n \xrightarrow{P} aX$
- Given a function $g$ that is continuous in the support of $X_n$ and $X$ then: $g(X_n) \xrightarrow{P} g(X)$ 
- $X_nY_n \xrightarrow{P} XY$ 