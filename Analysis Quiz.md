This updated active recall program combines structural analysis, quick-fire fact-checks, and precise Raw Theorem Recall prompts.

The theorem questions are intentionally non-generic: instead of asking you to simply "state a theorem," they force you to recall specific hypotheses, structural dependencies, and failure modes under perturbed conditions.

---

## 📅 Day 1: Sequences, Order, and Algebraic Limits (Sec 2.2–2.3)

## 📝 Structural & Fact Questions

- Q1.1: If $(x_n) \to 0$ and $(y_n)$ is a bounded sequence (not necessarily convergent), prove that $(x_n y_n) \to 0$. What structural property of bounds prevents divergence?
- Q1.2: If $(x_n)$ is a sequence of strictly positive numbers and $\lim(x_n) = x$, must $x > 0$? Provide the canonical counterexample where the boundary collapses.
- Q1.3: If $(x_n + y_n)$ converges, must $(x_n)$ and $(y_n)$ converge individually? Provide a quick-fire pair of oscillating sequences to prove your assertion.

## 📜 Raw Theorem Recall

- T1.1 (Algebraic Limit Theorem - Quotients): State the quotient portion of the Algebraic Limit Theorem exactly. Identify the _two_ distinct structural assumptions required for the denominator sequence $(y_n)$ and its limit $y$.
- T1.2 (Order Limit Theorem): Reconstruct the statement of the Order Limit Theorem. If the hypothesis $a_n \leq b_n$ is replaced with a strict inequality $a_n < b_n$ for all $n \in \mathbb{N}$, does the conclusion yield a strict inequality $a < b$? Prove or disprove.
- T1.3 (Squeeze Theorem): State the Squeeze Theorem for sequences. Pinpoint the exact step in its structural proof where the choice of $N = \max(N_1, N_2)$ forces the middle sequence into the $\epsilon$-neighborhood of the limit.

---

## 📅 Day 2: Monotone Sequences, Series, and Convergence Tests (Sec 2.4, 2.7)

## 📝 Structural & Fact Questions

- Q2.1: If a series $\sum a_n$ converges absolutely, and $(b_n)$ is a bounded sequence, does $\sum a_n b_n$ necessarily converge absolutely?
- Q2.2: Does the convergence of $\sum a_n^2$ imply the convergence of $\sum a_n$? Provide a simple fractional counterexample.
- Q2.3: Explain the precise algorithmic strategy used in Section 2.1 to rearrange the alternating harmonic series $\sum_{n=1}^\infty \frac{(-1)^{n+1}}{n}$ so that its partial sums diverge to $\infty$.

## 📜 Raw Theorem Recall

- T2.1 (Monotone Convergence Theorem): State the Monotone Convergence Theorem (MCT). If a sequence is decreasing and bounded below, what is the exact relationship between its limit and the infimum of the set of its terms?
- T2.2 (Alternating Series Test): State the Alternating Series Test hypotheses exactly. Why does the sequence $\frac{1}{2} - \frac{1}{2} + \frac{1}{3} - \frac{1}{4} + \frac{1}{3} - \frac{1}{6} + \frac{1}{3} - \dots$ fail to meet the raw criteria of this theorem?
- T2.3 (Cauchy Condensation Test): State the Cauchy Condensation Test theorem. What explicit behavior of the terms $a_n$ is mandatory for the equivalence $\sum a_n \iff \sum 2^k a_{2^k}$ to hold?

---

## 📅 Day 3: Subsequences, Bolzano-Weierstrass, and Cauchy Completeness (Sec 2.5–2.6)

## 📝 Structural & Fact Questions

- Q3.1: If every proper subsequence $(x_{n_k})$ of a sequence converges to the exact same value $L$, must the parent sequence $(x_n)$ converge to $L$?
- Q3.2: True or False: If a sequence $(x_n)$ satisfies the condition $\vert{}x_{n+1} - x_n\vert{} \to 0$ as $n \to \infty$, it is a Cauchy sequence. Provide a logarithmic counterexample if false.
- Q3.3: If a sequence $(x_n)$ is bounded and divergent, what is the minimum number of distinct subsequential limits it must possess?

