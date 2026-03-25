---
tags:
  - math
  - philosophy
  - richard_courant
date_created: 2026-03-25
parent: "[[Introduction to Calculus and Analysis I]]"
---
The chapter has no conceptual topics but is an application of previous results to establish fundamental rules for differentiation. The following rules all assume that the functions are differentiable (which is a stronger requirement than continuity):
1) Derivative of a function multiplied by a constant (the proof of this was provided in chapter 2)
2) Derivative of a sum of functions
3) Derivative of the product of functions. The proof involves adding the strategic zero.
	1) Derivative of several products where each function takes turn being a derivative
	2) Leibnitz's Rule of repeated differentiation proved by induction and takes on a form very similar to the binomial theorem: $$\frac{d^n}{dx^n}(fg)=\sum_{i=0}^n(\frac{d^i}{dx^i}f)(\frac{d^{n-i}}{dx^{n-i}}g)$$
4) Derivative of a quotient of functions which is just derived from 3)

With these 4 rules we can reprove some of our original results to show that they are consistent.
- The derivative of $x^n$ can be determined by knowing the derivative $x$ and noting $x^n=(x)(x)...(x)$ so that we can just apply the product rule 3). The result is identical with our result [derived straight from the definition Riemann integral](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%202.2%20Elementary%20Examples%20of%20Integration.md) so we are ensured that our results are consistent with each other. This derivation does not appeal to [the definition of the power function as an extension of the exponential function](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%202.7%20The%20Integral%20of%20an%20Arbitrary%20Power%20of%20x.md). We only appeal to our basic naive arithmetic definition of "$x$ multiplied by itself $n$ times"
- Similarly, the derivative with a rational exponent can similarly be determined using the quotient rule instead.

We can derive new functions as well using our new rules which would otherwise be tedious if we were to appeal to the raw definition of the Riemann integral. Using our results for the derivative of trigonometric functions, we can determine the derivative of other trigonometric functions without having to construct a Riemann sum:

![](Pasted%20image%2020260325182835.png)