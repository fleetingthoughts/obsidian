---
tags:
  - calculus
  - real_analysis
  - richard_courant
date_created: 2026-04-05
parent: "[[Introduction to Calculus and Analysis I]]"
---
We define and introduce the hyperbolic functions and derive the properties that are similar to the trigonometric properties:
1) Definition of the hyperbolic functions
2) Fundamental Theorem and addition theorems of hyperbolic functions
3) Derivatives of hyperbolic functions
4) Derivation of the inverse of the hyperbolic functions and computation of their derivatives.

# Definition of the hyperbolic functions
$$\begin{align*} && \sinh x &= \frac{e^x - e^{-x}}{2}, && \cosh x = \frac{e^x + e^{-x}}{2}, \\[1ex] && \tanh x &= \frac{e^x - e^{-x}}{e^x + e^{-x}}, && \coth x = \frac{e^x + e^{-x}}{e^x - e^{-x}}, \end{align*}$$ 
# Fundamental properties of the hyperbolic functions
The chapter is an amalgamation short identities and theorems that bear a striking resemblance to trigonometric identities:
### The fundamental relation
$$cosh^2(x)-sinh^2(x) =1$$
We also have the following:
1) $\cosh(x)+\sinh(x) =e^x$
2) $\cosh(x)-\sinh(x)=e^{-x}$ 
3) $\sinh(x)$ is an odd function
4) $\cosh(x)$ is an even function
5) The derivative of $\cosh(x)$ does not produce a negative sign unlike its trigonometric counterpart.
6) $\sinh(x)$ and $\cosh(x)$ are solutions to the differential equation $y''=y$.

### Addition Theorems
The addition formulas for $\sinh(x)$ are analogous to the trigonometric $\sin(x)$.
$$\sinh(x+y)= \sinh(x)\cosh(y)+\sinh(y)\cosh(x)$$
And because $\sinh$ is an odd function, we can make the substitution for the subtraction formula: $$\sinh(x-y)= \sinh(x)\cosh(y)-\sinh(y)\cosh(x)$$
The difference with trigonometric addition formulae is between $\cosh(x)$ and $\cos(x)$ as what adds and what subtracts is flipped:
$$\cosh(x+y)=\cosh(x)\cosh(y)+\sinh(x)\sin(y)$$
$$\cosh(x-y)=\cosh(x)\cosh(y)-\sinh(x)\sinh(y)$$
The hyperbolic is easier to remember than the trigonometric ones

### Inverse of hyperbolic functions
We can determine an analytic equation to solve for $x=\sinh(y)$ by making the substitution $u=e^x$ which results in us solving for the quadratic equation (note we must have $u>0$ as it represents an exponential): $$x=\sinh(y)\implies x=\frac{1}{2}(u-u^{-1}) \quad\quad x=\cosh(y)\implies x==\frac{1}{2}(u+u^{-1}) $$
The solutions for the quadratic equation give us the formula for the inverse hyperbolic functions $arcsinh(x)=y=\ln(u)$:
$$arcsinh(x)=\ln(x+\sqrt{x^2 +1})\quad\quad\quad arccosh(x)=\ln(x-\sqrt{x^2-1 })$$
Because $\sinh(x)$ is a monotonically increasing function, its inverse exists for the entire domain, but $\cosh(x)\ge 1$ and is not monotonic so we have to pick which branch to choose, the one we have above is the principal branch Courant chose.  