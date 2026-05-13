---
tags:
  - math
  - richard_courant
  - calculus
date_created: 2026-05-12
parent: "[[Introduction to Calculus and Analysis I]]"
---
While differentiation is computationally easier compared to integration, it is offset by the strict requirements for a function to be differentiable. Some integrals are proven to not have a closed analytic form, but the loose conditions required for the existence of the integral allow us to define function using the upper limit of the integral.
1) Integrals are hard to compute but easy to prove existence. We employ the strategy of defining functions using integrals.
2) Examples where 1) was employed for other functions like the logarithm
3) A new example in elliptic integrals

Derivatives and integrals are two sides of the same coin and we generally have a choice of reducing the problem to either a problem of differentiation or of integration. Reducing a problem to differentiation has mainly computational advantages:
- It does not take us out of known closed and analytic functions if the function is already so.
- They are easy to compute
But derivatives have a disadvantage in the stringent conditions required for differentiation to be possible. Continuity is not sufficient for differentiability but it is a necessary condition.

On the other hand integrals are hard to compute and it has been proven that some integrals have no closed analytic form. But it is easy to prove the existence of the integral. The integrand only needs to be continuous. Later in the next chapters, we show the conditions can be looser. The integral can exist with certain discontinuities in the integrand so even strict continuity is not required. If there is no closed analytic form of the integral but we know it exists, we can employ a different strategy: define the function as an integral with a variable upper limit. 

We have used the strategy of defining functions in terms of integrals with the natural logarithm function, but they also could've been used to define the inverse trigonometric functions. 

Another class of functions we define with integrals are the elliptic integrals $u(s)$. These are integrals in which the integrand depends rationally on the square root of a 3rd or 4th degree polynomial: $$u(s)=\int_0^s\frac{1}{\sqrt{(1-x^2)(1-k^2x^2)}}dx$$
The inverse of $u(s)$, if it exists, is called an elliptic function. Several integrals are secretly elliptic integrals that reveal themselves after substitution.

