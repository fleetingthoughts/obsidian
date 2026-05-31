---
parent: "[[_Fleeting]]"
tags:
  - "#fleeting"
date_created: "2026-05-31"
---

Here are the corrected, cleaned-up versions of the quizzes for Days 5 through 7 (INDEX). Section B (Core Factual Recall) has been shortened by removing two non-core questions from each day, while keeping the rest of the layout, plain-text math notation, and strict chapter constraints.

---

## 📅 Day 5 Quiz

## Section A: Application & Computation

- Question 5.1: Let $(\mathcal{C}, \mathcal{B}, P)$ be a probability space, and let $C_1, C_2, \dots, C_k$ be arbitrary events in $\mathcal{B}$. State Boole's Inequality, and prove it for the finite case ($n = k$) using induction and basic probability set properties.
- Question 5.2: Let $\beta = \{(1,1), (1,0)\}$ and $\gamma = \{(1,2), (0,1)\}$ be two alternative bases for $\mathbb{R}^2$. Let $T: \mathbb{R}^2 \to \mathbb{R}^2$ be the identity operator $T(v) = v$. Compute the change-of-basis coordinate matrix $[T]_\beta^\gamma$.
- Question 5.3: Define what it means for a subset $K \subseteq \mathbb{R}$ to be compact using the sequential definition. Use this definition to prove that the open interval $(0, 1)$ is not compact.
- Question 5.4: Evaluate the following definite integral using the method of integration by parts: the integral from $1$ to $e$ of $x \ln(x) \, dx$.

## Section B: Core Factual Recall

- Question 5.5: State the definition of a linear transformation from a vector space $V$ to a vector space $W$.
- Question 5.6: Define a critical point (or stationary point) of a differentiable function.
- Question 5.7: State the condition required for two events to be considered statistically independent.
- Question 5.8: What is the definition of a Cauchy sequence?
- Question 5.9: State the dimension theorem (Rank-Nullity Theorem) for linear transformations.
- Question 5.10: What is the general formula for integration by parts?
- Question 5.11: Define the covariance of two random variables $X$ and $Y$.
- Question 5.12: What is the definition of the sum of an infinite series?
- Question 5.13: State the rule for differentiating a composite function (the Chain Rule).
- Question 5.14: Define a limit point (or accumulation point) of a set.

---

## 📅 Day 6 Quiz

## Section A: Application & Computation

- Question 6.1: Let $X_1, X_2, \dots, X_n$ be a random sample drawn from a Normal distribution $N(\mu, \sigma^2)$. State Student's Theorem regarding the relationship between the sample mean $\bar{X}$ and the sample variance $S^2$. What deep algebraic structural relationship does this imply?
- Question 6.2: Let $f$ be a function defined on $[a, b]$ that is differentiable on $(a, b)$. Suppose $f'(x) \le 0$ for all $x$ in $(a, b)$. Prove directly (using the Mean Value Theorem) that $f$ is a non-increasing function on $[a, b]$.
- Question 6.3: Let $A$ be a square matrix. Define what it means for $A$ to be invertible. State the relationship between the invertibility of $A$, the determinant of $A$, and the rank of $A$.
- Question 6.4: Prove that if a sequence of real numbers converges to a limit $L$, then every subsequence must also converge to $L$.

## Section B: Core Factual Recall

- Question 6.5: Define similar matrices.
- Question 6.6: What is the definition of an inflection point of a continuous function?
- Question 6.7: State the property that relates independent random variables to their joint probability mass or density function.
- Question 6.8: State the definition of the correlation coefficient between two random variables.
- Question 6.9: What are the structural requirements for a subset to be a subspace of a vector space?
- Question 6.10: State the Fundamental Theorem of Calculus regarding evaluation of a definite integral.
- Question 6.11: Define a standard normal random variable.
- Question 6.12: What is the definition of absolute convergence for an infinite series?
- Question 6.13: Define a relative maximum of a function.
- Question 6.14: Define the closure of a set.

---

## 📅 Day 7 Quiz

## Section A: Application & Computation

