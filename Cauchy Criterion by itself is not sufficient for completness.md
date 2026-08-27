---
parent: "[[Understanding Analysis - 2.6 The Cauchy Criterion]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch2
date_created: 2026-07-24
---
Use the Cauchy Criterion to prove the Bolzano-Weierstrass theorem and note the exact step where the Archimedean Property needs to be assumed
#### Notes
### **Proof**
**Step 1: Constructing Nested Intervals (Bisection)**

Let $(x_n)$ be a bounded sequence of real numbers. By definition, there exists a real number $M > 0$ such that all terms of the sequence lie within the closed interval $I_0 = [-M, M]$.

We divide $I_0$ into two equal halves: $[-M, 0]$ and $[0, M]$. Because the sequence $(x_n)$ contains infinitely many terms, at least one of these two subintervals must contain $x_n$ for infinitely many indices $n$.

- Let $I_1$ be this subinterval. We select an index $n_1$ such that $x_{n_1} \in I_1$. The length of $I_1$ is $M$.
    
- Next, we bisect $I_1$ into two equal halves. Again, at least one half must contain infinitely many terms of the sequence. We call this half $I_2$, and its length is $\frac{M}{2}$. We choose an index $n_2 > n_1$ such that $x_{n_2} \in I_2$.
    

By continuing this process inductively, we construct a sequence of nested closed intervals $I_0 \supset I_1 \supset I_2 \supset \dots \supset I_k$ and a corresponding subsequence $(x_{n_k})$ where $x_{n_k} \in I_k$ for each $k \in \mathbb{N}$, ensuring that $n_1 < n_2 < n_3 < \dots < n_k$.

The length of the $k$-th interval $I_k$ is precisely $\frac{2M}{2^k}$.

**Step 2: Proving the Subsequence is Cauchy**

We now claim that our constructed subsequence $(x_{n_k})$ is a Cauchy sequence.

Let $\epsilon > 0$. We need to find an integer $N \in \mathbb{N}$ such that for all $j, k \ge N$, the distance $\vert{}x_{n_j} - x_{n_k}\vert{} < \epsilon$.

Because our intervals are nested, if $j \ge N$ and $k \ge N$, both $I_j$ and $I_k$ are subsets of $I_N$. This guarantees that both $x_{n_j}$ and $x_{n_k}$ are contained entirely within $I_N$. Therefore, the distance between them cannot exceed the total length of the interval $I_N$:

$$\vert{}x_{n_j} - x_{n_k}\vert{} \le \frac{2M}{2^N}$$

**Step 3: The Archimedean Property (The Exact Assumption Step)**

To complete the Cauchy definition, we must guarantee that there actually exists an $N \in \mathbb{N}$ large enough to make $\frac{2M}{2^N} < \epsilon$.

Since $2^N > N$ for all $N \in \mathbb{N}$, it is strictly sufficient to find an $N$ such that:

$$\frac{2M}{N} < \epsilon \implies N > \frac{2M}{\epsilon}$$

> **Note:** This is the exact step where the **Archimedean Property** must be assumed. The Archimedean Property states that for any real number (in this case, $\frac{2M}{\epsilon}$), there exists a natural number $N$ that is strictly greater than it. Without this property, we could not prove that the length of the intervals arbitrarily approaches zero.

**Step 4: Applying the Cauchy Criterion**

Because the Archimedean Property guarantees the existence of such an $N$, it follows that for all $j, k \ge N$, we have:

$$\vert{}x_{n_j} - x_{n_k}\vert{} \le \frac{2M}{2^N} < \frac{2M}{N} < \epsilon$$

Thus, $(x_{n_k})$ is a Cauchy sequence.

Finally, we apply the **Cauchy Criterion** for real numbers, which states that a sequence of real numbers converges if and only if it is a Cauchy sequence. Since $(x_{n_k})$ is Cauchy, it converges.

We have successfully found a convergent subsequence from our original bounded sequence $(x_n)$, completing the proof. $\blacksquare$
