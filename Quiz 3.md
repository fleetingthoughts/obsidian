---
parent: "[[_Fleeting]]"
tags:
  - "#fleeting"
date_created: "2026-05-23"
---
This is a structured 7-day interleaved study curriculum. Each day delivers a balanced mix of your four core subjects, immediately paired with its rigorous answer key and textbook justifications.

---

## 📅 Day 1: Convergence, Operations, and Expectations

## 📝 The Quiz

- Q1 (Real Analysis): State the strict definition of a Cauchy sequence of real numbers.
- Q2 (Linear Algebra): List the three valid elementary row operations applicable to a matrix.
- Q3 (Math Stats): State Chebyshev's Inequality for a random variable $X$ with mean $\mu$ and variance $\sigma^2$.
- Q4 (Calculus): State the structural definition of a Taylor series of a smooth function $f(x)$ expanded around a point $x_0$.

## 🔑 The Answer Key

## Q1 (Real Analysis)

- Definition: A sequence $(a_n)$ is a Cauchy sequence if for every $\epsilon > 0$, there exists an $N \in \mathbb{N}$ such that for all $m, n \geq N$, we have $|a_m - a_n| < \epsilon$.
- Explanation: Abbott notes that this definition allows us to prove a sequence converges by looking only at its internal elements, without needing to know the target limit in advance (stephen-ab... p. 12).

## Q2 (Linear Algebra)

- The Operations:
    
    1. Interchanging any two rows.
    2. Multiplying a row by a non-zero scalar.
    3. Adding a scalar multiple of one row to another row.
    
- Explanation: Friedberg states that elementary row operations preserve the solution set of linear systems and form the computational basis for computing matrix ranks and inverses (stephen-ab... p. 89).

## Q3 (Math Stats)

- Formula: $P(|X - \mu| \geq k\sigma) \leq \frac{1}{k^2}$ for any constant $k > 0$.
- Explanation: Hogg highlights this as a universal bound mapping probability to variance, working independently of the underlying shape of the distribution (hogg-mathe... p. 7).

## Q4 (Calculus)

- Formula: $\sum_{n=0}^{\infty} \frac{f^{(n)}(x_0)}{n!} (x - x_0)^n$.
- Explanation: Courant frames this as the absolute limiting extension of algebraic polynomials, allowing infinite transcendental processes to be analyzed through polynomial approximations.

---

## 📅 Day 2: Continuity, Transpositions, and Conditional Probability

## 📝 The Quiz

- Q1 (Real Analysis): State the definition of Uniform Continuity on a set $A$.
- Q2 (Linear Algebra): Define the transpose $A^t$ of an $m \times n$ matrix $A$, and clarify what makes a matrix symmetric.
- Q3 (Math Stats): State Bayes' Theorem for a partition of the sample space $A_1, A_2, \dots, A_k$ given an event $B$.
- Q4 (Calculus): State the Chain Rule for the derivative of a composite function $h(x) = f(g(x))$.

## 🔑 The Answer Key

## Q1 (Real Analysis)

- Definition: $f$ is uniformly continuous on $A$ if $\forall \epsilon > 0, \exists \delta > 0$ such that $\forall x, y \in A$, $|x - y| < \delta \implies |f(x) - f(y)| < \epsilon$.
- Explanation: Abbott highlights that $\delta$ is picked globally for the entire set, depending solely on $\epsilon$ rather than changing at each local point (stephen-ab... p. 13).

## Q2 (Linear Algebra)

- Definition: The transpose $A^t$ is an $n \times m$ matrix defined by $(A^t)_{ij} = A_{ji}$. A matrix is symmetric if it is square and $A^t = A$ (stephen-ab... p. 114).
- Explanation: Friedberg treats symmetric configurations as fundamental subspaces within matrix environments, setting up the foundation for spectral diagonalization (stephen-ab... p. 114).

## Q3 (Math Stats)

- Formula: $P(A_i | B) = \frac{P(B | A_i)P(A_i)}{\sum_{j=1}^k P(B | A_j)P(A_j)}$.
- Explanation: Hogg describes this as the core framework for inverse conditional probability, allowing observed data $B$ to update our background belief in hypotheses $A_i$ (hogg-mathe... p. 9).

