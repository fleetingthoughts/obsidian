---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - "#stephen_abbot"
  - "#math"
  - "#real_analysis"
date_created: 2026-02-16
---
Using the results we proved for sequences, we are now in a position to say something about an infinite series $\Sigma_{i=1}^{\infty}a_i$ . There are no new concepts here, as this section is effectly a collection of properties and tests for convergences for a series by applying theorems we already proved about sequences. I shall first present the theorems in the same order as the author before summarizing the "toolbox" we have at the end. At the end of the section, there is a new concept that we do learn about rearrangements

Summary:

Properties of convergent infinite series:
- Convergent infinite series are distributive with a real number constant
- Convergent infinite series follow conventional additive rules

Tests/conditions to determine wither an infinite series converges:
- Cauchy criterion $\iff$ convergence of the infinite series: series converges if and only if the sum of any # of countable terms can be made arbitrarily small by choosing terms far enough along the sequence
- The terms of the infinite series go to $0$
- Comparison test: determine convergence of a series by using a known convergent/divergent series that bounds or eventually bounds our series of interest
- Absolute convergence $\implies$ convergence. Note the reverse is not true
- (Series is non-increasing) $\cap$ (terms tend to 0) $\implies$ series alternatively converges

We first must make sure we make clear the distinction between two different sequences regarding an infinite series:
1) a sequence of its terms: $(a_1,a_2,...)$
2) the sequence of its partial sums $(s_1,s_2,s_3,..) where $s_n = a_1+a_2+...+a_n$

***Unofficial Definition of the convergence of an infinte series:*** We now define the convergence of an infinite series in terms of the sequence: Given an infinite series $\Sigma_{i=1}^{\infty}a_i$, and a sequence of its partial sums $(s_n)$:
$$\lim_{ n \to \infty}s_n  \iff \Sigma_{i=1}^{\infty}a_i=A$$
Now that we <u>defined</u> the convergence of a series in terms of the sequence of its partial sums, we can apply our results from sequences

***Theorem 2.7.1 (Algebraic Limit Theorem for Series).*** Given  $\Sigma_{i=1}^{\infty}a_i=A$ and  $\Sigma_{i=1}^{\infty}b_i=B$, that is both series converge to a definite limit, then we have the following two properties:
1)  $\Sigma_{i=1}^{\infty}ca_i=cA \text{\quad for all \quad}c\in R$   (Distributive property)
2)  $\Sigma_{i=1}^{\infty}(a_i+b_{i})=A+B$
The product of infinite series is left for later. The [[Proof of the Algebraic Limit Theorem for Series]] is already implied by [Theorem 2.3.3](Understanding%20Analysis%20-%202.3%20The%20Algebraic%20and%20Order%20Limit%20Theorems.md)

***Theorem 2.7.2 (Cauchy Criterion for Series).*** The series $\Sigma_{i=1}^{\infty}a_i$ converges if and only if given natural numbers $n>m >N$, for $(m,n,N)\in \mathbb{N}$, a sufficiently large $N$ can be chosen such that for any arbitrary choice of $\epsilon>0$ 
$$|a_m+a_{m+1}+a_{m+2}+....+ a_n| <\epsilon \text{\quad for\quad}\epsilon>0$$[[The proof of the Cauchy Criterion for Series]] follows by showing that the above summation is a identical to the condition for a Cauchy sequence and by [the Cauchy Criterion](Understanding%20Analysis%20-%202.6%20The%20Cauchy%20Criterion.md), this means it must converge

From the Cauchy Criterion for series, it can then be shown for an infinite series to converge, its terms must go to null:
***Theorem 2.7.3 (Behaviour of the terms in a convergent infinite series).*** If a series $\Sigma_{i=1}^{\infty}a_i$ converges, then it is sufficient that $$\lim_{ n \to \infty } a_n = 0$$
Note that the converse is not true (e.g. the harmonic series). 

The proof of this is a specific case where $n=m+1$ (i.e. consecutive terms) of the proof for the Cauchy Criterion of Series, that is, we show the difference between between consecutive terms in a sequence of partial sums ($a_n=|s_{n+1}-s_{n}|$) tends to 0. 

