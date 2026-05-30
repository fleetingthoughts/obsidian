---
tags:
  - math
  - calculus
  - real_analysis
  - richard_courant
  - fleeting
date_created: 2026-04-08
parent: "[[Introduction to Calculus and Analysis I]]"
---
We develop the theory to determine the maxima and minima which are guaranteed by Weierstrass' theorem:
1) A continuous function on a finite closed interval always has an extrema by Weierstrass' Theorem
2) If $x_o$ is a relative extrema, then $f'(x_o)=0$.
3) The absolute maxima is either 1) the endpoints of the domain or one of the critical points
4) We now have a theory of maxima and minima in point 1) which gives us the criteria for existence and 3) gives us a method to compute them. 

# A point being a relative extrema guarantees that its derivative at that point is 0
Note that the converse is not true. A counterexample would be a point of inflection. Nevertheless, our algorithm for determining the maxima still computes the points where the derivative is 0. Not because it guarantees that it is a relative extrema, but because it is a candidate for one.

The proof for the sufficiency condition assumes the given:
- Given a function $f$ defined on an interval $[a,b]$. This is so that we are guaranteed an absolute maxima to make this a tenable problem.
- The function $f(x)$ is differentiable everywhere in the interval so it is also continuous.
- The definition of the relative extrema given in the "Definitions" section
The proof is a direct proof by appealing to the definition of a limit and the requirements that all sequences converge to the same limit 
- Construct the derivative difference about the relative extrema $x=x_o$. This is an arbitrary construction that eventually lets us make use of the definition of the derivative
- Take the limit of the difference quotient and show we can form two sequences of numbers depending on whether $h$ is positive or negative:
	- Show that we have one sequence of numbers that is greater than or equal to 0.
	- Show that we have another sequence of numbers is less than or equal to 0
- We have two sequences that must converge to the same number so it must be 0. 
	- Because we assumed the limit (i.e. the derivative exists)
	- For the limit to exist all sequences must converge to the same number and 0 is the only number that satisfies equality between the two sequences


# Definitions
- ***Inflection point***
- ***Relative extrema***. The points $x=x_o$ such that all points in some interval $x\in (x-h,x+h)$ where $h>0$ such that $f(x)\le f(x_o)$ in the case of an relative maxima or $f(x_o) \le f(x)$ for a relative minima.
- ***Critical or stationary points***. Points that are roots to the equation $f'(x)=0$
# Theorems
***Theorem.*** $f'(\xi)=0$  whenever $f$ is a relative extremum point in the interior of the domain of $f$ provided $f$ is differentiable at $x=\xi$. 

***Theorem.*** An absolute maximum or minimum of the function coincides either with a critical point of the function or with an end point of its domain

***Theorem.*** The function $f(x)$ has a relative extremum at an interior point $\xi$  of its domain if, and only if, the derivative $f'(x)$ changes sign as x passes through this point; in particular, the function has a relative minimum if near $\xi$ the derivative is negative to the left of $\xi$ and positive to the right, whereas in the contrary case it has a maximum.

***Theorem.*** At the same time we see that the value $f(\xi)$ is the greatest or least value of the function, in every interval containing the point $\xi$, in which f is differentiable and in which the only change of sign of $f'(x)$ occurs at $\xi$ itself.

***Theorem.*** A point $\xi$ at which $f'(x)$ vanishes is a maximum point of $f$ if $f"(x) < 0$ throughout the interval (or if its curve is concave), and a minimum point off if throughout the interval $f"(x) > 0$ (that is, if the curve is convex). 