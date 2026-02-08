---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#statistics"
  - "#robert_hogg"
  - "#math"
date_created: 2026-02-06
---
We now transfer our understanding of single-variable probability distributions to multivariate distributions. A lot of this chapter is getting used to the notation once we move multi-dimensions.

***Definition 2.1.1. (Random Vector).*** Given a sample space $C$ of a random experiment, if we have two random variables $X_1, X_2$ that map every element of the sample space onto real numbers such that given the element $c$, we have functions $X_1(c) = x_1$ and $X_2(c) = x_2$. We then say the ordered pair of random variables $(X_1, X_2)$ is the random vector and the space, $D$, of $(X_1, X_2)$ is the set of all ordered pairs $D = \{(x_1,x_2): x_1 = X_1(c), x_2= X_2(C), c \in C\}$.

Similar to the univariate random variables, we can define the probabilities of a random vector, $P_{X_1,X_2}$ in terms of the cdf:
$$F_{X_1,X_2}(x_1,x_2) = P[(X_1 \le x_1) \cap (X_2 \le x_2)]$$
Hence, the probabilities of all events of the form $(x_1, x_2] \times (x_3,x_4]$ can be determined. Note how the intersection of the ordered pairs is right inclusive (see definition of cdf from 1.5).