## Q4 (Calculus)

- Formula: $h'(x) = f'(g(x)) \cdot g'(x)$.
- Assumption: $g$ must be differentiable at $x$, and $f$ must be differentiable at $g(x)$.
- Explanation: Courant emphasizes this as a tool that reduces rates of change across nested functional linkages down to product interactions.

---

## 📅 Day 3: Compactness, Compositions, and Discrete Inferences

## 📝 The Quiz

- Q1 (Real Analysis): State the Extreme Value Theorem using sequential compactness.
- Q2 (Linear Algebra): Let $T: V \to W$ and $U: W \to Z$ be linear transformations. State how the matrix representation of the composition $UT$ relates to the individual matrix representations of $U$ and $T$.
- Q3 (Math Stats): Define the probability mass function of a Poisson distribution with parameter $\lambda > 0$, and state its mean and variance.
- Q4 (Calculus): State the definition of the Riemann Integral of a bounded function $f(x)$ on an interval $[a, b]$ using upper and lower sums.

## 🔑 The Answer Key

## Q1 (Real Analysis)

- Theorem: If $f: K \to \mathbb{R}$ is continuous on a compact set $K$, then $f(K)$ is compact, meaning $f$ achieves its maximum and minimum values on $K$.
- Explanation: Abbott uses sequential compactness to pull a convergent subsequence from any maximizing path, forcing the limit to sit squarely inside the set boundaries (stephen-ab... p. 13).

## Q2 (Linear Algebra)

- Theorem: Let $[UT]_\alpha^\gamma = [U]_\beta^\gamma [T]_\alpha^\beta$, where $\alpha, \beta, \gamma$ are ordered bases for $V, W, Z$ respectively.
- Explanation: Friedberg highlights this theorem to show matrix multiplication is not an arbitrary rule; it is explicitly engineered to mirror the composition of linear mappings (stephen-ab... p. 88).

## Q3 (Math Stats)

- Definition: $p(x) = \frac{e^{-\lambda} \lambda^x}{x!}$ for $x = 0, 1, 2, \dots$ (hogg-mathe... p. 8)
- Parameters: $\text{Mean} = \lambda$, $\text{Variance} = \lambda$ (hogg-mathe... p. 8).
- Explanation: Hogg structures this distribution to model the frequency of random independent events occurring over fixed intervals of time or space (hogg-mathe... p. 8).

## Q4 (Calculus)

- Definition: $f(x)$ is Riemann integrable on $[a, b]$ if the supremum of all lower Darboux sums matches the infimum of all upper Darboux sums: $\underline{\int}_{a}^{b} f(x) \, dx = \overline{\int}_{a}^{b} f(x) \, dx$.
- Explanation: Courant builds this infrastructure to resolve areas under erratic graphs by trapping functional values inside a tightening squeeze of rectangular grids.

---

## 📅 Day 4: Open Covers, Spatial Sums, and Normal Continuous Models

## 📝 The Quiz

- Q1 (Real Analysis): State the characterization of a connected set $A \subseteq \mathbb{R}$.
- Q2 (Linear Algebra): Define the sum $W_1 + W_2$ of two subspaces of a vector space $V$, and state the condition required for it to be a direct sum $W_1 \oplus W_2$.
- Q3 (Math Stats): State the probability density function of a continuous Normal Distribution with mean $\mu$ and variance $\sigma^2$.
- Q4 (Calculus): State Rolle's Theorem, detailing its three explicit functional constraints.

## 🔑 The Answer Key

## Q1 (Real Analysis)

- Definition: A set $A \subseteq \mathbb{R}$ is connected if and only if whenever $a < b$ are points in $A$, then any point $c$ satisfying $a < c < b$ must also belong to $A$ (i.e., $A$ is an interval).
- Explanation: Abbott explains that connectivity avoids structural partitions. It guarantees you can never split the set into two disjoint open fragments (stephen-ab... p. 12).

## Q2 (Linear Algebra)

