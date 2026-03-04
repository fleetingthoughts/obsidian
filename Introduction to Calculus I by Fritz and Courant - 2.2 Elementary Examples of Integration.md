---
tags:
  - "#math"
  - "#calculus"
  - "#real_analysis"
  - richard_courant
date_created: 2026-02-22
parent: "[[Introduction to Calculus and Analysis I]]"
---
We shall now use the Riemann integral to directly derive the integral for basic functions. The derivations will be supported by the theorem of the existence of the Riemann integral, which as a reminder, states that if the function is continuous, the integral exists for any choice of integrating interval subdivision or choice of intermediate points.
$$F_n = \lim_{n\to \infty}\sum_{i=1}^nf(\xi_{i})(x_{i}-x_{i-1})=\lim_{n\to \infty}\sum_{i=1}^nf(\xi_{i})h$$


For each function, the choice of intermediate point, interval subdivision, the final limit to be computed, and the mathematical tools employed will be outlined. The interval of integration is $[a,b]$ and we assume the function is continuous over it.

1) Integration of a Linear function:
	- Equal subinterval division: $h = (b-a)/n$ 
	- Choice of intermediate point is the right hand point of each interval: $\xi_i = nh$
	- Final limit to evaluate is: $$F_n = \lim_{n\to \infty}\sum_{i=1}^n(a+nh)^2h$$
	- Toolbox: arithmetic sum of natural numbers
2) Integration of $x^2$
	- Equal subinterval division: $h = (b-a)/n$ 
	- Choice of intermediate point is the right hand point of each interval: $\xi_i = a+ih$
	- Toolbox: [Sum of Squares](Sum%20of%20Squares.md)
	- Final limit to evaluate is: $$F_n = \lim_{n\to \infty}\sum_{i=1}^n(a+nh)h$$
3) Integration of $x^{\alpha}$ for $\alpha \ne 1$.
The same argument for 1) and 2) can be applied for any integer powers that aren't -1 and then applying the following relation that will arise: $$\lim_{n \to \infty}(1^{\alpha}+2^{\alpha}+...+n^{\alpha})\frac{1}{n^{\alpha+1}} = \frac{1}{\alpha+1}$$An alternative to using this limit is to instead set up the limit with different intermediate points and subintervals:
- Subinterval by geometric progression: $h = aq^i-aq^{i-1}=aq^i(q-1)/q$  where $q =\sqrt[n]{b/a}$ 
- Intermediate point will be the right-hand points: $\xi_i = aq^i$ 

4) Integration of $x^{\alpha}$ for rational $\alpha$ other than -1
To perform this integration, we use the same derivation as for 3)but let $\alpha = r/s$ for integer $r$ and $s$ so that we can express it in terms of integer powers
5) Integration of $\sin{x}$ and $\cos{x}$
	- Equal subinterval division: $h = (b-a)/n$
	- Intermediate point is the right hand point of each interval: $\xi_i = a+ih$ 
	- Apply sine trigonometric identity to express the resulting sum as a telescoping sum.




