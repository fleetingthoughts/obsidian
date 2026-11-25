---
parent: "[[Understanding Analysis - 7.3 Uniform Convergence and the Riemann Integral]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch7
date_created: 2022-08-25
---
State the theorem regarding the integrability and integral of a function $g : [a, b] \to \mathbf{R}$ that agrees with a Riemann-integrable function $f : [a, b] \to \mathbf{R}$ at all but finitely many points.
#### Notes
Let $f, g : [a, b] \to \mathbb{R}$ be functions on a closed, bounded interval $[a, b]$. If $f$ is Riemann integrable on $[a, b]$ and the set$$\{x \in [a, b] : g(x) \neq f(x)\}$$is finite, then $g$ is Riemann integrable on $[a, b]$, and$$\int_a^b g(x)\,dx = \int_a^b f(x)\,dx.$$Because $f$ is necessarily bounded on $[a, b]$ and $g$ takes real values that differ from $f$ at only finitely many points, boundedness of $g$ follows automatically and does not need to be added as a separate hypothesis.
<!--SR:!fsrs,2026-12-03T21:16:16.986Z,8,8.2956,1,2,1,0,0,2026-11-25T21:16:16.986Z-->

$$\int_a^b g = \int_a^b f$$
