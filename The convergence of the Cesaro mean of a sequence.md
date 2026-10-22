---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch2
  - real_analysis
  - stephen_abbot
  - math
date_created: 2026-07-24
---
Define the Cesaro mean of a sequence $(a_n)$ and what propositions can we make relating the convergence of the sequence of Cesaro means and the convergence of the sequence
#### Notes
1. Write the difference $c_n - L = \frac{1}{n} \sum_{k=1}^n (a_k - L)$.
2. Fix $\epsilon > 0$. Choose $N \in \mathbb{N}$ such that $\vert{}a_k - L\vert{} < \frac{\epsilon}{2}$ for all $k > N$.
3. Split the sum into two parts: $k \le N$ and $k > N$.
4. Bound the second sum strictly by $\frac{n-N}{n} \frac{\epsilon}{2} < \frac{\epsilon}{2}$.
5. Observe the first sum is a fixed finite value divided by $n$; choose $M > N$ such that this term is bounded by $\frac{\epsilon}{2}$ for all $n > M$.
6. Conclude $\vert{}c_n - L\vert{} < \epsilon$ for all $n > M$.
<!--SR:!fsrs,2026-10-30T01:42:41.963Z,8,8.2956,1,2,1,0,0,2026-10-22T01:42:41.963Z-->

**Definition of the Cesàro Mean**
For a given sequence $(a_n)$, the sequence of its Cesàro means, typically denoted as $(c_n)$, is defined as the arithmetic average of the first $n$ terms of the sequence:


$$c_n = \frac{1}{n} \sum_{k=1}^{n} a_k = \frac{a_1 + a_2 + \dots + a_n}{n}$$

**Propositions Relating Convergence**

1. **Forward Implication (Cesàro's Theorem):** If the original sequence $(a_n)$ converges to a finite limit $L$ (i.e., $\lim_{n \to \infty} a_n = L$), then the sequence of its Cesàro means $(c_n)$ also converges to exactly the same limit $L$. This proposition also holds for limits diverging to $+\infty$ or $-\infty$.
2. **The Converse is False:** The convergence of the sequence of Cesàro means $(c_n)$ does *not* imply that the original sequence $(a_n)$ converges. A sequence can oscillate endlessly but still possess an average that settles to a stable limit.


* *Counterexample:* Consider Grandi's sequence $a_n = (-1)^n$, which alternates as $-1, 1, -1, 1, \dots$. The sequence $(a_n)$ strictly diverges, but its sequence of Cesàro means $(c_n)$ converges to $0$.


3. **Conditional Converse (Tauberian Theorems):** You can prove that the original sequence $(a_n)$ converges if its Cesàro mean $(c_n)$ converges *and* you apply an additional constraint restricting the growth rate of the original terms. For example, Hardy's Tauberian theorem states that if $\lim_{n \to \infty} c_n = L$ and the sequence $(n(a_{n} - a_{n-1}))$ is bounded, then $\lim_{n \to \infty} a_n = L$.
<!--SR:!fsrs,2026-10-01T23:24:09.727Z,0,4.24631526,6.40211507,1,2,0,1,2026-10-01T23:14:09.727Z-->

