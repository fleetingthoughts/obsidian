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
- Demonstration of predictors converging to the values they predict: the Weak Law of Large Numbers
- Convergence as a condition to show the conditions which a predictor approaches the value its predicting.

# Definitions
***Definition 5.1.1 (Convergence in Probability).*** Let $(X_n)$ be a sequence of random variables, we say that the sequence converges in probability to another random variable $X$, if fo
# Theorems
***Theorem 5.1.1 (Weak Law of Large Numbers).*** Let $(X_n)$ be a sequence of iid random variables having common mean $\mu$ and variance $\sigma^2<\infty$. Let $\bar{X_n}=n^{-1}\sum\limits_{i=1}^nX_i$. Then $(X_n)$ converges in probability to $\mu$:
$$\bar{X_n}\xrightarrow{P} \mu$$

***Theorems 5.1.2-5.1.4 (Fundamental properties of convergence in probability).*** Sequences of random variables that converge in probability have the usual algebraic properties, that is assuming $(X_n) \xrightarrow{P} X$ and $(Y_n)\xrightarrow{P} Y$, we have:
- $X_n+Y_n \xrightarrow{P} X+Y$
- $aX_n \xrightarrow{P} aX$
- Given a function $g$ that is continuous in the support of $X_n$ and $X$ then: $g(X_n) \xrightarrow{P} g(X)$ 
- $X_nY_n \xrightarrow{P} XY$ 