---
tags:
  - "#math"
  - "#real_analysis"
  - "#calculus"
  - "#richard_courant"
date_created: 2026-02-17
parent: "[[Introduction to Calculus and Analysis I]]"
---
The chapter contains a review of the basic concepts for real analysis. The authors go over the following key concepts:
- Rational numbers
- An intuitive appeal to understand the denseness of Rational Numbers on the number line (yet to be defined)
- The existence of incommensurable quantities
- Demonstration of proof by contradiction
- A description of irrational numbers in terms of rational numbers.
- Postulate of Nested Intervals (or [Axiom of continuity](Understanding%20Analysis%20-%201.3%20The%20Axiom%20of%20Completeness.md)).
- Decimal representation of a number as a nested intervals of lengths divisible by 10.
- Properties of inequalities
	- absolute value in inequalities
	- triangle inequality
	- Cauchy-Schwarz Inequality
# 
Rational number written in the form $p/q$ where $p$ and $q\ne 0$ are integers. Further more, the rational operations (addition, multiplication, subtraction and division) are closed within the rational numbers, that is, any operation between rational numbers will produce rational numbers. This is not the case with natural numbers as 1-2 will not be a natural number.

The author demonstrates that rational numbers can be made arbitrarily close to any other number by making the denominator large enough. This ability to make the rational numbers arbitrarily close to ANY other number is expressed by saying: The rational numbers are dense on the number axis. Intuitively, density implies between any two points, there are infinitely many other points.

***Definition of Commensurability:*** Two quantities $a$ and $b$ are commensurable if $\frac{a}{b}$ is a rational number. 

Rational numbers were described as an operation between two integers. How can we describe rational numbers? We describer rational numbers by the Postulate of Nested Intervals

***Axiom: Postulate of Nested Intervals (Axiom of Continuity)***. If $I_1, I_2, I_3, ...$ form a nested sequence of intervals with rational end points, there is a point $x$ that is contained in all $I_n$ 

This axiom is also described by [Understanding Analysis - 1.3 The Axiom of Completeness](Understanding%20Analysis%20-%201.3%20The%20Axiom%20of%20Completeness.md). The axiom guarantees no gaps in the real axis and gives us a way to describe irrational numbers in terms of rational numbers: by a sequence of nested intervals described by rational numbers. An example of this is demonstrated in 1.1c, where the decimal base system of a number $x$ that is contained within a closed interval say $c_0 \le x \le c_0+1$ where $c_0$ is a rational number. And then this interval is subdivided into 10 parts ($c_0 +1/10, c_0+2/10,..., c_0+9/10$). Then the subinterval containing $x$ say $c_1+c_{1}/10 \le x \le c_0+c_1/10+1/10$  where $c_1$ is a natural number 1-9 is further subdivided $n$ ti