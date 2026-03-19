---
tags:
  - richard_courant
  - "#math"
  - calculus
  - real_analysis
date_created: 2026-03-03
parent: "[[Introduction to Calculus and Analysis I]]"
---
The chapter goes through the following properties of integrals:
- Additivity of intervals of integration for the same function
- Additivity of functions over the same intervals of integration
- The Mean Value Theorem of Integral Calculus. This point takes the longest and is what will be expanded on.
The Mean Value Theorem (MVT) of integrals results from two basic motivations: 1) to determine a least and lower bound estimate of the integral over the interval $[a,b]$ and 2) to expand the concept of the arithmetic mean of finite quantities to infinite quantities.

In assuming the Riemann integral of $f(x)$ exists over the interval $[a,b]$, we assume that $f(x)$ is a continuous function on a closed interval and is therefore bounded above and below. If $M$ is the upper bound and $m$ the lower bound, then we can obtain an estimate of the Riemann integral: $$ \begin{gather*} m \le f(x) \le M \\
\lim_{n\to \infty}\sum_{i=1}^nm(x_{i}-x_{i-1}) \le \lim_{n\to \infty}\sum_{i=1}^nf(\xi_{i})(x_{i}-x_{i-1}) \le \lim_{n\to \infty}\sum_{i=1}^nM(x_{i}-x_{i-1}) \\
m(b-a)\le \int_{a}^b f(x)dx \le M(b-a)

\end{gather*}
$$
Moving onto the arithmetic mean, the arithmetic mean for a finite number of quantities $f_1, f_2,... f_n$ is defined by: $$\frac{f_{1}+f_{2}+\dots+f_{n}}{n}$$
We can extend this to the arithmetic mean of infinite quantities using the Riemann integral as it is an infinite sum: $$\begin{gather} 
\mu = \frac{f(x_1)+...+f(x_n)}{n} = \frac{1}{b-a} \lim_{n\to \infty}\sum_{i=1}^nf(\xi_{i})(x_{i}-x_{i-1}) \text{\quad where  }x_{1}=a; x_{n}=b & \\
\mu = \frac{\int_{a}^b f(x)dx}{\int_{a}^bdx}

\end{gather}$$
As the integral must exist for a continuous function, this has a finite value $\mu$. 

Now combining our results on the estimate for the Riemann integral with the existence of our newly defined mean of $f(x)$ on $[b,a]$ we find that $m \le \mu \le M$. As $f(x)$ has the values $m$ and $M$ somewhere in $[a,b]$, by the intermediate value theorem, this means there is some $x=\xi$ that lies somewhere in the $[a,b]$ interval such that $f(\xi)=\mu$. Stated more formally

***Mean Value Theorem.*** For a continuous function $f(x)$ over the interval $[a,b]$, there exists a $a \le \xi \le b$ such that $$\int_{a}^b f(x)dx = f(\xi)(b-a)$$
This theorem can be applied more generally by any "weighting" function $p(x)$.



