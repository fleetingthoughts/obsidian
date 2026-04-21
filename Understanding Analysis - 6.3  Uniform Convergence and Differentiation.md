---
tags:
  - real_analysis
  - stephen_abbot
  - math
date_created: 2026-04-17
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
The previous chapter looked at what properties we need to say something about the continuity of a sequence of functions. We continue analyzing the properties of the limiting function and determine the properties that allow us to say something about the derivative of the limiting function.

A weaker theorem formalizes the condition to know whether a sequence of functions that uniformly converges, is differentiable and what form it will take. We require the two following conditions:
1) That a sequence of functions converges uniformly to a limiting function $f$.
2) Each sequential function is differentiable and the sequence of derivatives also converges uniformly to another function $g$.
With the above, we can then say something about the differentiability of the limiting function and know what it must be identical to. It is sufficient to say the following:
- The sequence of functions converges uniformly to a limiting function, $f$, that is differentiable
- The derivative $f'$ of the limiting function is identical to the function $g$ that the sequential derivatives converged uniformly to.

Although this is a weaker form of the final theorem, because we can make do with a weaker form of 1). The uniform convergence of the sequence of derivatives, 2), says something about the uniform convergence of the original function if we have one other assumption. We can guarantee 1) if we have:
3) Each sequential function is differentiable and the sequence of derivatives also converges uniformly to another function $g$ on an interval $[a,b]$
4) The sequence of function point-wise converges at a single point $x$ within $[a,b]$.
The property 3) is the same as 2), but if we combine it with a weaker assumption in point-wise convergence, then we can guarantee uniform convergence in property 1).


# Theorems
***Theorem 6.3.1 (Uniform convergence of a sequence of functions and its derivatives is sufficient  differentiability of the limiting function and what form it will take).*** Let $f_n$ be a sequence of differentiable functions and let the derivatives $f'_n$ converge uniformly to $g$. If $f_n$ converges uniformly to $f$, then the limiting function $f$ is differentiable such that $f'=g$.

***Theorem 6.3.2 (The uniform convergence of a sequence of derivatives of a function and convergence at a point guarantees uniform convergence).*** Given a sequence of functions $f_n$ defined on an interval $[a,b]$ whose derivatives $f'_n$ converges uniformly on the $[a,b]$ interval, if the sequence of functions converges at a point $x \in [a,b]$, then $f_n$ converges uniformly to a limiting function on the entire $[a,b]$ interval

***Theorem 6.3.3 (Combination of 6.3.1 and 6.3.2).***
