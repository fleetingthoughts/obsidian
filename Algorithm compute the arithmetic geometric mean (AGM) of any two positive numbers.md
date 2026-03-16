---
tags:
  - math_tricks
  - math_toolbox
date_created: 2026-03-15
---

This note defines the arithmetic geometric mean (AGM) and how to produce it. The AGM is a type of mean of any two real positive numbers that is defined by the algorithm that produces it which goes as follows:

***Given any two positive numbers $x_{1},y_{1}\in \mathbb{R}$, the arithmetic geometric mean of $x_{1}$ and $y_{1}$ is defined the converging of the two recursive sequences:***$$x_{n+1}=\sqrt{x_{n}y_{n}}\text{\quad\quad;\quad\quad}y_{n+1}=\frac{x_{n}+y_{n}}{2}$$
The $x_n$ terms develop a geometric mean that can be shown to be monotonically increasing and the $y_n$ terms develop a sequence of arithmetic means that are shown to be decreasing. Using the [AM-GM inequality](The%20inequality%20of%20the%20arithmetic%20mean%20and%20geometric%20mean%20(AM-GM%20inequality).md), it is shown that $x_n \le y_n$ so by the monotonic convergence theorem, both these sequences must converge. The limit they converge can be shown to be the same as well. The resulting AGM of $x_1,y_1$ is therefore a number between the geometric mean $\sqrt{x_1y_1}$  and the arithmetic mean $\frac{x+y}{2}$.

The method was developed by Gauss and makes use of two convergent recursion sequences. Given 