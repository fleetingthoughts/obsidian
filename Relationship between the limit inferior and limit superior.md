---
parent: "[[Understanding Analysis - 2.4 The Monotone Convergence Theorem and a First Look at Infinite Series]]"
tags:
  - "#flashcard"
  - math
  - micro/math/abbott/ch2
  - stephen_abbot
  - real_analysis
date_created: 2026-07-24
---
State and prove the universal relationship between the limit inferior and limit superior
#### Notes
**Statement of the Universal Relationship** For any bounded real sequence $(a_n)$, the limit inferior is always less than or equal to the limit superior:

  

$$\liminf_{n \to \infty} a_n \le \limsup_{n \to \infty} a_n$$
**Phase 1: Define the Tail Sequences** Let $S_N = \{a_n : n \ge N\}$ represent the tail set of all terms in the sequence from index $N$ onward. Define the sequence of infimums as $u_N = \inf(S_N)$ and the sequence of supremums as $v_N = \sup(S_N)$. By definition, the limit inferior is $\lim_{N \to \infty} u_N$ and the limit superior is $\lim_{N \to \infty} v_N$.

**Phase 2: Establish the Inequality for a Fixed $N$**
For any chosen starting index $N$, the set $S_N$ contains the exact same elements for both the infimum and supremum calculations.
By the fundamental properties of real numbers, the greatest lower bound (infimum) of any non-empty set can never exceed its least upper bound (supremum). Therefore, for every $N \in \mathbb{N}$:

$$u_N \le v_N$$

**Phase 3: Apply the Order Limit Theorem**
Since the sequence of inequalities $u_N \le v_N$ holds for all $N$, the Order Limit Theorem guarantees that the limit operator preserves this non-strict inequality as $N$ approaches infinity.

Taking the limit of both sides yields: 
$$\lim_{N \to \infty} u_N \le \lim_{N \to \infty} v_N$$

Substituting the limit inferior and superior definitions from Phase 1, we arrive at the final conclusion:
$$\liminf_{n \to \infty} a_n \le \limsup_{n \to \infty} a_n$$
