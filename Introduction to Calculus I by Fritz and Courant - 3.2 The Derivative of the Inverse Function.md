---
tags:
  - math
  - calculus
  - real_analysis
date_created: 2026-03-28
parent: "[[Introduction to Calculus and Analysis I]]"
---
This chapter continues our application of our results from Chapter 2 to determine the derivatives of elementary common functions. The main tool developed is the derivative of the inverse of a function who's derivative is already known. The chapter is outlined as follows
- The relationship between the derivative of a function to the derivative of the inverse
- How to determine the derivative of the inverse of a function
- The edge cases called critical points where the results of this chapter when the inverse of the function is not guaranteed and our results in this chapter may not apply. The critical points when the derivative is 0.
- Application of the theorem to determine the derivative of inverse trigonometric functions from the derivative of trigonometric functions
- Derivation of the derivative of the exponential function from the derivative of the logarithm

Critical points are cases when $f'(x)=0$. If the derivative is consistently 0 in an interval, then $f(x)$ is a constant there, but if a derivative of 0 only occurs at isolated points, then there are 2 cases:
- The monotonicity changes and we no longer have an invertible function in the interval
- The monotonicity does not change and we simply have an inflection point.

A significant application of these results is the determination of the the inverse of trigonometric functions. Note that to guarantee the inverse exists, we must limit the domain accordingly.
![](Pasted%20image%2020260328172508.png)

As we know the derivative of the logarithm by its definition as an indefinite integral and the application of the fundamental theorem of calculus, we can then determine the derivative of the exponential function. We can continue to determine the derivative of an exponential with respect to any base. We first recall the inverse function: $$x=\log_{a}y=\frac{\ln y}{\ln a}$$
Then the derivative of $a^x$ is the inverse of the derivative of $x$ with respect to $y$: $$\frac{da^x}{dx}=\frac{1}{\frac{d(\log_{a}y)}{dy}}=y(\ln a)=a^x(\ln a)$$
# Definitions
- ***Critical Points*** (p. 208). Points where the derivative is 0 and not for an interval.
# Theorems
- ***Derivative of the inverse of a function (p.207)*** If a function is differentiable in an interval $a<x<b$ and either $f'(x)> 0$ or $f'(x)<0$ throughout the interval, then the inverse function also possesses a derivative at every interior point of its interval definition and is the reciprocal of the $f'(x)$


