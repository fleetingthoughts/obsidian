---
parent: "[[_Fleeting]]"
tags:
  - "#fleeting"
date_created: 2026-05-31
---

Here is the second set of interleaved cumulative quizzes for Days 5 through 7, matching the standard, mathematically rigorous presentation.

---

## 📅 Day 5 Quiz

## Section A: Application & Computation

- Question 5.1: Let $W_1$ and $W_2$ be finite-dimensional subspaces of a vector space $V$. Prove that the sum set $W_1 + W_2 = \{ w_1 + w_2 : w_1 \in W_1 \text{ and } w_2 \in W_2 \}$ is a subspace of $V$.
- Question 5.2: Let $\{x_n\}$ be a sequence defined recursively by $x_1 = 3$ and $x_{n+1} = \frac{1}{2}(x_n + \frac{5}{x_n})$ for $n \ge 1$. Given that this sequence converges to a positive limit $L$, determine the exact value of $L$.
- Question 5.3: Let $X$ and $Y$ have a continuous joint distribution with density function $f(x, y) = e^{-(x+y)}$ for $x > 0$ and $y > 0$ (and $0$ elsewhere). Calculate the conditional expectation $E[Y \mid X = x]$.
- Question 5.4: Evaluate the definite integral $\int_{0}^{\pi} x \sin(x) \, dx$ using the method of integration by parts.

## Section B: Core Factual Recall

- Question 5.5: Define what it means for a subset of a vector space to be linearly independent.
- Question 5.6: State the conditions under which a point $c$ is an inflection point of a continuous function.
- Question 5.7: State the mathematical formula for the binomial coefficient $\binom{n}{k}$.
- Question 5.8: State the definition of an open cover of a set of real numbers.
- Question 5.9: What is an elementary matrix?
- Question 5.10: State the First Fundamental Theorem of Calculus regarding functional differentiation of an integral.
- Question 5.11: Define the standard error of a statistic.
- Question 5.12: State the definition of absolute convergence for an infinite series.
- Question 5.13: State the chain rule for a function composition $f(g(x))$.
- Question 5.14: State the sequential definition of a closed set.

---

## 📅 Day 6 Quiz

## Section A: Application & Computation

- Question 6.1: Let $T: \mathbb{R}^2 \to \mathbb{R}^2$ be a linear transformation whose matrix representation with respect to the standard basis is given by $A = \begin{pmatrix} 0 & -1 \\ 1 & 0 \end{pmatrix}$. Show that $T$ has no real eigenvalues.
- Question 6.2: Let $f(x) = \frac{x}{x^2 + 1}$ be defined on $\mathbb{R}$. Locate all absolute extrema of $f$ by computing its first derivative and analyzing the boundary behavior as $x \to \pm\infty$.
- Question 6.3: Let $X_1, X_2, \dots, X_n$ be independent, identically distributed random variables from a distribution with variance $\sigma^2$. Prove from the variance properties that the variance of the sample mean satisfies $\text{Var}(\bar{X}) = \frac{\sigma^2}{n}$.
- Question 6.4: Prove that if $K_1$ and $K_2$ are compact subsets of $\mathbb{R}$, then their union $K_1 \cup K_2$ is also compact under the open-cover definition.

## Section B: Core Factual Recall

- Question 6.5: Define the rank of a matrix.
- Question 6.6: Define what it means for a function $f$ to be differentiable over an open interval $(a, b)$.
- Question 6.7: State the variance of a discrete Poisson random variable with parameter $\lambda$.
- Question 6.8: State the definition of a Cauchy sequence.
- Question 6.9: Define the coordinate vector of a vector $v$ relative to an ordered basis $\beta$.
- Question 6.10: State the Second Fundamental Theorem of Calculus regarding evaluation of a definite integral.
- Question 6.11: What is the definition of a standard normal distribution's probability density function?
- Question 6.12: Define the interior of a subset $A \subseteq \mathbb{R}$.
- Question 6.13: Define a local minimum of a function.
- Question 6.14: State the definition of a closed cover of a set.

---

## 📅 Day 7 Quiz

## Section A: Application & Computation