- Definition: $W_1 + W_2 = \{x_1 + x_2 : x_1 \in W_1 \text{ and } x_2 \in W_2\}$. It forms a direct sum $W_1 \oplus W_2$ if and only if $W_1 \cap W_2 = \{0\}$ (stephen-ab... p. 37).
- Explanation: Friedberg details that a direct sum guarantees every vector in the unified space can be written in exactly one way as a combination of elements from each subspace (stephen-ab... p. 39).

## Q3 (Math Stats)

- Definition: $f(x) = \frac{1}{\sigma \sqrt{2\pi}} \exp\left[ -\frac{1}{2}\left(\frac{x - \mu}{\sigma}\right)^2 \right]$ for $-\infty < x < \infty$ (hogg-mathe... p. 8).
- Explanation: Hogg frames this continuous model as the universal limit for averaged systems, acting as the fundamental distribution underpinning the Central Limit Theorem (hogg-mathe... p. 8).

## Q4 (Calculus)

- Theorem: If $f(x)$ is continuous on $[a, b]$, differentiable on $(a, b)$, and $f(a) = f(b)$, then there exists a $c \in (a, b)$ such that $f'(c) = 0$.
- Explanation: Courant interprets this mechanically: if an path returns back to its starting height, it must flatten out completely at an intermediate peak or trough.

---

## 📅 Day 5: Intermediate Properties, Bases, and Likelihood Mappings

## 📝 The Quiz

- Q1 (Real Analysis): State the Intermediate Value Theorem for continuous functions.
- Q2 (Linear Algebra): Define what constitutes a basis for a vector space $V$.
- Q3 (Math Stats): Define the Maximum Likelihood Estimator (MLE) $\hat{\theta}$ for a parameter space.
- Q4 (Calculus): State the derivative of an inverse function $f^{-1}(x)$ at a point $y_0 = f(x_0)$.

## 🔑 The Answer Key

## Q1 (Real Analysis)

- Theorem: If $f: [a, b] \to \mathbb{R}$ is continuous, and $k$ sits between $f(a)$ and $f(b)$, then there is a point $c \in (a, b)$ satisfying $f(c) = k$.
- Explanation: Abbott highlights that continuous operations preserve path connectedness, ensuring the mapping skips no values across the spectrum (stephen-ab... p. 13).

## Q2 (Linear Algebra)

- Definition: A basis $\beta$ for a vector space $V$ is a subset that is simultaneously linearly independent and spans the entire space $V$ ($\text{span}(\beta) = V$).
- Explanation: Friedberg notes that a basis represents a minimal generating environment, locking down an absolute coordinate frame for structural mapping (stephen-ab... p. 43).

## Q3 (Math Stats)

- Definition: The MLE $\hat{\theta}$ is the parameter value that maximizes the likelihood function: $L(\hat{\theta}; \mathbf{x}) = \sup_{\theta \in \Omega} L(\theta; \mathbf{x})$.
- Explanation: Hogg outlines this estimation strategy to calibrate parameters so that our observed empirical sample becomes the most probable outcome possible under the model (hogg-mathe... p. 9).

## Q4 (Calculus)

- Formula: $(f^{-1})'(y_0) = \frac{1}{f'(x_0)}$, provided that $f'(x_0) \neq 0$.
- Explanation: Courant demonstrates this as a geometric inversion property: swapping coordinate axes flips the slope of the tangent line across a reciprocal layout.

---

## 📅 Day 6: Series of Functions, Operators, and Confidence Intervals

## 📝 The Quiz

- Q1 (Real Analysis): State the theorem regarding the term-by-term integration of a series of functions under uniform convergence.
- Q2 (Linear Algebra): Define an inner product on a vector space $V$ over $\mathbb{R}$.
- Q3 (Math Stats): State the structural formulation for a $(1-\alpha)100\%$ Confidence Interval for a population mean $\mu$ when variance $\sigma^2$ is unknown and sample size is small.
- Q4 (Calculus): State the formula for the volume of a solid of revolution generated by rotating $f(x)$ on $[a, b]$ around the $x$-axis using the disk method.

## 🔑 The Answer Key

