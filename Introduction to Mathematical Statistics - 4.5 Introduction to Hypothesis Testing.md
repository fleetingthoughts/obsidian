---
tags:
  - "#math"
  - "#statistics"
  - "#robert_hogg"
date_created: 2026-03-09
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
In this chapter we answer the following:
- What is a hypothesis test and how is it set up.
- When do we use the test compared to other statistical inferences
- What is the general method to optimize the test (i.e. minimize the probability of making the wrong conclusion in our given scenarios)
- The power function as the function to optimize to minimize errors and how to calculate it. This chapter will not discuss how we can optimize it, but the chapter provides examples on how it is calculated for a given hypothesis test set up.

Along with point estimations, and confidence intervals, another statistical inference procedure is the hypothesis test. Like the confidence interval and point estimators (but not the order statistics), we assume to know the distribution $f(x;\theta)$ of our random variable, $X$, but we try to learn about the unknown parameter $\theta \in \Omega$  which is in some set (that could be all the reals). Given two disjoint subsets of $\Omega$, denoted $\omega_1$ and $\omega_2$ (i.e. $\omega_1 \cup \omega_2 = \Omega$), the hypothesis test tries to determine which of these two subsets our parameter belongs to. We refer to $\theta$ belonging to one of these subsets as the ***null hypothesis***, $H_o$  (say $\theta \in \omega_1$) and we refer to the other as the ***alternative hypothesis*** denoted $H_1$ (the hypothesis that $\theta \in \omega_2$). Generally, the null hypothesis is the "default hypothesis" that is being challenged by the alternative hypothesis. Examples of questions that would be answered by a hypothesis test include:
- Does a procedure cause the mean to increase compared to the default procedure. In this case the parameter to be tested is the average $\mu$ and we are determining where the null hypothesis is the subset of $\omega_1 = {\mu_o}$ which is known and given compared to the challenging procedures which is hypothesis that the average belongs to the subset $\omega_2 \ne \mu_o$. 
The hypothesis test aims to answer these kinds of binary questions.

To help us come to a conclusion on which hypothesis to accept, the criteria we set up is a set in the sample space $C$ called the critical region so that we reject or retain $H_o$ as follos:
- reject $H_o$ (i.e. accept $H_1$) if $(X_1,..X_n)\in C$
- retain $H_o$ (i.e. accept $H_1$) if $(X_1,..X_n)\notin C$ 
We say that a critical region is of size $\alpha$ by looking at the probability of obtaining the statistic in $C$ assuming the null hypothesis is true:

***Definition 4.5.1 (The size of the critical region)*** We say the critical region is of size $\alpha$ if $$\alpha = P_{\theta\in \omega_1}[(X_1,...X_n)\in C]$$
In conducting these tests, there are are 4 different conclusions we can arrive at relative to what is actually true. The goal of the statistician is to set up the test to avoid rejecting the null hypothesis when it is true (called a Type I error) and avoid accepting the null hypothesis when the alternative hypothesis $\theta \in \omega_2$ is correct (called a Type II error). The possible conclusions for a hypothesis test are shown below:
![](Pasted%20image%2020260309234014.png)
Normally the convention is that we want to maintain status quo so the risk of committing a type I error is greater than a type II error. It is generally not possible to minimize both types of error simultaneously, so we put a cap on our type I error and try to minimize the type II error within that constraint. The type I error is capped by setting an $\alpha$ sometimes called the <u>level of significance</u>. By definition 4.5.1, this is the probability we reject the null hypothesis assuming $X$ has distribution $f(x,\theta \in \omega_1)$ (i.e. the null hypothesis is true). With the $\alpha$ set, we now have a choice of how to set up this $C$ so that we minimize the Type II error. The probability of accepting the alternative hypothesis assuming the alternative hypothesis is true based on our choice of $C$ is: $$\gamma_{C}(\theta)=P_{\theta \in \omega_2}[(X_1,...X_n)\in C]$$
Or colloquially, the chance of committing a type II error is the probability that our statistic falls in our choice of $C$ assuming the alternative hypothesis is true (i.e. $X$ has a distribution of $f(x; \theta \in \omega_2)$). Notice also that $P_{\theta \in \omega_2}[(X_1,...X_n)\in C] = 1 - P(Type II Error)$ in the case that the alternative hypothesis is true so the goal to minimize a Type II error is to maximize $\gamma_{C}(\theta)$. This function that we optimize is called the ***power function***. 

And so we now know what our goal is: 
1) We cap our risk of committing a Type I error to $\alpha$ setting our $C$ to a certain size
2) Use our alternative hypothesis and the assumed distribution to construct the power function.
3) Choose how to construct that $C$ in a way that also maximizes the power function while respecting $\alpha$. Hence if we're given two choices $C_1$ or $C_2$ as our critical region both of which have size $\alpha$, we choose the one that maximizes the power function.
Note that in 2) there is the possibility for multiple hypotheses. Generally the null hypothesis is something like 
- $H_o: p = p_o$
which is called a ***simple hypothesis*** because there is only one underlying distribution, but typically the alternative hypothesis is something like:
- $H_1: p<p_o$
Which leads to many different distributions of different parameter $p$ and is called a ***composite hypothesis***.


# Key Concepts and denotation
- The null hypothesis
- The alternative hypothesis
- The critical region and the size of the critical reigion
- Limiting the chance of making a Type I error by setting a critical region of size $\alpha$ 
- The significance level is the maximum probability of committing a Type I error. The significance level is also referred to as the "maximum power of the test when $H_o$ is true". I prefer the former statement because it speaks to underlying probability concepts instead of invoking new terms like "power".