- Question 7.1: A deck of 52 cards is well-shuffled. A poker hand of 5 cards is dealt out at random without replacement. Compute the exact probability of obtaining a full house (3 cards of one matching rank, and 2 cards of another distinct matching rank). Express your answer both as a combination formula and a final decimal.
- Question 7.2: Let $x_1 = 1$, and for each natural number $n$ define $x_{n+1} = \frac{1}{2}x_n + 1$.
    
    1. Use mathematical induction to rigorously prove that the sequence is increasing; that is, show $x_n \le x_{n+1}$ for all natural numbers.
    2. State whether this sequence is guaranteed to converge, and name the specific theorem that justifies your conclusion.
    
- Question 7.3: Let $A = \begin{pmatrix} 1 & k \\ 4 & 1 \end{pmatrix}$. Find all values of the constant $k$ for which the system of linear equations $A\mathbf{x} = \mathbf{0}$ has non-trivial solutions.
- Question 7.4: Let $X$ be a random variable with probability density function $f(x) = \frac{1}{2} e^{-\vert{}x\vert{}}$ for $-\infty < x < \infty$. Compute the mathematical expectation $E[X^2]$.

## Section B: Core Factual Recall

- Question 7.5: Define the characteristic polynomial of a square matrix.
- Question 7.6: State the Intermediate Value Theorem for continuous functions.
- Question 7.7: What is a binomial distribution's probability mass function?
- Question 7.8: Define a countable set.
- Question 7.9: Define an eigenvalue and an eigenvector of a linear operator.
- Question 7.10: State the Mean Value Theorem for integrals.
- Question 7.11: What is a conditional probability density function?
- Question 7.12: State the definition of conditional convergence for an infinite series.
- Question 7.13: State the second derivative test for local extrema.
- Question 7.14: Define a perfect set of real numbers.

---

---

## 🔑 Comprehensive Answer Key

## Day 5 Solutions

- Solution 5.1: Proved. Boole's inequality states $P(\bigcup A_i) \le \sum P(A_i)$. Base case ($n = 2$): $P(C_1 \cup C_2) = P(C_1) + P(C_2) - P(C_1 \cap C_2)$. Since $P(C_1 \cap C_2) \ge 0$, it follows directly that $P(C_1 \cup C_2) \le P(C_1) + P(C_2)$. Assume true for $n = k$. For $n = k + 1$: $P(\bigcup_{i=1}^{k+1} C_i) = P((\bigcup_{i=1}^{k} C_i) \cup C_{k+1}) \le P(\bigcup_{i=1}^{k} C_i) + P(C_{k+1})$. Applying the induction step: $\le \sum_{i=1}^{k} P(C_i) + P(C_{k+1}) = \sum_{i=1}^{k+1} P(C_i)$.
- Solution 5.2: The change-of-basis matrix is $\begin{pmatrix} 1 & 1 \\ -1 & -2 \end{pmatrix}$. Vector $\beta_1 = (1, 1) = 1(1, 2) - 1(0, 1)$, which gives the first column. Vector $\beta_2 = (1, 0) = 1(1, 2) - 2(0, 1)$, which gives the second column.
- Solution 5.3: Proved. A set $K$ is sequentially compact if every sequence contained within $K$ has a subsequence that converges to a limit that is also contained within $K$. Consider the sequence $x_n = \frac{1}{n+1}$ inside the set $(0, 1)$. Every subsequence of $x_n$ converges uniquely to $0$. Since $0 \notin (0, 1)$, the convergent limit point escapes the domain boundaries, proving $(0, 1)$ is not compact.
- Solution 5.4: The exact value of the integral is $\frac{e^2 + 1}{4}$. Let $u = \ln(x)$, meaning $du = \frac{1}{x} \, dx$. Let $dv = x \, dx$, meaning $v = \frac{x^2}{2}$. The integration by parts formula gives $[ \frac{x^2}{2} \ln(x) ] - \int \frac{x}{2} \, dx$, which evaluates to $[ \frac{x^2}{2} \ln(x) ] - \frac{x^2}{4}$. Evaluating this expression from $1$ to $e$ yields $[ \frac{e^2}{2} - \frac{e^2}{4} ] - [ 0 - \frac{1}{4} ]$, simplifying directly to $\frac{e^2 + 1}{4}$.
- Solution 5.5: A function $T: V \to W$ such that $T(u+v) = T(u) + T(v)$ and $T(cu) = cT(u)$ for all vectors $u,v$ and scalars $c$.
- Solution 5.6: A point $x$ in the domain of a function where the derivative is zero or is undefined.
- Solution 5.7: Two events $A$ and $B$ such that $P(A \cap B) = P(A)P(B)$.
- Solution 5.8: A sequence where for every $\epsilon > 0$, there exists an index $N$ such that for all $m, n \ge N$, $\vert{}x_m - x_n\vert{} < \epsilon$.
- Solution 5.9: $\dim(\text{Null Space } T) + \dim(\text{Range } T) = \dim(V)$.
- Solution 5.10: $\int u \, dv = uv - \int v \, du$.
- Solution 5.11: $\text{Cov}(X,Y) = E[(X - E[X])(Y - E[Y])] = E[XY] - E[X]E[Y]$.
- Solution 5.12: The limit of the sequence of partial sums, provided that this limit exists.
- Solution 5.13: $(f \circ g)'(x) = f'(g(x)) \cdot g'(x)$.
- Solution 5.14: A point $x$ where every open neighborhood contains at least one point of the set other than $x$ itself.

