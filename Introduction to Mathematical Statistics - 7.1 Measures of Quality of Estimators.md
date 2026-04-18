---
tags:
  - math
  - statistics
  - robert_hogg
date_created: 2026-04-18
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
Chapters 4 and 6 developed properties of point estimators that were desirable to us such as the consistency of MLEs and unbiasedness, which MLEs do not necessarily have though they are asymptotically unbiased (***Theorem 6.2.2***). These previous chapters touched on desirable qualities of estimators and some methods that produce estimators with these desirable qualities, but we now furnish a method that lets us compare between these estimators beginning with point estimation. 

This chapter introduces heuristics to compare point estimators using the idea of risk. The chapter is outlined as follows:
- The statistics variance as the criteria for the best estimator: The MVUE
- Alternative criteria to choose between point estimators using: the use of deviations of a point estimator statistic from the true parameter using another statistic called the loss function
- A comparison of point estimators using the risk function which is the expected value of the loss function.
- Introduce heuristics and criteria to make a decision based on a comparison of the risk function between estimators
The chapter does not contain many concrete computations and is a general philosophic and practical guideline to compare different point estimators.

The scenario in question is the same as the sections for MLE point estimators: we assume the general form of the pdf of a random variable of interest with an unknown parameter of interest that we estimate. The chapter at two scenarios where we choose between point estimator candidates:
- Scenario 1: The statistics are all unbiased and we choose the statistic with the smallest variance, namely, we choose the statistic that is the minimum variance unbiased estimator (MVUE). This is the simplest of the two and is simply determining the variance of the estimators and choosing the smallest one
- Scenario 2: the statistic is categorized by its deviation from the true parameter called the loss function which depends on the possible parameter values $\theta \in \Omega$ and the candidate statistic. This method takes the longest explanation
We shall expand on scenario 2 which consists of several components:
- The decision function which "decides" the value of our point estimate of the parameter of interest $\theta$. In this context it is essentially a statistic
- The loss function that is a measure of the deviation of the decision function from the "correct decision" or the true parameter
- The risk function that is the expected value of the loss function
- A decision criteria that takes the value of the risk function and chooses between the candidates
Of these 4 components, we have several heuristics for the loss function and the decision criteria.

Some common loss functions $\mathcal{L}(\theta,\delta)$ include
- The squared-error loss function
- The absolute-error loss function
- The goalpost loss function

Regarding the decision criteria, three are discussed with one of them essentially being the MVUE showing that the risk function heuristic can reduce to the MVUE:
- The <u>minimax principle </u>which selects the decision function, or statistic in this context, that has minimizes the maximum risk. In other words, we choose the statistic $\delta_o(y)$ with the smallest expected value of its loss compared to all the other $\delta(y)$ decision functions for all possible values of $\theta$. We therefore look at what value the risk function gets maximized by all possible values of the true parameter $\theta$ and select the decision function $\delta_o(y)$ that has the smallest maximum compared to the others: $$\max\limits_{\theta}R[\theta ,\delta_o]\le \max\limits_{\theta}(\theta,\delta)$$The decision function chosen this way is called the <u>minimax decision function</u>
- If we restrict our selves to decision functions such that $E[\delta(y)]=\theta$ (i.e. unbiased) and use the loss function $\mathcal{L}(\theta,\delta)=[\theta-\delta(y)]^2$ then the decision function that minimizes the risk function is effectively the one with the smallest variance and is effectively the MVUE.
- The <u>minimum mean-squared-error estimator </u> chooses the decision function that isn't necessarily unbiased that minimizes the same risk function $E[(\theta-\delta(y))^2]$ . The minimum mean-squared-error estimator reduces to the MVUE if we restrict the decision function to being unbiased.

# Definitions
***Definition 7.1.1 (The MVUE).***
***Definition (Decision Rule).***
***Definition (Loss Function).*** 
***Definition (Risk Function).***
# Theorems
