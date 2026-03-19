---
tags:
  - "#math"
  - calculus
  - richard_courant
date_created: 2026-03-10
parent: "[[Introduction to Calculus and Analysis I]]"
---
We now discuss the Euler's number, powers of Euler's number, and their relationship to the $\ln(x)$ function defined as an indefinite integral. In this chapter we show:
- $\ln(e)=1$ 
- Demonstrate that the natural logarithm is the inverse function of $e^{\alpha}$ for $\alpha \in \mathbb{R}$ using the limit definition.
- Redefining the arbitrary power of positive numbers in terms of exponentials. This later lets us bypass limit definitions of power functions with irrational exponents which apparently rely on special convergence conditions that is outside the scope of this book
- Prove the multiplicative property of exponential functions
- Determine the natural logarithm of any base other than $e$.

We demonstrate that the natural logarithm is an inverse function of the exponential by first proving $\ln(e)=1$ from the limit definition of $e$: $$ln(e^x)= \ln(\lim_{n\to \infty}(1+\frac{x}{n})^n)$$
We can now try to define the exponential function as the inverse of the logarithm function. In doing so we see the strength in defining the logarithm as an indefinite integral to make use of the continuity properties of integrals.  If we define powers of $e$ (i.e. the exponential function) by taking this inverse, then the continuity of $e^x$ arises from general theorems that require no special arguments. Most notably, we can be assured that we can take irrational powers of $e$. Defining powers as the inverse of a continuous function breaks us free from the elementary definitions of powers such as $e^m$ as "multiply $e$ an $m$ number of times". While such an elementary definition can be extended for rational numbers, it falls apart with irrational numbers (how do we multiply $e$ a $\pi$ number of times for instance?). Instead of appealing to special arguments like sequences of irrational powers, we can now appeal to the continuity of the inverse function to guarantee the existence of the limit and compute the limit using the indefinite integral which is easier. In summary:
- Because the natural logarithm is an indefinite integral, it continuous and monotonic. This also means it has an inverse that is continuous and monotonic as well. We do not need to check for continuity for each case (such as for irrational exponents).
- We no longer need elementary definitions of power functions.
- The exponential powers such as $x=e^{\pi}$ do not need to be computed with sequences of irrational numbers but is instead defined by the number $x$ such that $ln(x)=\pi$.

Since the logarithm is an integral of a continuous function, and the limit is known to exist, we can commute the limit symbol: $$\begin{aligned}
\lim_{n \to \infty } \ln\left( \left( 1+\frac{x}{n} \right)^n \right) & = \lim_{ n \to \infty } \int_{1}^{1+x/n}\frac{1}{u}du \\ 
& = \lim_{ n \to \infty }  \frac{1}{\xi}\left( 1+\frac{x}{n} -1\right) \text{\quad for }0 \le \xi \le 1+\frac{x}{n}
\end{aligned}$$
Where the last one step follows from the mean value theorem. Evaluating the limit then yields $x$. To then evaluate the logarithm to any base other than $e$, we note the relationship: $$\begin{aligned}
a^y & = x \\
y\ln a&=\ln x\\
y&= \frac{\ln x}{\ln a}\\
\ln_{a}a^y&=\frac{\ln x}{\ln a}
\end{aligned}$$





