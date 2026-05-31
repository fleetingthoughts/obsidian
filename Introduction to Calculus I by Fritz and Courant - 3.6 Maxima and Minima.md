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
1) A continuous function on a finite closed interval always has an extremum by Weierstrass' Theorem. The purpose of this chapter is to determine the extremum.
2) ***A necessary condition for a relative extremum***: If $x_o$ is a relative extrema and is differentiable at the point, then $f'(x_o)=0$
3) ***A sufficient condition for a relative extremum*** If the derivative $f'(x)$ changes sign when it passes through $x=x_o$ then $x_o$ is a relative extrema
4) If $f''(x_o) \ne 0 \land f'(x_{o})=0$ , then it guarantees $x=x_o$ is a relative extremum. Note this test is weaker than 3) as we have no information if $f''(x_o)=0$ 
5) The absolute maximum is either 1) the endpoints of the domain or one of the critical points
6) We now have a theory of maxima and minima in point 1) which gives us the criteria for existence and combining 2) and 4)  gives us a method to compute them by point-wise computations

## A point being a relative extremum guarantees that its derivative at that point is 0
Note that the converse is not true. A counterexample would be a point of inflection. Nevertheless, our algorithm for determining the maxima still computes the points where the derivative is 0. Not because it guarantees that it is a relative extremum, but because it is a candidate for one.

The proof for the sufficiency condition assumes the given:
- Given a function $f$ defined on an interval $[a,b]$. This is so that we are guaranteed an absolute maxima to make this a tenable problem.
- The function $f(x)$ is differentiable everywhere in the interval so it is also continuous.
- The definition of the relative extrema given in the "Definitions" section
The proof is a direct proof by appealing to the definition of a limit and the requirements that all sequences converge to the same limit 
- Construct the derivative difference about the relative extremum $x=x_o$. This is an arbitrary construction that eventually lets us make use of the definition of the derivative
- Take the limit of the difference quotient and show we can form two sequences of numbers depending on whether $h$ is positive or negative:
	- Show that we have one sequence of numbers that is greater than or equal to 0.
	- Show that we have another sequence of numbers is less than or equal to 0
- We have two sequences that must converge to the same number so it must be 0. 
	- Because we assumed the limit (i.e. the derivative exists)
	- For the limit to exist all sequences must converge to the same number and 0 is the only number that satisfies equality between the two sequences

## A point being a relative extremum guarantees that the derivative changes sign at that point. 
The proof of this is an application of the mean value theorem where the difference $f(x+h)-f(x)$ must always have the same positive or negative sign depending on whether $x$ is a minimum or a maximum. Therefore by the mean value theorem: $$f(x+h)-f(x)=f'(\xi+\theta h)h$$
## The 2nd derivative is used to determine whether the point is a maximum or minima.
From the previous two theorems, we've established the following conditions required for a relative extremum:
1)  The derivative at the point $x=x_o$ is $f'(x_o)=0$.
2)  The derivative changes sign at $x=x_o$.
Condition 1) alone is not enough sufficient for $x=x_o$ to be a relative extremum, but condition 2) is. The problem with condition 2) is it describes a local property not a point property so it is harder to compute.

We can actually replace 2) with a different condition that when combined with 1), it guarantees that the point is a local extremum and we can further determine what kind of extrema. Specifically we can compute the value of the 2nd derivative at the point $x=x_o$, we can combine it with the previous two theorems to determine whether the point is a local maximum or minimum. Specifically we will prove that if the $x=x_o$ :
3) If $f''(x_o)>0$ and 1) is satisfied, then it guarantees $x=x_o$ is a local minimum
4) If $f''(x_o)<0$ and 1) is satisfied, then it guarantees $x=x_o$ is a local maximum






# Definitions
- ***Inflection point***
- ***Relative extremum***. The points $x=x_o$ such that all points in some interval $x\in (x-h,x+h)$ where $h>0$ such that $f(x)\le f(x_o)$ in the case of an relative maxima or $f(x_o) \le f(x)$ for a relative minima.
- ***Critical or stationary points***. Points that are roots to the equation $f'(x)=0$
# Theorems
***Theorem.*** $f'(\xi)=0$  whenever $f$ is a relative extremum point in the interior of the domain of $f$ provided $f$ is differentiable at $x=\xi$. 

***Theorem (Candidates for the absolute maxima or minima).*** An absolute maximum or minimum of the function coincides either with a critical point of the function or with an end point of its domain

***Theorem (A relative extrema implies change in sign of the derivative).*** The function $f(x)$ has a relative extremum at an interior point $\xi$  of its domain if, and only if, the derivative $f'(x)$ changes sign as $x$ passes through this point; in particular, the function has a relative minimum if near $\xi$ the derivative is negative to the left of $\xi$ and positive to the right, whereas in the contrary case it has a maximum.

***Theorem.*** At the same time we see that the value $f(\xi)$ is the greatest or least value of the function, in every interval containing the point $\xi$, in which f is differentiable and in which the only change of sign of $f'(x)$ occurs at $\xi$ itself.

***Theorem.*** A point $\xi$ at which $f'(x)$ vanishes is a maximum point of $f$ if $f"(x) < 0$ throughout the interval (or if its curve is concave), and a minimum point off if throughout the interval $f"(x) > 0$ (that is, if the curve is convex). 