---
tags:
  - math
  - philosophy
  - richard_courant
date_created: 2026-03-25
parent: "[[Introduction to Calculus and Analysis I]]"
---
With the fundamental theory of calculus discussed in chapter 2, we now apply these concepts to compute the integrals and derivatives for various functions. Derivatives are easier to compute than integrals, but with the Fundamental Theorem of Calculus, we gain information about the integrals if we develop results in differentiation. 

A common mathematical strategy is to use a definition to develop a result for a specific case and then to develop properties of the definition so that we can generalize the specific case to a wider class of objects. In chapter 2, we computed the integral of various functions by determining the limit of their Riemann sum. We discuss 5 topics to determine the derivative for a wider class of functions. Knowing the derivatives then tells us the integral of a certain class of functions:
1) Derivative of a function multiplied by a constant (the proof of this was provided in chapter 2)
2) Derivative of a sum of functions
3) Derivative of the product of functions. The proof involves adding the strategic zero.
	1) Derivative of several products where each function takes its turn being differentiated
	2) Leibniz's Rule of repeated differentiation proved by induction and takes on a form very similar to the binomial theorem: $$\frac{d^n}{dx^n}(fg)=\sum_{i=0}^n(\frac{d^i}{dx^i}f)(\frac{d^{n-i}}{dx^{n-i}}g)$$
4) Derivative of a quotient of functions which is just derived from 3)
5) Apply the properties 1)-4) to the derivative of $x^n$ and $sin(x)$, and $cos(x)$ to apply it to determine the derivative for a wider class of polynomial and trigonometric functions

With these 4 rules we can reprove some of our original results to show that they are consistent. 
- The derivative of $x^n$ can be determined by knowing the derivative of $x$ and noting $x^n=(x)(x)...(x)$ so that we can just apply the product rule 3). The result is identical with our result [from the definition of the derivative](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%202.8%20The%20Derivative.md) so our results are consistent with each other. This derivation does not appeal to [the definition of the power function as an extension of the exponential function](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%202.7%20The%20Integral%20of%20an%20Arbitrary%20Power%20of%20x.md). We only appeal to our basic naive arithmetic definition of "$x$ multiplied by itself $n$ times"
- Similarly, the derivative with a negative integer exponents can be determined using the quotient rule instead.
The properties allow us to compute the derivative of a wider class of polynomials without appealing to the raw definition of the derivative or compute the respective integrals with Riemann integral

The properties can also be applied to determine the derivative and therefore the integral of a wider class of trigonometric functions. Using our results for the derivative of trigonometric functions, we can determine the derivative of other trigonometric functions without using the definition of the derivative:
$$\begin{aligned}
\int \cos x \, dx &= \sin x, & \int \sin x \, dx &= -\cos x, \\
\int \frac{1}{\cos^2 x} \, dx &= \tan x, & \int \frac{1}{\sin^2 x} \, dx &= -\cot x.
\end{aligned}$$

