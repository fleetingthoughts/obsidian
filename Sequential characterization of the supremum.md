---
parent: "[[Understanding Analysis - 1.4 Consequences of Completeness]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch1
  - math
  - real_analysis
  - stephen_abbot
date_created: 2026-07-24
---
State the sequential characterization of the supremum. Given a non-empty set $A$ that is bounded above, what sequence is guaranteed to exist?
#### Notes
Let $A \subseteq \mathbb{R}$ be a non-empty set that is bounded above, and let $s = \sup(A)$. The sequential characterization of the supremum states that there exists a sequence $(a_n)$ where $a_n \in A$ for all $n \in \mathbb{N}$, such that: $$ \lim_{n \to \infty} a_n = s $$ *** ### Proof 1. **Leverage the analytical definition of the supremum:** Because $s = \sup(A)$, we know that for any $\epsilon > 0$, the value $s - \epsilon$ is strictly less than $s$ and therefore cannot be an upper bound for $A$. 2. **Construct the sequence:** For each $n \in \mathbb{N}$, let $\epsilon = \frac{1}{n}$. Because $s - \frac{1}{n}$ is not an upper bound, there must exist some element in $A$, which we will call $a_n$, such that: $$ s - \frac{1}{n} < a_n \leq s $$ 3. **Apply the Squeeze Theorem:** We have constructed a sequence $(a_n)$ entirely contained within $A$. Since $\lim_{n \to \infty} \left(s - \frac{1}{n}\right) = s$ and $\lim_{n \to \infty} s = s$, it follows by the Squeeze Theorem that: $$ \lim_{n \to \infty} a_n = s $$ This completes the proof.
