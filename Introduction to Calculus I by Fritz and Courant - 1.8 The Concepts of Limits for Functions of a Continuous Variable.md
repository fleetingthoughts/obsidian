---
tags:
  - "#math"
  - richard_courant
  - "#calculus"
  - real_analysis
date_created: 2026-02-22
parent: "[[Introduction to Calculus and Analysis I]]"
---
We have previously discussed limits in terms of sequences and the continuity of functions, but we now connect these two to discuss the limits of functions

The limit of a function is defined such that the only difference between the limit of a function at $f(x_o)$ and whether it is continuous at $x_o$ is whether the function is actually defined at $x_o$ and is equal to the limit. In other words if the limit exists we just need to check if $\\lim_{x\to x_o}f(x_o)=f(x_o)$ to determine if it is continuous.

The definition of the limit can also be described in terms of the limits of sequences. Given a function $f$ continuous at $x_o$ and a sequence $(x_n)$ that converges to $x_o$, the following statement can be proven (p.83): $$\lim_{ x \to x_{o} } f(x)=\lim_{ n \to \infty } f(x_{n})$$
More generally, for a function continuous in an interval, the limit can be commuted across the function operator (and in turn applies to compound functions as well):
$$\lim_{  n \to \infty  } f(x_{n})=f( \lim_{ n \to \infty } x_{n})$$
Showing that the limit operation can commute across the function operator of continuous functions allows us to perform algebraic addition and scalar multiplication of functions and commute the limit as freely as we want as long as the functions are continuous as we can express these additions, product, and quotient of functions as new functions and show they can converge by writing the limits of the functions as limits of sequences. 


A couple important limits involving transcendental functions: 
- The limit of the  <u>sinc function</u> and [the proof in the book is geometric](Proof%20of%20the%20limit%20as%20x%20approaches%200%20of%20the%20sinc%20function.md):
$$\lim_\limits{  x \to 0 } \frac{sin(x)}{x} = 1$$
-  The following also follows from the aforementioned limit of the sinc function: 
$$\begin{align}
\lim_\limits{x\to 0}\frac{1-cosx}{x}  & = \frac{(1-\cos{x})(1+\cos{x})}{x(1+\cos{x})}  \\
& = \frac{1-\cos^2{x}}{x(1+\cos{x})} \\
& = \frac{\sin}{x}\frac{1}{1+\cos{x}}\sin{x} = 0
\end{align}$$
In the last line, the first 2 terms tend to 1 while the last term tends to 0

With these results, we can show that any [elementary function](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%201.3%20Elementary%20Functions.md) is continuous by using our previously proven limits to make compound functions of any elementary function we want. For example, knowing $x$ is continuous, we can show $x^2$ is continuous by the product of $x \times  x$.

As a final side note, as continuous functions are completely described by sequences converging to any number in the interval the function is continuous on, we can define functions containing irrational numbers in the domain by using a sequence of rational numbers that converges to the irrational number as $\mathbb{Q}$ is dense in $\mathbb{R}$. An actual application of this will be shown in chapter two, but this can also be shown by the Archimedean property in [Understanding Analysis - 1.4 Consequences of Completeness](Understanding%20Analysis%20-%201.4%20Consequences%20of%20Completeness.md)



We combine the results that we've established between sequences and functions:
- relationship between limit and continuity
- limit of a function described completely in terms of sequence. Limit can be commuted between function operator
- Algebraic limit theorems of functions
- sinx/x by geometry
- 1-cosx/x
- limit of compound function
- functions with irrational numbers defined in terms of sequences of rational numbers that are dense on the real. Example with power to a rational