***Theorem 2.7.4. (Comparison Tests for Convergence)***. Given sequences $(a_k)$ and $(b_k)$ where $0\le a_k \le b_k$, then:
1) $\Sigma_{i=1}^{\infty}a_i$ converges if $\Sigma_{i=1}^{\infty}b_i$ converges
2) $\Sigma_{i=1}^{\infty}a_i$ diverges if $\Sigma_{i=1}^{\infty}b_i$ diverges

Note that these statements do not care for the behavior of a finite number of terms and it only cares about the eventual behavior of the sequence for indeed the comparison tests can be used for the weaker condition that $a_k \le b_k$ for $k > M$, that is, the condition is satisfied after the initial $M$ terms.

***Theorem 2.7.6 (Absolute Convergence Test)***. If the series $\Sigma_{i=1}^{\infty}|a_i|$ then it is sufficient that $\Sigma_{i=1}^{\infty}a_i$ converges as well

The [[Proof for Absolute Convergence Test of an Infinite Series]] is proved using the Cauchy Criterion, but I believe it can also be proved with the [Monotone Convergence Theorem](Understanding%20Analysis%20-%202.4%20The%20Monotone%20Convergence%20Theorem%20and%20a%20First%20Look%20at%20Infinite%20Series.md).

Note that the converse for this is not true (e.g. the harmonic series diverges while the alternating harmonic series diverges). This leads us to the next test
***Theorem 2.7.7. (Alternating Series Test).*** If a sequence $(a_n)$ satisfies the following conditions:
1) $a_1 \ge a_2 \ge a_3 \ge ... a_n \ge a_{n+1} \ge...$  (sequence is non-increasing)
2) $\lim_{ n \to \infty } a_{n} =0$
Then the alternating sequence $\Sigma_{i=1}^{\infty}(-1)^{n+1}a_i$.  The [[Proof for the Alternate Series Test]] is done in Exercise 2.7.13

The existence of infinite series that show that the converse of Theorem 2.7.6 isn't true leads us to define different types of convergent series

***Definition 2.7.8 (Absolute and Conditional Convergence).*** If $\Sigma_{i=1}^{\infty}|a_i|$ converges, then we say $\Sigma_{i=1}^{\infty}a_i$ <u>converges absolutely</u> (by theorem 2.7.4). If $\Sigma_{i=1}^{\infty}a_i$ converges but $\Sigma_{i=1}^{\infty}|a_i|$ does not converge, then we say $\Sigma_{i=1}^{\infty}a_i$ <u>converges conditionally</u>

The Alternating series test is the most accessible test for conditional convergence but [[Abel's Test]] from Exercise 2.7.13 will show another.

Question: Is there a way we can show the series converges to a limit if and only if the sequence of its partial sums converges to the same limit? How do we analytically connect the sequence of partial sums to the infinite series.

Answer: We simply defined the convergence of a series in terms of the sequence of its partial sums

# Rearrangements
Now we look at actual new concept and answer one of our questions about infinite series: does the rearrangement of terms in an infinite series change anything about the properties of the original series? First it is helpful to be precise about what we mean by rearrangement:

***Definition 2.7.9. (Rearrangement of the terms of an Infinite Series)*** Given an infinite series $\Sigma_{k=1}^{\infty}a_k$, we say $\Sigma_{k=1}^{\infty}b_k$ is a rearrangement of the original series if there is a one-to-one AND onto function (i.e.[bijective](Surjectivity,%20Injectivity,%20and%20Bijectivity.md)) $f: \mathbb{N} \to \mathbb{N}$  that can map each $b_{f(k)} \to a_k$  for all $k\in \mathbb{N}$ (this also means we can map $a_{f^{-1}(k)} \to b_k$ since the function is bijective)

In other words, a rearrange is strictly a permutation of the terms from the original sequence and does not:
- add terms with a different magnitude
- change the magnitude of the terms

***Theorem 2.7.10. (The rearrangement of An Infinite Series).*** If a series converges absolutely, then any rearrangement of the series converges to the same limit.

The [[Proof for the convergence for the rearrangement of an absolutely convergent series]] uses the triangular inequality and the creativity of introducing adding then subtracting another term.