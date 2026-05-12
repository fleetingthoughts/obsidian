---
tags:
  - math
  - statistics
  - probability
  - robert_hogg
date_created: 2026-05-11
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
---
The Rao-Blackwell theorem produces a way to refine an unbiased statistic which narrows our search of the MVUE to functions of a sufficient statistic $\varphi(Y_1)$. But how do we know which functions of $Y_1$ are the best one? Rao-Blackwell does not guarantee a unique MVUE. To ensure uniqueness, we require a sufficient statistic that is complete. Any unbiased function of a complete and sufficient statistic is uniquely the MVUE.
1) The sufficient conditions for uniqueness of the unbiased statistic that is a function of $Y_1$.
2) Define a property of the pdf of the sufficient statistic that is needed to make $\varphi(Y_1)$ unique called completeness.

So by Rao-Blackwell, we know the MVUE must be some function of a sufficient statistic $Y_1$. For if there was an unbiased estimator $Y_2$ that isn't solely a function of $Y_1$, then we can refine it by $E[Y_2|Y_1]=\varphi(Y_1)$. 

Lets assume we have a sufficient statistic $Y_1=u(X_1,...X_n)$ with the pdf $f_{Y_1}(y_1;\theta)$ and say we have two functions of $Y_1$ say $\varphi(Y_1)$ and $\psi(Y_1)$ that are both unbiased estimators of the parameter $\theta$. Then we have the following relationship: $$E[\varphi(Y_1)-\psi(Y_1)]=\int_{-\infty}^{\infty}[\varphi(y_{1})-\psi(y_{1})]f_{Y_{1}}dy=0$$
Here is the spark of creativity. What if the pdf of $Y_1$ has the property that the only way for the expectation $E[u(Y_1)]=0$ for any function $u$ in general to be 0 is if $u(y_1)$ is identically 0 on the support of $f_{y_1}$. If the pdf has such a property for all possible $\theta$, then any unbiased estimator that is solely a function of $Y_1$ must be identical to each other on the support of $Y_1$ in order for the difference of their expectations to be 0, and so, $\varphi(Y_1)$ is unique. We call such a property of the pdf completeness and define it in ***Definition 7.4.1.***

In summary, if a sufficient statistic $Y_1$ is  complete, then any function $\varphi(Y_1)$ that is unbiased is unique and cannot be refined by Rao-Blackwell so it is the MVUE which was furnished by Lehmann and Scheffe in ***Theorem 7.4.1***. 

# Computational summary
- ***Find the MVUE of an unknown parameter of a known pdf given a sufficient statistic $Y_1$.***This will depend on what else we have:
	1) If we have an unbiased estimator
		1) Determine if its a function solely of a sufficient statistic because otherwise we can refine it by the Rao-Blackwell theorem.
		2) Determine if the sufficient statistic is complete. If it is, then the refined unbiased estimator that must be solely a function of our sufficient statistic $Y_1$ is the MVUE
	2) If we have a function of the sufficient statistic:
		1) Determine if it is unbiased
		2) If it is unbiased, then we have found our MVUE. Otherwise, see if we can modify it to become unbiased
	3) If we do not have anything
		1) Determine the MLE.
		2) The MLE must be a function of the sufficient statistic by [Theorem 7.3.2](Introduction%20to%20Mathematical%20Statistics%20-%207.3%20Properties%20of%20a%20%20Sufficient%20Statistic.md).
		3) Determine if the MLE is unbiased and see if we can modify if it isn't.

# Definitions
***Definition (Completeness).***

# Theorems
***Theorem 7.4.1 (Lehmann and Scheffe).***


