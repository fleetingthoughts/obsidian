---
tags:
  - "#math"
  - "#probability"
  - "#statistics"
date_created: 2026-03-07
---
Chernoff's bound is an application of a specific case of Markov's inequality, which provides an exponentially decaying upper bound on the tails of a probability distribution. Specifically the inequality is derived from Markov's inequality: $$P(X\ge a) \le \frac{E(X)}{a}$$
Substituting $X$ for $e^{tX}$ and a for $e^{ta}$, we obtain the Chernoff bound:
$$\begin{align}
P(X\ge a) &\le M(t)e^{-ta}\text{\quad for }0<t<h \\
P(X\le a) &\le M(t)e^{-ta}\text{\quad for }0>t>-h
\end{align}$$


