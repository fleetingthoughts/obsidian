---
tags:
  - math
  - probability
  - statistics
  - robert_hogg
date_created: 2026-05-15
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
The previous chapters looked at determining the MVUE of the parameter from a well-known distribution. We determine the MVUE of a function of a parameter if we know the MVUE of the parameter itself. We look at two different techniques and one method to estimate the standard error of an MVUE:
1) Modifying the expected value of the function of the parameter. 
	- Determine the asymptotic distribution of the MVUE of a function of a parameter using the mle. This method is not guaranteed to work.
2) Use the conditional distribution given a sufficient statistic.
3) Emphasize the MVUE is a heuristic and not a given theorem. Generally, we want an estimator that has the lowest variance, but the MVUE can be an undesirable statistic useless for our purposes.
4) Bootstrap methods to estimate the standard error of an estimator including the MVUE.


Using [Theorem 7.3.2](Introduction%20to%20Mathematical%20Statistics%20-%207.3%20Properties%20of%20a%20%20Sufficient%20Statistic.md), we know the mle is a function of a sufficient statistic. While not guaranteed, we can determine a relationship between the mle and MVUE and obtain the asymptotic distribution of the MVUE of a function of a parameter from the asymptotic distribution of the mle

# Bootstrap methods to estimate the standard error of an estimate
The standard error of an estimator $\hat{\theta}$  is nonparametrically determined by the bootstrap method meaning we make no assumptions of the pdf $f(x;\theta)$. The heuristic is to take a random sample and treat it as a new population that mimics the properties of the true population we sampled from. Sampling from the true population can be expensive, so can instead use a computer to "artificially" produce new random samples: 
1) We sample with replacement from our random sample. This is referred to as a bootstrap sample and the standard method samples with replacement the same number of times as the original sample from the true population.
2) Calculate the new estimator with that sample
3) Repeat 1)-2) as $x$ times to produce $x$ different estimated values from the realization of each bootstrap sample.
4) Calculate the Bessel corrected sample variance of our $x$ estimated parameters to produce an estimate of the standard error of the estimator.

