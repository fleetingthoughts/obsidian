---
parent: "[[Understanding Analysis - 2.3 The Algebraic and Order Limit Theorems]]"
tags:
  - "#flashcard"
  - math
  - stephen_abbot
  - real_analysis
  - micro/math/abbott/ch2
date_created: 2026-07-24
---
State the relationship between a convergence sequence and its boundedness and prove it.
#### Notes
1. Let $(a_n)$ converge to $L$ and set $\epsilon = 1$.
2. Invoke convergence to find $N \in \mathbb{N}$ such that $\vert{}a_n - L\vert{} < 1$ for all $n \ge N$.
3. Apply the reverse triangle inequality to establish $\vert{}a_n\vert{} < \vert{}L\vert{} + 1$ for $n \ge N$.
4. Define $M = \max\{\vert{}a_1\vert{}, \vert{}a_2\vert{}, \dots, \vert{}a_{N-1}\vert{}, \vert{}L\vert{} + 1\}$.
5. Conclude $\vert{}a_n\vert{} \le M$ for all $n \in \mathbb{N}$, satisfying the definition of a bounded sequence.
<!--SR:!fsrs,2026-10-30T01:40:56.994Z,8,8.2956,1,2,1,0,0,2026-10-22T01:40:56.994Z-->

* **Relationship:** Every convergent sequence is bounded. *(Note: The converse is false; a bounded sequence is not necessarily convergent, such as $a_n = (-1)^n$)*.



---

### Proof

1. Let $(a_n)$ be a convergent sequence with $\lim_{n \to \infty} a_n = L$ for some real number $L$.


2. By the definition of convergence with $\epsilon = 1$, there exists an integer $N$ such that for all $n \ge N$, $\vert{}a_n - L\vert{} < 1$.


3. Using the triangle inequality, we can bound the terms where $n \ge N$:



$$\vert{}a_n\vert{} = \vert{}(a_n - L) + L\vert{} \le \vert{}a_n - L\vert{} + \vert{}L\vert{} < 1 + \vert{}L\vert{}$$



4. For the finite set of terms preceding index $N$ ($a_1, a_2, \dots, a_{N-1}$), let us define a global bound $M$ for the entire sequence:



$$M = \max\left(\vert{}a_1\vert{}, \vert{}a_2\vert{}, \dots, \vert{}a_{N-1}\vert{}, \vert{}L\vert{} + 1\right)$$



5. Consequently, $\vert{}a_n\vert{} \le M$ for all $n \in \mathbb{N}$, which proves that the sequence is bounded. $\blacksquare$
<!--SR:!fsrs,2026-10-28T23:59:56.009Z,8,8.2956,1,2,1,0,0,2026-10-20T23:59:56.009Z-->

