---
tags:
  - "#math"
  - "#calculus"
  - "#real_analysis"
  - "#richard_courant"
date_created: 2026-02-22
parent: "[[Introduction to Calculus and Analysis I]]"
---
The first part of the chapter is a geometric appeal to procedure to calculate the area that results in an infinite sequence. This limit is defined as the Riemann integral and the existence of the limit as a finite value is stated as a theorem whose proof is left to the Supplement.
***Definition of the Riemann Integral.*** Given a function $f(x)$ defined on a closed interval $[a,b]$, The integral is defined as: $$\lim_{ n \to \infty }\sum_{i=1}^{\infty}f(\eta_{i})\triangle x_{i}$$
Where $\triangle x_i$ are the $n$ subintervals of $[a,b]$ and $\eta_i$ is a point in each corresponding sub interval.

***Theorem on the existence of the integral as a limit (p. 125).*** For any continuous function $f(x)$, in a closed interval $[a,b]$, the integral over this interval exists as a limit independently of the choice of subdivision or choice of intermediate points in the subinterval as long as the largest subinterval length tends to 0.

Note that by this theorem, the continuity over the interval of integration is the only sufficiency requirement for the limit to exist.

Some notes on the Leibnitz notation and how to interpret it:
- Do not interpret $dx$ as an "infinitesimal" as 18th century mathematicians have done. As of this moment, $dx$ has not been defined at all.
- The $dx$ denotes the variable of integration in the same way the index of summation just indicated the variable that was being iterated over. It is purely notational and is not a variable in itself. 
- The integral is a function of a variable over a defined interval so it only the defined interval that affects the value. The variable can be interchanged with anything in the same way our summation can use $i, j, k...$ for the index of summation.

It should be noted that our geometric appeal of the Riemann Integral does allow us to define it over functions with jump or point discontinuities by simply modifying the intervals we integrate over. The way the Riemann integral can be modified to account for certain kinds of discontinuities is its distinguishing feature from other ways to define the integral that are out of the scope of this book