## Q1 (Real Analysis)

- Theorem: If $f_n \to f$ uniformly on $[a, b]$, and each $f_n$ is integrable, then $f$ is integrable and $\lim_{n \to \infty} \int_{a}^{b} f_n(x) \, dx = \int_{a}^{b} f(x) \, dx$.
- Explanation: Abbott stresses that uniform controls are necessary to safely swap limit operators and integrals without leaking tracking bounds (stephen-ab... p. 13).

## Q2 (Linear Algebra)

- Definition: A mapping associating a scalar $\langle x, y \rangle$ to vector pairs, satisfying:
    
    1. Linearity: $\langle cx + y, z \rangle = c\langle x, z \rangle + \langle y, z \rangle$.
    2. Symmetry: $\langle x, y \rangle = \langle y, x \rangle$.
    3. Positive-Definiteness: $\langle x, x \rangle \geq 0$, and $\langle x, x \rangle = 0 \iff x = 0$.
    
- Explanation: Friedberg builds this framework to introduce geometric parameters like distance, length, and perpendicularity to abstract vector landscapes (stephen-ab... p. 89).

## Q3 (Math Stats)

- Formula: $\bar{X} \pm t_{\alpha/2, n-1} \left( \frac{S}{\sqrt{n}} \right)$ (hogg-mathe... p. 8).
- Explanation: Hogg utilizes Student's $t$-distribution here to adjust confidence bounds outward, compensating for the extra uncertainty introduced by estimating the variance (hogg-mathe... p. 8).

## Q4 (Calculus)

- Formula: $V = \pi \int_{a}^{b} [f(x)]^2 \, dx$.
- Explanation: Courant structures this by stacking infinitesimal circular cross-sections along the axis of rotation to calculate total spatial volumes.

---

## 📅 Day 7: Cardinality, Eigen-Environments, and Sufficiency

## 📝 The Quiz

- Q1 (Real Analysis): State Cantor's Theorem regarding the cardinality of power sets.
- Q2 (Linear Algebra): Define what it means for a scalar $\lambda$ and a non-zero vector $v$ to be an eigenvalue and eigenvector of an operator $T$.
- Q3 (Math Stats): State the Fisher-Neyman Factorization Theorem for identifying a sufficient statistic.
- Q4 (Calculus): State the analytical formula for finding the arc length of a continuously differentiable curve $f(x)$ on $[a, b]$.

## 🔑 The Answer Key

## Q1 (Real Analysis)

- Theorem: For any set $A$, the power set $\mathcal{P}(A)$ has a strictly larger cardinality than $A$ ($A \nsim \mathcal{P}(A)$).
- Explanation: Abbott demonstrates through Cantor's diagonal argument that infinite scales are stratified, meaning there is no cap on the sizing tiers of infinity (stephen-ab... p. 12).

## Q2 (Linear Algebra)

- Definition: A scalar $\lambda$ and a non-zero vector $v \in V$ satisfy $T(v) = \lambda v$.
- Explanation: Friedberg frames this as an invariant direction layout. The transformation $T$ acts along the line of the eigenvector $v$ through simple scalar stretching (stephen-ab... p. 89).

## Q3 (Math Stats)

- Theorem: A statistic $Y = u(\mathbf{X})$ is sufficient for $\theta$ if and only if the joint density factors as: $f(\mathbf{x}; \theta) = g(u(\mathbf{x}); \theta) \cdot h(\mathbf{x})$, where $h(\mathbf{x})$ is completely independent of $\theta$.
- Explanation: Hogg notes that this isolation pattern strips away data clutter, leaving only the sufficient kernel necessary to compute parameter inferences (hogg-mathe... p. 9).

## Q4 (Calculus)

- Formula: $L = \int_{a}^{b} \sqrt{1 + [f'(x)]^2} \, dx$.
- Explanation: Courant applies the local Pythagorean theorem across tiny path changes, integrating to find the total linear length of a curved profile.

---

How would you like to use this curriculum? We can focus on Day 1 to flesh out individual proofs, or look at how Day 7's eigen-environments tie back into your statistical variance matrices!