---
tags:
  - "#math"
  - "#calculus"
  - "#real_analysis"
  - "#richard_courant"
date_created: 2026-02-22
parent: "[[Introduction to Calculus and Analysis I]]"
---
The definition of the integral employs a common strategy in mathematics where mathematical interest and intuition requires us to furnish a specific property which we then define and work backwards to derive the intuition that motivated us in the first place Historically, the intuitive concept of area drove the development of the integral, but Courant reverses the process and defines a concept known as the integral in a way that allows us to derive the intuitive properties of the area. Three central themes motivate this approach
1) The intuitive notions (i.e. "axioms") for area
2) Intuitive notion of the method of exhaustion to provide the moral answer that area can be described as a limiting process of summation
3) 1) and 2) motivate us to define the integral in a way that derives all the intuitive notions of area so we can define the integral as the area. One such definition is the Riemann integral.

We start with some familiar properties of area that we take for granted and are arguably axioms in Courant's book:
- Area is a nonnegative number
- Area is the same for all congruent figures so it is invariant to translation
- The area is always defined for the rectangle as the product of its two sides
- If one geometric is a subset of another, then it has a smaller area. Area exhibits monotonicity.
- An area can be exhaustively decomposed into small rectangles ad infinitum.

The first part of the chapter is a geometric approach to calculate the area that results in an infinite series. This limit is defined as the Riemann integral and the existence of the limit as a finite value is stated as a theorem whose proof is left to the Supplement.
***Definition of the Riemann integral.*** Given a function $f(x)$ defined on a closed interval $[a,b]$, with a partition $P=\{x_1,...,x_n\}$ and a choice of intermediate points $\eta_i$ within each subinterval. The integral is defined as the limit of the Riemann sum $S$: $$\lim_{ n \to \infty } S(f,\eta_{i},P_{n})=\lim_{ n \to \infty }\sum_{i=1}^{n}f(\eta_{i})\triangle x_{i}$$
Where $\triangle x_i$ is the length of the $i$th subintervals of $[a,b]$ and $\eta_i$ is a point in each corresponding subinterval. The Riemann sum is a function of three things:
1) The function $f(x)$ to be integrated
2) The choice of partition $P_n$
3) The choice of intermediate points $\eta_i$ within each subinterval of the partition.

***Theorem on the existence of the integral as a limit (p. 125).*** For any continuous function $f(x)$, in a closed interval $[a,b]$, the integral over this interval exists as a limit independently of the choice of subdivision or choice of intermediate points in the subinterval as long as the largest subinterval length tends to 0.

By this theorem, the continuity over the interval of integration is the only sufficiency requirement for the limit to exist.

Some notes on the Leibnitz notation and how to interpret it:
- Do not interpret $dx$ as an "infinitesimal" as 18th century mathematicians have done. As of this moment, $dx$ has not been defined at all.
- The $dx$ denotes the variable of integration in the same way the index of summation just indicated the variable that was being iterated over. It is purely notational and is not a variable in itself. 
- The integral is a function of a variable over a defined interval so it only the defined interval that affects the value. The variable can be interchanged with anything in the same way our summation can use $i, j, k...$ for the index of summation.

It should be noted that our geometric appeal of the Riemann Integral does allow us to define it over functions with jump or point discontinuities by simply modifying the intervals we integrate over. The way the Riemann integral can be modified to account for certain kinds of discontinuities is its distinguishing feature from other ways to define the integral that are out of the scope of this book.