## 📜 Raw Theorem Recall

- T3.1 (Subsequence Convergence): State the theorem regarding the convergence of subsequences. Identify the exact step in its proof where the index inequality $n_k \geq k$ is logically required.
- T3.2 (Bolzano-Weierstrass Theorem): State the Bolzano-Weierstrass Theorem. What is the minimal structural property of the real line $\mathbb{R}$ that prevents an arbitrary bounded sequence from escaping without a cluster point?
- T3.3 (Cauchy Criterion): State the Cauchy Criterion for sequences. Why is the set of rational numbers $\mathbb{Q}$ considered "incomplete" with respect to this theorem? State the specific sequence of rationals that exposes this gap.

---

## 📅 Day 4: Topology of the Real Line: Open, Closed, and Limit Points (Sec 3.1–3.2)

## 📝 Structural & Fact Questions

- Q4.1: Is the empty set $\emptyset$ open, closed, both, or neither? What about the full real line $\mathbb{R}$?
- Q4.2: Can an open set contain any isolated points? Explain using the structural definition of an isolated point versus an $\epsilon$-neighborhood.
- Q4.3: If $A$ is an open set and $B$ is a closed set, what can be definitively asserted about the topological classification of the set difference $A \setminus B$?

## 📜 Raw Theorem Recall

- T4.1 (Characterization of Open Sets): State the theorem that characterizes open sets via unions of intervals. Can an uncountable open set be expressed as a union of uncountably many _disjoint_ open intervals? Explain why based on the density of $\mathbb{Q}$.
- T4.2 (Characterization of Closed Sets): State the raw theorem that characterizes closed sets via limit points. Explain the exact mechanism by which a set $F$ contains all its limit points if and only if every convergent sequence in $F$ has its limit inside $F$.
- T4.3 (Properties of Open and Closed Sets): State the theorem governing arbitrary and finite operations on open sets. Provide a nested geometric interval counterexample showing why an _infinite_ intersection of open sets fails to remain open.

---

## 📅 Day 5: Compactness, Perfect Sets, and Connectedness (Sec 3.3–3.4)

## 📝 Structural & Fact Questions

- Q5.1: If a set $K \subseteq \mathbb{R}$ is compact, must its supremum $\sup K$ and infimum $\inf K$ be elements of $K$? Why?
- Q5.2: True or False: The union of two compact sets is compact. The arbitrary intersection of any collection of compact sets is compact.
- Q5.3: Can a perfect set contain an interval of the form $(a,b)$? Name a specific uncountable perfect set that contains absolutely zero intervals.

## 📜 Raw Theorem Recall

- T5.1 (Heine-Borel Theorem): State the Heine-Borel Theorem exactly. Why does the direction "Closed and Bounded $\implies$ Compact" fail for the set $K = [0, \sqrt{2}] \cap \mathbb{Q}$ if the target metric space is shifted from $\mathbb{R}$ to $\mathbb{Q}$?
- T5.2 (Cantor Set Properties): State the structural theorem defining the Cantor Set $C$. Explicitly state the two topological properties that make $C$ a perfect set, and recall how its total length behaves under infinite complementation.
- T5.3 (Characterization of Connected Sets): State the theorem characterizing connected sets in $\mathbb{R}$. If a set $A \subseteq \mathbb{R}$ is connected, and $x, y \in A$ with $x < y$, what must the theorem assert about every intermediate real number $c$ satisfying $x < c < y$?

---

## 📅 Day 6: Functional Limits, Continuity, and Compact Domains (Sec 4.1–4.4)

## 📝 Structural & Fact Questions

- Q6.1: In the $\epsilon$-$\delta$ definition of $\lim_{x \to c} f(x) = L$, why is the horizontal distance bounded by $0 < \vert{}x - c\vert{} < \delta$ instead of just $\vert{}x - c\vert{} < \delta$?
- Q6.2: If $f: \mathbb{R} \to \mathbb{R}$ is continuous at a point $c$, and $f(c) > 0$, prove that there exists an entire neighborhood $V_\delta(c)$ where $f(x) > 0$ for all $x \in V_\delta(c)$.
- Q6.3: Using the sequential divergence criterion, prove that the Dirichlet function $g(x) = \mathbf{1}_{\mathbb{Q}}(x)$ fails to have a functional limit at any point $c \in \mathbb{R}$.