- Question 7.1: Let $A = \begin{pmatrix} 1 & 2 \\ 2 & 1 \end{pmatrix}$. Calculate the distinct eigenvalues of $A$ and determine a corresponding eigenvector for each.
- Question 7.2: Let $f(x) = x^2$ for $x \in [0, 1]$. Use the Mean Value Theorem to find the exact point $c \in (0, 1)$ such that the derivative $f'(c)$ matches the average rate of change over the entire interval.
- Question 7.3: Let $X$ follow a continuous uniform distribution over the interval $(0, \theta)$. Calculate the expected value $E[X^2]$ in terms of $\theta$.
- Question 7.4: Let $A$ and $B$ be subsets of $\mathbb{R}$ defined by $A = \{x \in \mathbb{R} : \vert{}x - 2\vert{} < 1\}$ and $B = \{x \in \mathbb{R} : \vert{}x - 4\vert{} \le 2\}$. Explicitly determine the sets $A \cap B$ and $B \setminus A$.

## Section B: Core Factual Recall

- Question 7.5: Define what it means for an $n \times n$ matrix to be diagonalizable.
- Question 7.6: State the Intermediate Value Theorem.
- Question 7.7: Define the covariance of two random variables $X$ and $Y$.
- Question 7.8: State the Monotone Convergence Theorem for sequences.
- Question 7.9: Define a homogeneous linear transformation.
- Question 7.10: State Rolle's Theorem.
- Question 7.11: Define the conditional distribution function of a continuous random variable $Y$ given $X = x$.
- Question 7.12: What does it mean for a set to be perfect?
- Question 7.13: State the second derivative test for finding local extrema.
- Question 7.14: Define the boundary of a set $A \subseteq \mathbb{R}$.

---

---

## 🔑 Comprehensive Answer Key

## Day 5 Solutions

- Solution 5.1: Proved. (i) Since $\mathbf{0} \in W_1$ and $\mathbf{0} \in W_2$, $\mathbf{0} + \mathbf{0} = \mathbf{0} \in W_1 + W_2$. (ii) Let $x, y \in W_1 + W_2$. Then $x = u_1 + u_2$ and $y = v_1 + v_2$ for $u_1, v_1 \in W_1$ and $u_2, v_2 \in W_2$. Then $x + y = (u_1 + v_1) + (u_2 + v_2)$. Since $W_1, W_2$ are subspaces, $u_1 + v_1 \in W_1$ and $u_2 + v_2 \in W_2$, so $x + y \in W_1 + W_2$. (iii) Similarly, for any scalar $c$, $cx = c(u_1 + u_2) = cu_1 + cu_2$. Since $cu_1 \in W_1$ and $cu_2 \in W_2$, $cx \in W_1 + W_2$.
- Solution 5.2: Taking the limit on both sides of the recurrence relation yields $L = \frac{1}{2}(L + \frac{5}{L}) \implies 2L = L + \frac{5}{L} \implies L = \frac{5}{L} \implies L^2 = 5$. Since the limit must be positive, $L = \sqrt{5}$.
- Solution 5.3: The joint distribution factors as $f(x, y) = e^{-x} \cdot e^{-y} = f_X(x)f_Y(y)$, meaning $X$ and $Y$ are independent standard exponential random variables. Therefore, the conditional distribution of $Y$ given $X$ is equal to its marginal distribution: $f_{Y \mid X}(y \mid x) = e^{-y}$. The expectation is $E[Y \mid X = x] = \int_{0}^{\infty} y e^{-y} \, dy = 1$.
- Solution 5.4: Let $u = x$, meaning $du = dx$. Let $dv = \sin(x)dx$, meaning $v = -\cos(x)$. Applying integration by parts gives $[-x \cos(x)]_{0}^{\pi} - \int_{0}^{\pi} (-\cos(x)) \, dx = [-\pi(-1) - 0] + [\sin(x)]_{0}^{\pi} = \pi + 0 = \pi$.
- Solution 5.5: A set of vectors $S$ such that the only linear combination summing to the zero vector is the trivial one where all scalar coefficients equal zero.
- Solution 5.6: A point $c$ where the function is continuous and the direction of concavity changes (changes from upward to downward or downward to upward).
- Solution 5.7: $\binom{n}{k} = \frac{n!}{k!(n-k)!}$.
- Solution 5.8: A collection of open sets whose union completely contains the target set.
- Solution 5.9: A square matrix obtained by performing exactly one elementary row operation on the identity matrix.
- Solution 5.10: $\frac{d}{dx} \left[ \int_{a}^{x} f(t) \, dt \right] = f(x)$.
- Solution 5.11: The standard deviation of the sampling distribution of a given estimator or statistic.
- Solution 5.12: An infinite series $\sum a_n$ converges absolutely if the matching series of absolute values $\sum \vert{}a_n\vert{}$ converges to a finite real value.
- Solution 5.13: $(f \circ g)'(x) = f'(g(x)) \cdot g'(x)$.
- Solution 5.14: A set $F \subseteq \mathbb{R}$ is closed if, whenever a sequence $\{x_n\}$ contained in $F$ converges to a limit $L$, that limit $L$ is also an element of $F$.