## Day 6 Solutions

- Solution 6.1: Student's Theorem states that the sample mean $\bar{X}$ and sample variance $S^2$ are statistically independent, and $\frac{(n-1)S^2}{\sigma^2} \sim \chi^2(n-1)$. Algebraically, this implies that the sample variance projection vector acts completely perpendicular to the subspace baseline vector of the mean.
- Solution 6.2: Proved. Let $x, y \in [a, b]$ with $x < y$. By the Mean Value Theorem applied to $f$ on $[x, y]$, there exists some $c \in (x, y)$ such that $f(y) - f(x) = f'(c)(y - x)$. We are given that $f'(x) \le 0$ everywhere, so $f'(c) \le 0$. Since $x < y \implies y - x > 0$, the product $f'(c)(y - x) \le 0$. Therefore, $f(y) - f(x) \le 0 \implies f(y) \le f(x)$, proving $f$ is non-increasing.
- Solution 6.3: $A$ is invertible if there exists a matrix $A^{-1}$ such that $A A^{-1} = A^{-1} A = I$. Relationship: $A$ is invertible if and only if $\det(A) \neq 0$, which is true if and only if $\text{rank}(A) = n$ (full rank).
- Solution 6.4: Proved. Convergence means that for every $\epsilon > 0$, there exists an index $N$ such that $n \ge N \implies \vert{}x_n - L\vert{} < \epsilon$. A subsequence index sequence satisfies $n_k \ge k$ for all $k$. Therefore, if we look at indices where $k \ge N$, we are guaranteed that $n_k \ge k \ge N$, which triggers the convergence requirement: $\vert{}x_{n_k} - L\vert{} < \epsilon$.
- Solution 6.5: Two matrices $A$ and $B$ such that there exists an invertible matrix $P$ satisfying $B = P^{-1}AP$.
- Solution 6.6: A point on a curve where the concavity changes from upward to downward, or vice versa.
- Solution 6.7: Their joint function factors perfectly into the product of their individual marginal functions: $f(x,y) = f_X(x)f_Y(y)$.
- Solution 6.8: $\rho = \frac{\text{Cov}(X,Y)}{\sigma_X \sigma_Y}$.
- Solution 6.9: The subset must contain the zero vector, be closed under vector addition, and be closed under scalar multiplication.
- Solution 6.10: If $F'(x) = f(x)$, then $\int_{a}^{b} f(x) \, dx = F(b) - F(a)$.
- Solution 6.11: A continuous random variable following a normal distribution with a mean of $0$ and a variance of $1$.
- Solution 6.12: An infinite series converges absolutely if the series of absolute values $\sum \vert{}a_n\vert{}$ converges.
- Solution 6.13: A point $c$ where there exists a neighborhood around $c$ such that $f(c) \ge f(x)$ for all $x$ in that neighborhood.
- Solution 6.14: The union of a set with all of its limit points.

## Day 7 Solutions

