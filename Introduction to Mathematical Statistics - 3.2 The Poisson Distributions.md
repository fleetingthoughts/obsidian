---
parent: "[[Introduction to Mathematical Statistics 8th ed. - Hogg, McKean, Craig]]"
tags:
  - "#math"
  - "#statistics"
  - "#robert_hogg"
date_created: 2026-02-13
---
The Poisson random variable is a discrete one that has the following distribution:
$$p(x) = \frac{-\lambda^xe^{-\lambda}}{x!}$$
where $x = 0,1,2,3,..$ is a natural number and the probability is 0 anywhere else. To demonstrate a lot of the properties of the Poisson distribution, we make use of the series expansion for all real numbers $z$
$$e^z = 1+z+\frac{z^2}{2!}\frac{z^3}{3!}\dots=\Sigma_{x=0}^{\infty}\frac{z^x}{x!}$$
The mgf determined to be
$$M(t)=\Sigma_{x=0}^{\infty}e^{tx}p(x)$$
$$M(t)=e^{\lambda(e^t-1)}$$
From the mgf, we have the mean ($\mu = \lambda$) and the variance ($\sigma^2=\lambda$ )
It can be shown that given a random variable $X_t$ with parameter $t$ denote the # of occurrences within an interval $(0,t]$ with the pmf $P(X_t=k)=g(k,t)$, then $X_t$ has the Poisson distribution has these 3 properties:
1) <u>Homogeneity property</u>: $g(1,h) = \lambda h + o(h)$. The $o(h)$ notation is an error term that has $\frac{o(h)}{h} \to 0$  as $h \to 0$, that is, 
$$\\lim_{ h \to 0 } \frac{g(1,h)}{h}=\lambda$$Intuitively, what this means is that the probability a singular event occurring is directly proportional to some $\lambda$ constant with respect to $h$ (which can represent something like time)
2) <u>non-concurrence</u>: $\Sigma_{t=2}^{\infty}g(t,h) = o(h)$. This states that the probability of two or more events occurring goes to 0 as $h\to 0$. What this intuitively means is that events can occur simultaneously and that you can only have 1 or no events occur at an instant.
3) The number occurrences in nonoverlapping intervals are independent of one another.
The author then [shows how we can derive the Poisson distribution from the axioms of a Poisson process](Derivation%20of%20the%20Poisson%20distribution%20from%20a%20Poisson%20Process.md)

The book does not explain this, but note that axiom 1) implies stationarity, that is the Poisson process does only depends on the length of $h$ and not on the start time. Also 1) together with 2) imply that to satisfy the properties of a probability set function we must have for the probability of no events occurring, $g(0,h)=1-\lambda h+o(h)$ 

It is then proven that the [[Sum of random variables with a Poisson distribution is itself a Poisson distribution]]. <u>Note that in general, a linear combination of Poisson distributed random variables is not a Poisson distribution itself (i.e. the coefficients must be 1)</u>
***Theorem 3.2.1 (Sum of Random variables with a Poisson distribution).*** Suppose $X_1,  X_2,..,X_n$ are random variables with a Poisson distribution each with a corresponding parameter $\lambda_i$. If $Y= \Sigma^{\infty}_{i=1}X_i$, then $Y$ is a Poisson distribution with the parameter $Y= \Sigma^{\infty}_{i=1}\lambda_i$ 

