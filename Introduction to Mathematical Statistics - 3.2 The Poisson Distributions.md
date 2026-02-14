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