- Solution 7.1: Total hands = $\binom{52}{5} = 2,598,960$. Formula: $\frac{\binom{13}{1}\binom{4}{3} \cdot \binom{12}{1}\binom{4}{2}}{\binom{52}{5}} = \frac{13 \cdot 4 \cdot 12 \cdot 6}{2598960} = \frac{3744}{2598960} \approx \mathbf{0.00144}$ (or about $0.14\%$).
- Solution 7.2:
    
    1. Induction Proof: For $n = 1$, $x_1 = 1$ and $x_2 = \frac{1}{2}(1) + 1 = 1.5$. Since $1 \le 1.5$, the base case holds. Assume $x_k \le x_{k+1}$ is true. Multiplying across this assumption by $\frac{1}{2}$ gives $\frac{1}{2}x_k \le \frac{1}{2}x_{k+1}$. Adding $1$ to both sides yields $\frac{1}{2}x_k + 1 \le \frac{1}{2}x_{k+1} + 1 \implies x_{k+1} \le x_{k+2}$, completing the inductive step.
    2. The sequence is guaranteed to converge by the Monotone Convergence Theorem. Because it is monotonic (increasing) and bounded above (it never reaches $2$), this theorem dictates that it must possess a finite limit.
    
- Solution 7.3: Non-trivial solutions exist if and only if $\det(A) = 0$. $\det(A) = 1(1) - 4(k) = 1 - 4k$. Setting $1 - 4k = 0 \implies \mathbf{k = \frac{1}{4}}$.
- Solution 7.4: $E[X^2] = \mathbf{2}$. Computed via symmetry expansion: $\int_{-\infty}^{\infty} x^2 \left(\frac{1}{2}e^{-\vert{}x\vert{}}\right)dx = \int_{0}^{\infty} x^2 e^{-x}dx$. This evaluates directly using the standard Gamma identity $\Gamma(3) = 2! = 2$.
- Solution 7.5: The polynomial defined by $p(\lambda) = \det(A - \lambda I)$.
- Solution 7.6: If $f$ is continuous on $[a, b]$, then for any value $u$ between $f(a)$ and $f(b)$, there exists a point $c \in (a, b)$ such that $f(c) = u$.
- Solution 7.7: $p(x) = \binom{n}{x} p^x (1-p)^{n-x}$ for $x = 0, 1, \dots, n$.
- Solution 7.8: A set that can be placed in a one-to-one correspondence with the set of natural numbers $\mathbb{N}$.
- Solution 7.9: A scalar $\lambda$ and a non-zero vector $v$ such that $T(v) = \lambda v$.
- Solution 7.10: If $f$ is continuous on $[a, b]$, there exists a point $c \in (a, b)$ such that $\int_{a}^{b} f(x) \, dx = f(c)(b - a)$.
- Solution 7.11: $f_{Y\vert{}X}(y\vert{}x) = \frac{f(x,y)}{f_X(x)}$, provided that $f_X(x) > 0$.
- Solution 7.12: An infinite series converges conditionally if the series $\sum a_n$ converges, but the series of absolute values $\sum \vert{}a_n\vert{}$ diverges.
- Solution 7.13: If $f'(c) = 0$ and $f''(c) < 0$, then $c$ is a local maximum; if $f'(c) = 0$ and $f''(c) > 0$, then $c$ is a local minimum.
- Solution 7.14: A set that is closed and contains no isolated points (meaning every point in the set is a limit point of the set).

---

## 📈 Blueprint Reference Map (For Review Tracking)

- Linear Transforms & Matrices: Checked by vector closure tests, null space checks, change of basis matrices, and determinant boundaries.
- Continuums & Analysis Limits: Evaluated via completeness properties, sequence subsequence tracking, topological compactness bounds, and monotone convergence parameters.
- Calculus Operational Toolkits: Computed by tracking extrema values, fundamental integrals, integration by parts, and boundary derivatives.
- Probability Distributions: Dissected using variable transformations, expectation series, combinatoric conditions, and independence rules.

---

Propose a target tracking goal to continue your study:

- Request a mock exam layout strictly validating change-of-basis mechanics.
- Focus on a targeted definition drill comparing connectedness versus compactness.
- Propose text-specific practice tracking for a new chapter selection.







