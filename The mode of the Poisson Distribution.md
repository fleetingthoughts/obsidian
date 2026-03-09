---
tags:
  - "#math"
  - "#statistics"
  - "#probability"
date_created: 2026-03-07
---
The mode of a random variable $X$ with a Poisson distribution with parameter $\lambda$ is $x = floor(\lambda)$. This can be derived by noting that the mode at $x$  is such that $P(x+1) \le P(x)$ and $P(x-1) \le P(x)$. For the former, we have the condition: $$\begin{aligned}
\frac{\lambda^{x+1}e^{-\lambda}}{(x+1)!} & \le \frac{\lambda^{x}e^{-\lambda}}{x!} \\
\lambda &\le x+1
\end{aligned}$$
Similarly for the latter: $$\begin{aligned}
\frac{\lambda^{x-1}e^{-\lambda}}{(x-1)!} & \le \frac{\lambda^{x}e^{-\lambda}}{x!} \\
x &\le \lambda
\end{aligned}$$



