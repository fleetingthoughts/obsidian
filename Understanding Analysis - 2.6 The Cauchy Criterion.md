---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - "#math"
  - "#understanding_analysis"
  - "#stephen_abbot"
  - "#real_analysis"
date_created: 2026-02-16
---
We look at another condition for convergence called the Cauchy criterion. The significance of this criterion, like [The Monotone Convergence Theorem](Understanding%20Analysis%20-%202.4%20The%20Monotone%20Convergence%20Theorem%20and%20a%20First%20Look%20at%20Infinite%20Series.md), is that we can show that a sequence converges without knowing what the limit is. A sequence that has the Cauchy criterion is a Cauchy sequence:
***Definition 2.6.1. (Cauchy Sequence).*** A sequence $(a_n)$ is a Cauchy sequence if for any $\epsilon >0$, we can choose a natural number $N$ such that for any $m,n>N$, we have:
$$|a_m-a_n| <\epsilon$$
Restated in words, this means we can make the difference in the magnitude between any two terms (not necessarily consecutive) as small as we want by going far enough along the sequence (i.e. looking at the difference in magnitude between the terms past the $N$th term in the sequence).

The usefulness of the Cauchy sequence is that it gives us a condition for convergence

***Theorem 2.6.2 (Convergence as a sufficiency condition for Cauchy sequences).*** Every convergent sequence is a Cauchy Sequence

This criterion is more powerful than the monotone convergent sequence as convergent sequences are a subset of Cauchy Sequences (i.e. a sequence that satisfies convergences is sufficient for it to be a Cauchy sequence).

$$\text{Bounded Monotone sequence}\subset\text{convergent}\subset\text{Cauchy Sequence}$$

To prove that convergence is implies that the sequence satisfies the Cauchy criterion is in Exercise 2.6.1

Its outside of the scope of this book, but Cauchy sequences technically don't converge unless they are in "complete spaces". For example a Cauchy sequence in rational numbers may not converge, but in complete spaces like the real numbers it is a sufficient and necessary condition for convergence. Since we're in the real numbers, the Cauchy Criterion is a sufficient and necessary condition for convergence so we can prove that a Cauchy sequence is sufficient for convergence

***Theorem 2.6.4 (Cauchy Convergence Criterion).*** A sequence converges if and only if it is a Cauchy sequence

The difficulty in proving the converse is that to prove the Cauchy sequence converges, we must have a proposed limit from the sequence. We have been in this situation before when proving the Monotone Convergence Theorem and the Bolzano-Weierstrass Theorem. We made use of another theorem/property as a proposed limit and tried to show we can always generally satisfy the conditions for that property/theorem:
- Bolzano-Weierstrass theorem: Use the nested interval property to imply the limit must exist and find a strategy to generate those nested intervals exist.
and so to [prove that a sequence satisfying the Cauchy Criterion is sufficient for Convergence](Proof%20that%20a%20sequence%20satisfying%20the%20Cauchy%20Criterion%20is%20sufficient%20for%20Convergence.md), we apply a similar strategy by showing that the Cauchy criterion satisfies some condition for our proposed limit.




