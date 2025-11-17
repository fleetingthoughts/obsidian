---
parent: "[[Introduction to Mathematical Statistics - 1 Probability and Distributions]]"
tags:
  - math
  - statistics
  - robert_hogg
date_created:
---
First defining a discrete random variable

***Definition 1.6.1 (Discrete Random Variable)***. We say a random variable is a discrete random variable if its space is either finite or countable. ^def-1-6-1

***Definition 1.6.2 (Probability Mass function (pmf)).*** Let $X$ be a discrete random variable with space $D$, then the probability mass function (pmf) of $X$ is given by:
$$p_X(x) = P(X=x)$$
Note that by the properties of probability functions, it must satisfy the two properties:
1) $0 \le p_X(x) \le 1$ 
2) $\sum_{x \in D}p_X(x) = 1$ 
Outside the scope of this book, but more advanced techniques can show that if a function satisfies the above two properties for a discrete set $D$  then this function can uniquely determine the distribution of the random variable.

The <u>support</u> of the discrete random variable is defined as the $x \in X$ such that $P(x) \gt 0$ or basically the set of real numbers that actually matter and have a chance of occurring. It can be shown that if a point $x$ is not in the support of $X$ then the CDF of $X$ is continuous at this $x$ using [Theorem 1.5.3](Introduction%20to%20Mathematical%20Statistics%20-%201.5%20Random%20Variables.md)

# 1.6.1 Transformations

We aim to describe the PMF and CDF of a random variable $Y = g(X)$ that is a transformation of the original random variable $X$. The space of $Y$ is therefore $D_Y = \{g(x): x \in D_X\}$. In describing the PDF and CDF of $Y$ we consider two cases: 

1) the transformation is one-to-one (injective) then there exists an invertible function such that PMF is:
$$p_Y(y) = P(Y= y) = P(g(X) = Y) = P(X = g^{-1}(y))= p_X(g^{-1}(y))$$
Note the book mentions that this is possible if the transformation is injective, but they probably meant bijective for $g(X)$ needs to map to every possible value in the codomain $Y$ so that $g^{-1}(Y)$ has a mapping for every $Y \to X$  invertible function to exist.
2) If the transformation $g(x)$ is not one-to-one, we try to restrict the domain so that it is one-to-one.

