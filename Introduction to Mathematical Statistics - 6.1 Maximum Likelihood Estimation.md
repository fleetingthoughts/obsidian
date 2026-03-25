---
tags:
  - math
  - statistics
  - robert_hogg
date_created: 2026-03-25
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---

# Definitions
***Assumptions 6.1.1. (The Regularity Conditions).*** Regularity conditions 1-3 are:
1) The cdfs are distinct in that if $\theta \ne \theta' \implies F(x_{i};\theta)\ne F(x_{i};\theta')$. In other words, the cdf definitely changes if the parameter is different
2) The pdfs have a common support for all of $\theta$. This is an important one as there will be models that don't satisfy this
3) The true parameter $\theta_o$ is an interior point in the same set as $\theta\in \Omega$ 
***Definition 6.1.1 (The Maximum Likelihood Estimator).*** We say that a $\hat{\theta}=\hat{\theta}(X)$ is a maximum likelihood estimator of $\theta$ if it is the value where the likelihood function achieves its maximum, that is: $$\theta=Argmax[L(\theta;X)]$$

# Theorems
***Theorem 6.1.1 (The true parameter is the maximum of the likelihood function).*** Assume that $\theta_o$ is the true parameter and that $E_{\theta_o}[f(X_i;\theta)/f(X_i;\theta_o)]$ exists. Then under the regularity assumptions, we observe that: $$\lim_{ n \to \infty }P_{\theta_{o}}[L(\theta_{o}, X)>L(\theta,X)]\text{\quad for all }\theta \ne \theta_{o} $$