## 📜 Raw Theorem Recall

- T6.1 (Sequential Criterion for Functional Limits): State the Sequential Criterion for Functional Limits exactly. Detail how this theorem transforms a statement about uncountably many continuous paths into a countable tracking mechanism.
- T6.2 (Preservation of Compact Sets): State the theorem for the Preservation of Compact Sets by continuous functions. If $f$ is continuous and $A$ is closed but unbounded, provide an exact counterexample showing that $f(A)$ need not be closed.
- T6.3 (Extreme Value Theorem): State the Extreme Value Theorem (EVT) exactly. Pinpoint where the structural machinery of the theorem breaks down if the underlying domain is altered to the open interval $(0, 1)$.

---

Here is the complete, rigorous answer key for your active recall program, including the specific sections and mathematical frameworks from Stephen Abbott’s _[Understanding Analysis](https://www.google.com/search?q=Understanding+Analysis&kgmid=/hkb/Cg4KCGxhbmd1YWdlEgJlbgoMCgR0eXBlEgRCT09LCiUKC2VudGl0eV9uYW1lEhZ1bmRlcnN0YW5kaW5nIGFuYWx5c2lz#sv=CBwS0QYKugUStwUK9wRBSmlUNHRKNGJnRUh3U1Fla19JMURBeThKSzVzNXlDQUh3X1hRcV9mMFJCa2pIYkNhY3lXYjJhZ245ZElnR1NSYVFELXB5Mkw5M0hnSTZEWmZlQWkybllrS0FUOWwxSE1hWlFhR1NxYTQ0U2dtU21VT2RFSU4zSno0dUNKbUwtQ2pnWmV2eDEwSy1NT3lDZGpqSVBtb1YtcVRRQy1hRVdmV01wRHdZWHY3UXAyWmlGaHAxdXI2aGNqSUxTWk1KVndXZUdOU3BIbWxaUmVDWnBKY0tBTVFzN2FWSzVCX3UzY1EyQ2pQYVZPdHhzZ3lvQTFRUmtLRkduZ3pDWU9oWlBhUVRtcENkS2puX1JyYnRXeUh0aWtlZ3dIZENpNHNSSVdveVlzV2QtUzR2LVQ0QXppOGVPQm82RFRnSFBnQzliS2tMZTNhdVVsNnRVTTJlbl92NUo5bFp6dHV0X2JlcG1JUnJpeVkzYlh3NTd0SzFWQUtyR2x6b01XaXdDSThiamJYc3hZcEVTZjk1LVlXVk9qTEFvdERsbWRQSF9oN25ldG9pU0Z5TE1oNFViMVgwVVFGWGVBRVZlNzRTMTVhNk5pYmY0M1dILXZmWnU0cDdJaDRlLThRNURkaWVneVZ1bTVzMjFDWUFPMjNyMGI0alBSLWNnekN4cmRsMUNZRkhHZ3JMS0RaT3FGdngwTDg0Y3B2ODBuS3FZTGcydVo0WkZvdGVZRU5MRUxPQ3plNTBaLTlJeEhDeU9uTG5odkcyZk0zRzVXY2QyaVJRSDIyV01EdDBQTVU0ZV9VME1kTWdLT21meG80VGo3VnBwSldrcHNxUnVnVXkwEhdHTHhKYXZtNE9fVEVydUVQOUxLd3FBTRoiQURzcjlmVHlWc1VzRm11OFRUR2lIUGRleWFVTW41RTUxdxIENzg1NBoBMyIbCgFxEhZVbmRlcnN0YW5kaW5nIEFuYWx5c2lzImoKBWtnbWlkEmEvaGtiL0NnNEtDR3hoYm1kMVlXZGxFZ0psYmdvTUNnUjBlWEJsRWdSQ1QwOUxDaVVLQzJWdWRHbDBlVjl1WVcxbEVoWjFibVJsY25OMFlXNWthVzVuSUdGdVlXeDVjMmx6KAAYRSD8_6B5)_ (p. 5).

---

## 📅 Day 1: Sequences, Order, and Algebraic Limits (Sec 2.2–2.3)

## 📝 Structural & Fact Questions

## Q1.1: If $(x_n) \to 0$ and $(y_n)$ is a bounded sequence, prove that $(x_n y_n) \to 0$.

- Answer: Because $(y_n)$ is bounded, there exists $M > 0$ such that $\vert{}y_n\vert{} \leq M$ for all $n \in \mathbb{N}$ (p. 28). Let $\epsilon > 0$. Since $x_n \to 0$, there exists $N \in \mathbb{N}$ such that for all $n \geq N$, $\vert{}x_n - 0\vert{} < \frac{\epsilon}{M}$. Therefore, for all $n \geq N$:  
    $$\vert{}x_n y_n - 0\vert{} = \vert{}x_n\vert{}\vert{}y_n\vert{} < \left(\frac{\epsilon}{M}\right) M = \epsilon$$  
    This proves $\lim(x_n y_n) = 0$.
- Book Source: Section 2.2 (Exercises and Example discussions) (p. 12).

## Q1.2: If $(x_n) > 0$ for all $n$ and $\lim(x_n) = x$, must $x > 0$?

- Answer: False. The boundary conditions collapse to inclusive inequalities under limits.
- Canonical Counterexample: Let $x_n = \frac{1}{n}$. Every term is strictly positive ($x_n > 0$), but $\lim\left(\frac{1}{n}\right) = 0$, which is not strictly greater than 0.
- Book Source: Section 2.3 (Order Limit Theorem implications) (p. 12).

## Q1.3: If $(x_n + y_n)$ converges, must $(x_n)$ and $(y_n)$ converge individually?

- Answer: No.
- Canonical Counterexample: Let $x_n = (-1)^n$ and $y_n = (-1)^{n+1}$. Both oscillate and diverge individually. However, their sum sequence is $x_n + y_n = 0$ for all $n$, which trivially converges to 0.
- Book Source: Section 2.3 (Algebraic Limit Theorem boundary scenarios) (p. 12).

## 📜 Raw Theorem Recall

## T1.1: Algebraic Limit Theorem (Quotient Portion)

- Hypotheses: Given $\lim x_n = x$ and $\lim y_n = y$, if (1) $y_n \neq 0$ for all $n \in \mathbb{N}$ and (2) $y \neq 0$, then $\lim(x_n / y_n) = x / y$.
- Book Source: Theorem 2.3.3 (Part iv), Section 2.3 (p. 12).

## T1.2: Order Limit Theorem

- Hypotheses & Statement: If $a_n \leq b_n$ for all $n \in \mathbb{N}$, and $\lim a_n = a, \lim b_n = b$, then $a \leq b$. If the hypothesis is shifted to strict inequality ($a_n < b_n$), the conclusion does not change to $a < b$; it remains $a \leq b$ (as demonstrated by $a_n = 0$ and $b_n = \frac{1}{n}$, where $0 < \frac{1}{n}$ but their limits are equal).
- Book Source: Theorem 2.3.4, Section 2.3 (p. 12).

## T1.3: Squeeze Theorem

- Statement: If $x_n \leq y_n \leq z_n$ for all $n \in \mathbb{N}$, and $\lim x_n = L = \lim z_n$, then $\lim y_n = L$.
- Proof Mechanism: For a given $\epsilon > 0$, choose $N_1$ such that $L - \epsilon < x_n$ for all $n \geq N_1$, and choose $N_2$ such that $z_n < L + \epsilon$ for all $n \geq N_2$. Setting $N = \max(N_1, N_2)$ yields:  
    $$L - \epsilon < x_n \leq y_n \leq z_n < L + \epsilon \implies \vert{}y_n - L\vert{} < \epsilon \quad \forall n \geq N$$
- Book Source: Theorem 2.3.8 (Requested in Exercise 2.3.3), Section 2.3 (p. 12).

---

## 📅 Day 2: Monotone Sequences, Series, and Convergence Tests (Sec 2.4, 2.7)

## 📝 Structural & Fact Questions

## Q2.1: If $\sum a_n$ converges absolutely and $(b_n)$ is bounded, does $\sum a_n b_n$ converge absolutely?

- Answer: Yes. Since $(b_n)$ is bounded, $\vert{}b_n\vert{} \leq M$ for some $M > 0$ (p. 28). Therefore, $\vert{}a_n b_n\vert{} \leq M\vert{}a_n\vert{}$. Because $\sum \vert{}a_n\vert{}$ converges, $\sum M\vert{}a_n\vert{}$ converges by limit properties, and $\sum \vert{}a_n b_n\vert{}$ converges by the Direct Comparison Test.
- Book Source: Section 2.7 (p. 12).

## Q2.2: Does the convergence of $\sum a_n^2$ imply the convergence of $\sum a_n$?

- Answer: No.
- Canonical Counterexample: Let $a_n = \frac{1}{n}$. The series of squares is $\sum \frac{1}{n^2}$, which converges ($p=2$). However, the original series $\sum \frac{1}{n}$ is the Harmonic series, which diverges.
- Book Source: Section 2.7 (p. 12).

## Q2.3: Explain the algorithmic layout to make the Alternating Harmonic Series diverge to $\infty$.

- Answer: Because the positive terms $\left(1, \frac{1}{3}, \frac{1}{5}, \dots\right)$ sum to $\infty$, you can take a single negative term (e.g., $-\frac{1}{2}$), and then append as many consecutive positive terms as needed to drive the partial sum above 1. Next, subtract $-\frac{1}{4}$ and append positive terms until the total exceeds 2. Repeating this pattern drives the sequence of partial sums to $\infty$.
- Book Source: Section 2.1 (Discussion on Rearrangements) (p. 12).

## 📜 Raw Theorem Recall

## T2.1: Monotone Convergence Theorem

- Statement: A monotone sequence converges if and only if it is bounded.
- Infimum Relationship: If a sequence $(x_n)$ is decreasing and bounded below, it converges to $x = \inf\{x_n : n \in \mathbb{N}\}$.
- Book Source: Theorem 2.4.2, Section 2.4 (p. 12).

## T2.2: Alternating Series Test

- Hypotheses: Let $(a_n)$ be a sequence satisfying: (1) $a_1 \geq a_2 \geq a_3 \geq \dots \geq 0$ (must be monotonically decreasing), and (2) $\lim a_n = 0$. Then $\sum (-1)^{n+1} a_n$ converges.
- Failure Analysis: The sequence provided in the prompt oscillates up and down in magnitude ($\frac{1}{2} \to \frac{1}{3} \to \frac{1}{4} \to \frac{1}{3}$), directly violating the requirement to be strictly decreasing.
- Book Source: Theorem 2.7.7, Section 2.7 (p. 12).

## T2.3: Cauchy Condensation Test

- Statement: Suppose $(a_n)$ is a decreasing sequence of positive terms ($a_n \geq a_{n+1} \geq 0$). Then, $\sum_{n=1}^\infty a_n$ converges if and only if $\sum_{k=0}^\infty 2^k a_{2^k}$ converges.
- Mandatory Behavior: The terms must be non-negative and non-increasing. Without monotonicity, grouping terms by blocks of $2^k$ breaks down.
- Book Source: Theorem 2.4.6, Section 2.4 (p. 12).

---

## 📅 Day 3: Subsequences, Bolzano-Weierstrass, and Cauchy Completeness (Sec 2.5–2.6)

## 📝 Structural & Fact Questions

## Q3.1: If every proper subsequence $(x_{n_k})$ converges to $L$, must the parent sequence converge to $L$?

- Answer: Yes. If every subsequence converges to $L$, then the canonical subsequence $(x_n)$ itself (which is technically a subsequence of itself where $n_k = k$) must converge to $L$.
- Book Source: Section 2.5 (p. 12).

## Q3.2: If $\vert{}x_{n+1} - x_n\vert{} \to 0$, is it guaranteed to be a Cauchy sequence?

- Answer: False. Consecutive terms getting closer together does not prevent the full sequence from drifting apart across long distances.
- Logarithmic Counterexample: Let $x_n = \ln(n)$ or $x_n = \sum_{k=1}^n \frac{1}{k}$. Here, $\vert{}x_{n+1} - x_n\vert{} = \frac{1}{n+1} \to 0$, but the sequence grows without bound and diverges, meaning it cannot be Cauchy.
- Book Source: Section 2.6 (p. 12).

## Q3.3: Bounded and divergent sequence: minimum number of subsequential limits?

- Answer: Two. By the Bolzano-Weierstrass theorem, a bounded sequence must contain at least one subsequential limit. If it contained _only_ one unique subsequential limit, a standard theorem states that the parent sequence would have to converge to that limit. Because it diverges, it must possess at least two distinct subsequential limits (e.g., $x_n = (-1)^n$ has subsequential limits $\{-1, 1\}$).
- Book Source: Section 2.5 (p. 12).

## 📜 Raw Theorem Recall

## T3.1: Subsequence Convergence Theorem

- Statement: If a sequence $(x_n)$ converges to $x$, then any subsequence $(x_{n_k})$ of $(x_n)$ also converges to $x$.
- Index Requirement: The indices must satisfy $n_k \geq k$. This ensures that when we choose an index $k \geq N$, the subsequence index $n_k$ is guaranteed to be $\geq N$, allowing us to inherit the convergence bounds of the parent sequence.
- Book Source: Theorem 2.5.2, Section 2.5 (p. 12).

## T3.2: Bolzano-Weierstrass Theorem

- Statement: Every bounded sequence contains a convergent subsequence.
- Minimal Property: The Completeness (or the Least Upper Bound property) of $\mathbb{R}$. Without it, the sub-divided intervals would close in around a missing gap (hole), preventing the subsequence from converging within that number system.
- Book Source: Theorem 2.5.5, Section 2.5 (p. 12).

## T3.3: Cauchy Criterion

- Statement: A sequence converges if and only if it is a Cauchy sequence.
- Incompleteness Example: Let $x_n$ be the sequence of rational approximations of $\sqrt{2}$ (i.e., $1, 1.4, 1.41, 1.414, \dots$). This sequence is Cauchy and its terms are strictly in $\mathbb{Q}$, but it fails to converge to an element _inside_ $\mathbb{Q}$.
- Book Source: Theorem 2.6.4, Section 2.6 (p. 12).

---

## 📅 Day 4: Topology of the Real Line: Open, Closed, and Limit Points (Sec 3.1–3.2)

## 📝 Structural & Fact Questions

## Q4.1: Topological classification of $\emptyset$ and $\mathbb{R}$.

- Answer: Both sets are both open and closed (often called "clopen").
- Proof Context: They vacuously satisfy the conditions: every point in $\emptyset$ is an interior point (since no points exist), and $\emptyset$ contains all its limit points. For $\mathbb{R}$, every $\epsilon$-neighborhood stays within $\mathbb{R}$ (open), and it contains all real numbers, including all possible limit points (closed).
- Book Source: Section 3.2 (p. 12).

## Q4.2: Can an open set contain any isolated points?

- Answer: No. If $x$ is an isolated point of $A$, there exists an $\epsilon$-neighborhood $V_\epsilon(x)$ that contains _no points of $A$ other than $x$ itself_. However, if $A$ is open, every point must be an interior point, requiring an entire neighborhood $V_\delta(x)$ to be _completely contained_ inside $A$. These two conditions are mutually exclusive.
- Book Source: Section 3.2 (p. 12).

## Q4.3: Topological classification of set difference $A \setminus B$ where $A$ is open and $B$ is closed.

- Answer: Open. By set theory, $A \setminus B = A \cap B^c$. Because $B$ is closed, its complement $B^c$ is open. The intersection of two open sets is guaranteed to be open.
- Book Source: Section 3.2 (p. 12).

## 📜 Raw Theorem Recall

## T4.1: Characterization of Open Sets

- Statement: A set is open if and only if it can be written as a countable union of disjoint open intervals.
- Uncountable Interrogation: No. Every non-empty open interval contains a rational number by the density of $\mathbb{Q}$ (p. 35). Since the intervals must be disjoint, each interval matches with a unique rational number. Because $\mathbb{Q}$ is countable, the collection of disjoint intervals is strictly limited to a countable number (p. 40).
- Book Source: Theorem 3.2.14, Section 3.2 (p. 12).

## T4.2: Characterization of Closed Sets

- Statement: A set $F \subseteq \mathbb{R}$ is closed if and only if it contains all its limit points.
- Mechanism: If a sequence $(a_n) \subseteq F$ converges to $x$, every neighborhood of $x$ contains elements of the sequence (and thus elements of $F$). This fits the definition of a limit point, forcing $x \in F$ because the set is closed.
- Book Source: Theorem 3.2.6, Section 3.2 (p. 12).

## T4.3: Properties of Open and Closed Sets

- Statement: The intersection of a _finite_ collection of open sets is open; the intersection of an _arbitrary_ collection of open sets is not guaranteed to be open.
- Geometric Counterexample: Let $O_n = \left(-\frac{1}{n}, \frac{1}{n}\right)$ for $n \in \mathbb{N}$. Each $O_n$ is an open interval. However, their infinite intersection is:  
    $$\bigcap_{n=1}^\infty \left(-\frac{1}{n}, \frac{1}{n}\right) = \{0\}$$  
    The single-element set $\{0\}$ is closed, not open.
- Book Source: Theorem 3.2.3, Section 3.2 (p. 12).

---

## 📅 Day 5: Compactness, Perfect Sets, and Connectedness (Sec 3.3–3.4)

## 📝 Structural & Fact Questions

## Q5.1: If $K$ is compact, must $\sup K$ and $\inf K$ belong to $K$?

- Answer: Yes. Since $K$ is compact, it is closed and bounded. By definition of the supremum, $\sup K$ is a limit point of $K$ (or an isolated maximum). Because $K$ is a closed set, it must contain all its limit points, guaranteeing $\sup K \in K$ and $\inf K \in K$.
- Book Source: Section 3.3 (p. 12).

## Q5.2: Truth values of compact set operations.

- Answer:
    
    1. The union of two compact sets is compact: True (finite unions of closed and bounded sets remain closed and bounded).
    2. The arbitrary intersection of compact sets is compact: True (arbitrary intersections of closed sets are closed, and the result is bounded by the individual sets).
    
- Book Source: Section 3.3 (p. 12).

## Q5.3: Can a perfect set contain an interval $(a,b)$? Uncountable perfect set with no intervals?

- Answer: Yes (e.g., the closed interval $[a, b]$ is perfect and contains open sub-intervals).
- Zero-Interval Set: The Cantor Set is an uncountable perfect set that is totally disconnected and contains absolutely zero intervals.
- Book Source: Section 3.1 & 3.4 (p. 12).

## 📜 Raw Theorem Recall

## T5.1: Heine-Borel Theorem

- Statement: A subset $K \subseteq \mathbb{R}$ is compact if and only if it is closed and bounded.
- Failure Analysis: In the metric space $\mathbb{Q}$, the set $K = [0, \sqrt{2}] \cap \mathbb{Q}$ is bounded and closed relative to $\mathbb{Q}$. However, if we construct a sequence of rationals in $K$ converging to $\sqrt{2}$, that sequence has no limit _within $\mathbb{Q}$_. This breaks sequential compactness, showing that the Heine-Borel theorem relies completely on the completeness of the underlying space $\mathbb{R}$.
- Book Source: Theorem 3.3.4, Section 3.3 (p. 12).

## T5.2: Cantor Set Properties

- Statement: The Cantor Set $C$ is a closed, uncountably infinite set with a total length (measure) of 0.
- Perfect Set Criteria: It is closed and contains no isolated points (every point in the Cantor set is a limit point of other points in the Cantor set).
- Book Source: Theorem 3.4.4, Section 3.4 (p. 12).

## T5.3: Characterization of Connected Sets

- Statement: A set $A \subseteq \mathbb{R}$ is connected if and only if for all $x, y \in A$ with $x < y$, the intermediate interval $[x, y] \subseteq A$.
- Assertion: If $x, y \in A$ and $x < c < y$, then $c \in A$. Connected sets in $\mathbb{R}$ cannot have gaps; they must be intervals.
- Book Source: Theorem 3.4.7, Section 3.4 (p. 12).

---

## 📅 Day 6: Functional Limits, Continuity, and Compact Domains (Sec 4.1–4.4)

## 📝 Structural & Fact Questions

## Q6.1: Why do we specify $0 < \vert{}x - c\vert{} < \delta$ instead of just $\vert{}x - c\vert{} < \delta$?

- Answer: The condition $0 < \vert{}x - c\vert{}$ explicitly enforces $x \neq c$. Functional limits evaluate the behavior of a function as $x$ _approaches_ $c$, completely independent of the actual value of $f(c)$ (which may be undefined or mismatched, as seen in removable discontinuities).
- Book Source: Section 4.2 (p. 12).

## Q6.2: If $f(c) > 0$ and $f$ is continuous, prove $f(x) > 0$ on a full neighborhood.

- Answer: Let $\epsilon = \frac{f(c)}{2} > 0$. Since $f$ is continuous at $c$, there exists a neighborhood $V_\delta(c)$ such that for all $x \in V_\delta(c)$, $\vert{}f(x) - f(c)\vert{} < \epsilon$. This unfolds to:  
    $$f(c) - \frac{f(c)}{2} < f(x) < f(c) + \frac{f(c)}{2} \implies f(x) > \frac{f(c)}{2} > 0$$
- Book Source: Section 4.3 (p. 12).

## Q6.3: Prove the Dirichlet function $g(x) = \mathbf{1}_{\mathbb{Q}}(x)$ diverges everywhere.

- Answer: Let $c \in \mathbb{R}$. By the density of $\mathbb{Q}$ and the irrationals, we can construct two distinct sequences (p. 35): $(x_n) \subseteq \mathbb{Q}$ where $x_n \to c$, and $(y_n) \subseteq \mathbb{R} \setminus \mathbb{Q}$ where $y_n \to c$. Evaluating the function yields:  
    $$\lim f(x_n) = \lim(1) = 1 \quad \text{and} \quad \lim f(y_n) = \lim(0) = 0$$  
    Because $1 \neq 0$, the sequential divergence criterion confirms that no functional limit exists at $c$.
- Book Source: Section 4.1 & 4.2 (p. 12).

## 📜 Raw Theorem Recall

## T6.1: Sequential Criterion for Functional Limits

- Statement: Given a function $f: A \to \mathbb{R}$, $\lim_{x \to c} f(x) = L$ if and only if for every sequence $(x_n) \subseteq A$ satisfying $x_n \neq c$ and $x_n \to c$, it follows that $f(x_n) \to L$.
- Tracking Mechanism: It maps uncountable directional limit paths onto discrete, countable sequence limits, allowing the full diagnostic power of Chapter 2 sequence theorems to be applied directly to functional tracking.
- Book Source: Theorem 4.2.3, Section 4.2 (p. 12).

## T6.2: Preservation of Compact Sets

- Statement: If $f: A \to \mathbb{R}$ is continuous and $K \subseteq A$ is compact, then the image set $f(K)$ is compact.
- Closed/Unbounded Counterexample: Let $A = [1, \infty)$, which is closed but unbounded. Let $f(x) = \frac{1}{x}$, which is continuous on $A$. The image set is $f(A) = (0, 1]$. This resulting set is not closed, confirming that the domain must be closed _and_ bounded (compact) to guarantee a compact image.
- Book Source: Theorem 4.4.1, Section 4.4 (p. 12).

## T6.3: Extreme Value Theorem

- Statement: If $f: K \to \mathbb{R}$ is continuous on a compact set $K$, then $f$ attains a maximum and a minimum value on $K$.
- Failure Analysis: Let the domain be the non-compact open interval $(0, 1)$, and let $f(x) = x$. The function is continuous, and its bounds are bounded by $(0, 1)$, but it never reaches its supremum (1) or its infimum (0) anywhere inside the open domain.
- Book Source: Theorem 4.4.2, Section 4.4 (p. 12).

---