## Day 6 Solutions

- Solution 6.1: The characteristic polynomial is $\det(A - \lambda I) = \det\begin{pmatrix} -\lambda & -1 \\ 1 & -\lambda \end{pmatrix} = \lambda^2 - (-1) = \lambda^2 + 1$. Setting $\lambda^2 + 1 = 0 \implies \lambda^2 = -1$, which has zero real solutions. Thus, $T$ has no real eigenvalues.
- Solution 6.2: The first derivative is $f'(x) = \frac{1(x^2 + 1) - x(2x)}{(x^2 + 1)^2} = \frac{1 - x^2}{(x^2 + 1)^2}$. Setting $f'(x) = 0 \implies x = \pm 1$. Evaluating at these points gives $f(1) = \frac{1}{2}$ and $f(-1) = -\frac{1}{2}$. Since $\lim_{x \to \infty} f(x) = 0$ and $\lim_{x \to -\infty} f(x) = 0$, the absolute maximum is $\frac{1}{2}$ at $x = 1$ and the absolute minimum is $-\frac{1}{2}$ at $x = -1$.
- Solution 6.3: Proved. By definition, $\bar{X} = \frac{1}{n}\sum_{i=1}^n X_i$. Pulling out the scalar factor maps as $\text{Var}(\bar{X}) = \frac{1}{n^2} \text{Var}\left(\sum_{i=1}^n X_i\right)$. Since the random variables are mutually independent, the variance of their sum equals the sum of their individual variances: $\frac{1}{n^2} \sum_{i=1}^n \text{Var}(X_i) = \frac{1}{n^2} (n \sigma^2) = \frac{\sigma^2}{n}$.
- Solution 6.4: Proved. Let $\mathcal{O}$ be an open cover for $K_1 \cup K_2$. Since $K_1 \subseteq K_1 \cup K_2$, $\mathcal{O}$ is also an open cover for $K_1$. By compactness of $K_1$, there exists a finite subcover $\mathcal{O}_1 \subseteq \mathcal{O}$ that covers $K_1$. Similarly, there exists a finite subcover $\mathcal{O}_2 \subseteq \mathcal{O}$ that covers $K_2$. The combined collection $\mathcal{O}_1 \cup \mathcal{O}_2$ is a finite subcollection of $\mathcal{O}$ that completely covers $K_1 \cup K_2$.
- Solution 6.5: The maximum number of linearly independent rows (or columns) in a matrix.
- Solution 6.6: A function is differentiable over an interval if the derivative limit exists at every individual point within that open domain.
- Solution 6.7: For a Poisson distribution, the variance is exactly equal to its rate parameter, $\lambda$.
- Solution 6.8: A sequence where for every $\epsilon > 0$, there exists a threshold $N \in \mathbb{N}$ such that $m, n \ge N \implies \vert{}x_m - x_n\vert{} < \epsilon$.
- Solution 6.9: The column vector of unique scalar coefficients needed to express $v$ as a linear combination of the ordered basis vectors in $\beta$.
- Solution 6.10: If $f$ is continuous on $[a,b]$ and $F$ is an antiderivative of $f$ ($F' = f$), then $\int_{a}^{b} f(x) \, dx = F(b) - F(a)$.
- Solution 6.11: $f(x) = \frac{1}{\sqrt{2\pi}} e^{-x^2/2}$ for all real $x$.
- Solution 6.12: The collection of all interior points of $A$, where an interior point is a point that possesses an open neighborhood entirely contained within $A$.
- Solution 6.13: A point $c$ where there exists an open neighborhood $V$ around $c$ such that $f(c) \le f(x)$ for all $x \in V$.
- Solution 6.14: A collection of closed sets whose union completely contains the target set.

## Day 7 Solutions

- Solution 7.1: The characteristic equation is $\det(A - \lambda I) = (1-\lambda)^2 - 4 = \lambda^2 - 2\lambda - 3 = (\lambda - 3)(\lambda + 1) = 0$, giving $\lambda = 3, -1$. For $\lambda = 3$, solving $(A - 3I)\mathbf{x} = \mathbf{0} \implies \begin{pmatrix} -2 & 2 \\ 2 & -2 \end{pmatrix} \mathbf{x} = \mathbf{0}$ yields the eigenvector $\begin{pmatrix} 1 \\ 1 \end{pmatrix}$. For $\lambda = -1$, solving $(A + I)\mathbf{x} = \mathbf{0} \implies \begin{pmatrix} 2 & 2 \\ 2 & 2 \end{pmatrix} \mathbf{x} = \mathbf{0}$ yields the eigenvector $\begin{pmatrix} 1 \\ -1 \end{pmatrix}$.
- Solution 7.2: The average rate of change over $[0, 1]$ is $\frac{f(1) - f(0)}{1 - 0} = \frac{1 - 0}{1} = 1$. The derivative is $f'(x) = 2x$. By the Mean Value Theorem, we set $2c = 1 \implies c = \frac{1}{2}$, which lies safely in $(0, 1)$.
- Solution 7.3: The density function is $f(x) = \frac{1}{\theta}$ for $0 < x < \theta$. The expected value is $E[X^2] = \int_{0}^{\theta} x^2 \left(\frac{1}{\theta}\right) \, dx = \frac{1}{\theta} \left[ \frac{x^3}{3} \right]_{0}^{\theta} = \frac{\theta^3}{3\theta} = \frac{\theta^2}{3}$.
- Solution 7.4: Solving the inequalities yields intervals: $A = (1, 3)$ and $B = [2, 6]$. Therefore, the intersection is $A \cap B = [2, 3)$. The set difference represents everything in $B$ that is not in $A$, which leaves $B \setminus A = [3, 6]$.
- Solution 7.5: A square matrix $A$ is diagonalizable if there exists an invertible matrix $P$ and a diagonal matrix $D$ such that $P^{-1}AP = D$.
- Solution 7.6: If $f$ is continuous on a closed interval $[a, b]$, then for any value $u$ strictly between $f(a)$ and $f(b)$, there exists at least one point $c \in (a, b)$ such that $f(c) = u$.
- Solution 7.7: $\text{Cov}(X, Y) = E[(X - E[X])(Y - E[Y])] = E[XY] - E[X]E[Y]$.
- Solution 7.8: Every sequence of real numbers that is monotonic and bounded is guaranteed to converge to a finite real limit.
- Solution 7.10: A transformation $T$ that maps a vector space $V$ into itself and satisfies properties of additivity and scalar homogeneity.
- Solution 7.10: If $f$ is continuous on $[a,b]$, differentiable on $(a,b)$, and $f(a) = f(b)$, then there exists a point $c \in (a,b)$ such that $f'(c) = 0$.
- Solution 7.11: $f_{Y \mid X}(y \mid x) = \frac{f(x, y)}{f_X(x)}$ for all values where $f_X(x) > 0$.
- Solution 7.12: A set of real numbers that is closed and contains no isolated points (every point is a limit point).
- Solution 7.13: If $f'(c) = 0$ and $f''(c) > 0$, $c$ is a local minimum; if $f'(c) = 0$ and $f''(c) < 0$, $c$ is a local maximum.
- Solution 7.14: The set of points belonging to the closure of $A$ that do not belong to the interior of $A$.

---

## 📈 Blueprint Reference Map (For Review Tracking)

- Linear Transforms & Matrices: Evaluated via sum space closures, characteristic eigenvalue matrix solutions, and basis structures.
- Continuums & Analysis Limits: Checked using recursive real sequence convergence, compact set topological union mechanics, and interval configurations.
- Calculus Operational Toolkits: Computed by tracking absolute extrema optimization, integration by parts execution, and Mean Value derivative equations.
- Probability Distributions: Dissected using conditional expected values, continuous uniform sample statistics, and variance independent expansions.

---

This completes your tailored interleaved prep plan. Let me know if you would like to adjust the structure or focus on a particular proof drill to target your study session.