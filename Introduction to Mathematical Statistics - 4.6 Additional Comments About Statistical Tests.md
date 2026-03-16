---
tags:
  - "#math"
  - statistics
  - robert_hogg
date_created: 2026-03-11
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
The two-tailed tests are discussed to distinguish between the way the critical area is constructed from the one-sided tests. It is then noted that the set up of a critical region of size $\alpha$ as a basis to reject or retain a hypothesis is identical to determining a confidence interval with a $1-\alpha$ level of confidence.

Often with discrete random variables and low amount of samples, it is difficult to target a specific critical region of size $\alpha$ in this case. In this case we can try to modify the probabilities by conducting auxiliary tests on top of the samples to fine tune the size of the critical region. For instance, say we had a Poisson distribution with a null hypothesis $H_o=\lambda_{\omega_1}=0.1$ with only 10 samples. If we desired an critical region of size $\alpha =0.05$ we would note that $P(X\ge 3)< 0.05 < P(X \ge 4)$ (the actual probability is $P(X\ge 3)-P(X \ge 4)=0.06$ which is a large gap).  We can then conduct an auxiliary test (say conduct a Bernoulli trial by flipping a coin) with a random variable $W$ with a probability of success being 31/61. We can then use this auxiliary trial to fine tune the size of our critical region by for example then redefining our criteria: $$\text{reject }H_{o} \text{ if } \sum_{1}^{10}x_{i}\ge 4 \text{ or if }\sum_{1}^{10}x_{i}\ge 3 \text{ and }W=1 $$The probability of committing a type 1 error is then: $$P_{H_{o}}(Y \ge 4)+ P_{H_{o}}(Y = 3)P(W=1)$$
which would be our desired significance level. The process of performing auxiliary test to determine whether to reject a hypothesis is referred to as a randomized test. Of course these can seem very ridiculous on paper and are often not done. It often means that two experimenters doing the exact same tests can report different conclusions because one decided on an irrelevant test. 

Rather than reporting the conclusion, a common metric that is reported for a hypothesis test is the $p$-value which is the significance level that would be required to reject an observation. This lets experimenters come to different conclusions depending on their level of tolerance for a Type I error.


