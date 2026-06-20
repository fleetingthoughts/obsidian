## 📅 Day 1

- Question 1: Let $A \subset \mathbb{R}$ be a nonempty set that is bounded above, and let $c < 0$. Define the scaled set $cA = \{ca : a \in A\}$. Formulate a precise structural conjecture for $\sup(cA)$ in terms of $\inf A$, and provide a rigorous proof using the $\epsilon$-characterization of bounds.
- Question 2: Prove the Cauchy-Schwarz inequality for real scalars ($AC \geq B^2$) using the non-negativity of a quadratic polynomial in a real tracking variable $t$: $f(t) = \sum_{i=1}^n (a_i + b_i t)^2 \geq 0$. Explain the geometric interpretation when $n=2$.
- Question 3: Let $\mathcal{C}$ be a sample space and let $\{C_n\}_{n=1}^\infty$ be a nonincreasing (nested downward) sequence of random events. Prove the decreasing case of the Continuity Theorem of Probability:  
    $$\lim_{n \to \infty} P(C_n) = P\left(\bigcap_{n=1}^\infty C_n\right)$$  
    Do not assume the increasing case; build your proof directly by constructing disjoint telescoping rings.
- Question 4: Write down the definition of an Ordered Field and state the Axiom of Completeness explicitly.
- Question 5: State the formal definition of a Rational Number and outline why its algebraic structure forms a Field while the integers ($\mathbb{Z}$) do not.
- Question 6: Define what it means for a subset of $\mathbb{R}$ to be Bounded Below and write the formal definition of an Infimum.
- Question 7: State the three conditions that a real-valued function must satisfy to be defined as a Probability Set Function.
- Question 8: Define a Random Experiment and explain the formal structural difference between a Sample Space and an Event.
- Question 9: State Bonferroni’s Inequality for two arbitrary random events. Under what restriction regarding their individual probabilities does it provide a meaningful bound?

---

## 📅 Day 2

- Question 1: Assume $a_n \to a$ and $b_n \to b$ as $n \to \infty$. Prove the algebraic product limit rule ($a_n b_n \to ab$) using the triangular add-and-subtract technique to isolate the parameter variations. Explicitly show how the boundedness of a convergent sequence is required to establish your final epsilon control.
- Question 2: Define the natural logarithm function strictly as an integral accumulation framework: $\log x = \int_1^x \frac{1}{t}dt$ for $x > 0$. Prove the addition theorem $\log(xy) = \log x + \log y$ using an explicit coordinate substitution strategy within the integral.
- Question 3: Let $X$ be a continuous random variable with a strictly increasing Cumulative Distribution Function $F(x)$. Define $Y = F(X)$. Prove that $Y$ distributes uniformly over the continuous interval $(0, 1)$. This represents the foundational engine for inverse transform sampling.
- Question 4: Define a Relative Frequency and state the three exact axioms of a Probability Set Function.
- Question 5: Write down the formal definition of the Convergence of a Sequence using an index cut-off threshold $N$.
- Question 6: Define a Monotone Sequence and distinguish between a non-decreasing sequence and a strictly increasing sequence.
- Question 7: State the Order Limit Theorem for sequences. If $a_n \geq 0$ for all $n$ and $a_n \to a$, what must be true of $a$?
- Question 8: State the formal definition of an Unbiased Estimator in sampling theory.
- Question 9: Define the Sample Mean ($\bar{X}$) and write out its expected value and variance in terms of the population parameters $\mu$ and $\sigma^2$.

---

## 📅 Day 3

- Question 1: Prove the forward direction of the Cauchy Criterion for sequences: if a sequence converges, it must be a Cauchy sequence. Then, write out the contrapositive negation of the Cauchy convergence criterion into a positive mathematical statement that avoids using the word "not."
- Question 2: Evaluate the dynamic growth and order of magnitude behaviors ("O" and "o" notation) between exponential scales ($e^x$) and polynomial configurations ($x^n$) as $x \to \infty$. Use an analytical tracking mechanism to justify which family dominates the continuum.
- Question 3: Prove Markov's Inequality for a non-negative random variable $u(X)$ and a static macro threshold $c > 0$:  
    $$P(u(X) \geq c) \leq \frac{E[u(X)]}{c}$$  
    Show exactly how splitting the integral/sum at the operational cutoff boundaries yields this global control framework.
- Question 4: State the formal definition of a Moment Generating Function ($M(t)$) and explain its mathematical utility in statistics.
- Question 5: State the unique definition of a Cauchy Sequence without referencing its limit value.
- Question 6: State the Monotone Convergence Theorem (MCT) for sequences. What two baseline criteria guarantee convergence?
- Question 7: State Chebyshev's Inequality explicitly. How is it derived directly from Markov's Inequality?
- Question 8: Define the Sample Variance ($S^2$) and explain the mathematical purpose of using $n-1$ as the denominator instead of $n$.
- Question 9: State the formal algebraic relationship between a random variable's variance, its second raw moment ($E[X^2]$), and its first central moment ($E[X]$).

---

## 📅 Day 4

- Question 1: Prove that a set $F \subset \mathbb{R}$ is topologically closed if and only if every convergent sequence contained entirely within $F$ has its tracking target limit within $F$ as well.
- Question 2: A particle moves along a plane curve parametrized dynamically by $x = \cos^3 t$ and $y = \sin^3 t$ for $t \in [0, \pi/2]$. Derive the geometric arc length of this path using infinitesimal string component integration, and verify that the parametric tangent at any point matches your kinematic intuition.
- Question 3: Let $X_1$ and $X_2$ have a joint probability density function $f_{X_1, X_2}(x_1, x_2)$. Let $Y_1 = X_1 + X_2$ and $Y_2 = X_1 - X_2$. Derivationally unroll the joint density function $f_{Y_1, Y_2}(y_1, y_2)$ by calculating the structural determinant of the Jacobian Matrix for this bivariate transformation.
- Question 4: Define an $\epsilon$-Neighborhood of a point $x_0$ and distinguish between a Limit Point and an Isolated Point.
- Question 5: State the definition of an Open Set in $\mathbb{R}$ and write out the definition of the Closure of a set.
- Question 6: Define what it means for an infinite collection of open sets to form an Open Cover for a target set.
- Question 7: State De Morgan’s Laws for two sets and outline the proof strategy for showing that $(A \cap B)^c = A^c \cup B^c$.
- Question 8: Define the mathematical difference between a Joint Probability Density Function and a Marginal Probability Density Function.
- Question 9: Define the Covariance between two random variables and state its formula in terms of expectations.

---

## 📅 Day 5

- Question 1: Prove the Sequential Criterion for Functional Limits: $\lim_{x \to c} f(x) = L$ if and only if for every sequence $x_n \to c$ (with $x_n \neq c$), it follows that $f(x_n) \to L$.
- Question 2: Formulate the Mean Value Theorem for integrals on a continuous function $f(x)$ across the bounded block $[a, b]$. Geometrically demonstrate how this theorem guarantees the existence of a true rectangular height that matches the total accumulated area under the curve.
- Question 3: Let $X_1, \dots, X_n$ be a random sample from a distribution with mean $\mu$ and variance $\sigma^2$. Prove that the sample variance estimator $S^2 = \frac{1}{n-1}\sum_{i=1}^n (X_i - \bar{X})^2$ is an unbiased estimator for $\sigma^2$. Explicitly detail why the degrees of freedom correction factor ($n-1$) cancels out the structural covariance bias introduced by subtracting the sample mean $\bar{X}$.
- Question 4: State the crisp definition of a Statistic and define what makes an estimator Unbiased.
- Question 5: Write down the rigorous mathematical definition of a Functional Limit using epsilon and delta thresholds.
- Question 6: State what it means for a function $f$ to be Continuous at a Point $c$ using both limit notation and neighborhood windows.
- Question 7: State the definition of a Quantile Function and write its relation to the Cumulative Distribution Function (CDF).
- Question 8: State the Correlation Coefficient ($\rho$) formula and name its absolute geometric boundaries.
- Question 9: State the Mean Value Theorem for Derivatives explicitly.

---

## 📅 Day 6

- Question 1: Provide a rigorous example of a function that is continuous on an open interval $A$ but fails to be uniformly continuous on $A$. Prove the failure of uniform continuity using two tracking sequences whose absolute spatial distance approaches zero while their output separation remains bounded by a static macro epsilon buffer.
- Question 2: Prove that the essential geometric arc length of a continuous parametric plane curve remains completely invariant (unchanged) under a structural rotation of the underlying coordinate system axes.
- Question 3: Let $X_1$ and $X_2$ be two independent continuous random variables. Prove the Conditional Mean Decomposition theorem (the Law of Total Expectation): $E[E[Y\vert{}X]] = E[Y]$. Show the full step-by-step collapse of the nested iterated integrals into a unified spatial joint integral.
- Question 4: Write out the explicit condition for two random variables to be Independent using their joint and marginal PDFs/PMFs.
- Question 5: State the definition of Uniform Continuity on a set and outline how it fundamentally differs from ordinary continuity.
- Question 6: State the definition of an Open Interval versus a Closed Interval. Explain why an infinite intersection of open intervals $\bigcap_{n=1}^{\infty} (-\frac{1}{n}, \frac{1}{n})$ fails to be open.
- Question 7: State the definition of Conditional Expectation $E[Y \vert{} x]$ for continuous random variables.
- Question 8: State the definition of a Variance-Covariance Matrix for an $n$-dimensional random vector.
- Question 9: State the mathematical definition of a Random Sample of size $n$.

---

## 📅 Day 7

- Question 1: Prove that if a function $f: K \to \mathbb{R}$ is continuous and its assigned domain $K \subset \mathbb{R}$ is compact, then the resulting output image field $f(K)$ is also compact. Use sequential compactness (Bolzano-Weierstrass tracking) as your primary proof line.
- Question 2: Set up Thomae’s Function on the interval $(0,1)$ by declaring its unique output behaviors at rational fractions versus irrational points. Prove analytically, using an $\epsilon$-$\delta$ neighborhood framework, that it is continuous at every irrational point but discontinuous at every rational point.
- Question 3: Let $X_1, \dots, X_n$ be an independent, identically distributed sample extracted from a Gaussian field $N(\mu, \sigma^2)$ where $\sigma^2$ is entirely unknown. State the explicit pivot random variable used to build interval estimators for $\mu$, prove its structural distribution, and construct the standard two-sided $(1-\alpha)$ confidence interval equation.
- Question 4: Give the mathematical definitions for a Perfect Set and a Connected Set.
- Question 5: State the Heine-Borel Theorem defining the exact properties required for sets to be sequentially trapped in finite spaces.
- Question 6: State the Extreme Value Theorem (EVT) for continuous functions. What boundary domain constraint is strictly required?
- Question 7: State the Intermediate Value Theorem (IVT) for continuous functions.
- Question 8: State Jensen's Inequality for a convex fwunction $\phi(x)$ operating on a random variable $X$.
- Question 9: Define the Bivariate Normal Distribution parameters and state the exact component that isolates the linear alignment factor between dimensions.

---


## Complete Master Solution Key

---

## 📅 Day 1

- Question 1: Conjecture: $\sup(cA) = c \inf A$.
    
    - _Proof_: Let $l = \inf A$. By definition, $a \geq l \implies ca \leq cl$ (since $c < 0$), so $cl$ is an upper bound for $cA$. Given $\epsilon > 0$, choose $\epsilon' = \epsilon / \vert{}c\vert{} > 0$. Since $l = \inf A$, there exists $a \in A$ such that $a < l + \epsilon'$. Multiplying by $c$ flips the inequality: $ca > c(l + \epsilon') = cl + c(\epsilon / \vert{}c\vert{}) = cl - \epsilon$. By the $\epsilon$-characterization of suprema, $\sup(cA) = cl = c \inf A$.
    
- Question 2: Define $f(t) = \sum_{i=1}^n (a_i + b_i t)^2 = A + 2Bt + Ct^2 \geq 0$ for all $t \in \mathbb{R}$, where $A = \sum a_i^2$, $B = \sum a_i b_i$, and $C = \sum b_i^2$. For this quadratic to be non-negative for all real $t$, its discriminant must be non-positive: $\Delta = (2B)^2 - 4AC \leq 0 \implies 4B^2 \leq 4AC \implies B^2 \leq AC$.
    
    - _Geometric Interpretation ($n=2$)_: The squared dot product of two 2D vectors is less than or equal to the product of their squared Euclidean norms: $[(\mathbf{u} \cdot \mathbf{v})]^2 \leq \Vert{}\mathbf{u}\Vert{}^2 \Vert{}\mathbf{v}\Vert{}^2$, which simplifies to $\cos^2 \theta \leq 1$.
    
- Question 3: Define disjoint telescoping rings $R_1 = C_1^c$ and $R_n = C_n^c \cap C_{n-1}$ for $n > 1$. Since $\{C_n\}$ is nested downward, $\{C_n^c\}$ is an increasing chain nested upward, and $\bigcup_{n=1}^\infty C_n^c = (\bigcap_{n=1}^\infty C_n)^c$. Also, $\bigcup_{n=1}^\infty R_n = \bigcup_{n=1}^\infty C_n^c$ and $P(R_n) = P(C_n^c) - P(C_{n-1}^c) = P(C_{n-1}) - P(C_n)$. By countable additivity:  
    $$P\left(\left(\bigcap_{n=1}^\infty C_n\right)^c\right) = \sum_{n=1}^\infty P(R_n) = \lim_{n \to \infty} \sum_{j=1}^n P(R_j) = \lim_{n \to \infty} [P(C_1^c) + P(C_1) - P(C_n)] = 1 - \lim_{n \to \infty} P(C_n)$$  
    Complementing both sides yields $P(\bigcap_{n=1}^\infty C_n) = \lim_{n \to \infty} P(C_n)$.
- Question 4:
    
    - _Ordered Field_: A field $F$ equipped with a total order relation $(<)$ that is compatible with field operations: (i) if $a < b$, then $a + c < b + c$; (ii) if $a < b$ and $c > 0$, then $ac < bc$.
    - _Axiom of Completeness_: Every nonempty set of real numbers that is bounded above has a least upper bound (supremum) in $\mathbb{R}$.
    
- Question 5: A Rational Number is any real value expressible as $\frac{p}{q}$ where $p, q \in \mathbb{Z}$ and $q \neq 0$. $\mathbb{Q}$ forms a field because it contains its multiplicative inverses ($\frac{q}{p}$) for all nonzero elements, closed under all rational operations. $\mathbb{Z}$ fails this because integers like $2$ do not have a multiplicative inverse in $\mathbb{Z}$.
- Question 6: A set $A \subset \mathbb{R}$ is bounded below if there exists an $le \in \mathbb{R}$ such that $a \geq le$ for all $a \in A$. The infimum ($\inf A$) is the unique greatest lower bound: it bounds $A$ below, and if $l$ is any lower bound for $A$, then $le \geq l$.
- Question 7: (1) $P(A) \geq 0$ for all events $A$; (2) $P(\mathcal{C}) = 1$; (3) For any sequence of pairwise disjoint events $\{A_n\}$, $P(\bigcup_{n=1}^\infty A_n) = \sum_{n=1}^\infty P(A_n)$.
- Question 8: A Random Experiment is a repeatable process with a known, well-defined set of outcomes that cannot be predicted with certainty prior to trial execution. The Sample Space ($\mathcal{C}$) is the universal set of _all_ possible outcomes; an Event is simply any subset of $\mathcal{C}$.
- Question 9: $P(C_1 \cap C_2) \geq P(C_1) + P(C_2) - 1$. It provides a meaningful positive bound only if the right-hand side is greater than 0, which requires $P(C_1) + P(C_2) > 1$.

---

## 📅 Day 2

- Question 1: Since $(a_n)$ converges, it is bounded: $\exists M > 0$ such that $\vert{}a_n\vert{} \leq M$ for all $n$. Add and subtract $a_n b$:  
    $$\vert{}a_n b_n - ab\vert{} = \vert{}a_n b_n - a_n b + a_n b - ab\vert{} \leq \vert{}a_n\vert{}\vert{}b_n - b\vert{} + \vert{}b\vert{}\vert{}a_n - a\vert{} \leq M\vert{}b_n - b\vert{} + \vert{}b\vert{}\vert{}a_n - a\vert{}$$  
    Given $\epsilon > 0$, select $N_1$ such that $\vert{}b_n - b\vert{} < \frac{\epsilon}{2M}$ for all $n \geq N_1$, and select $N_2$ such that $\vert{}a_n - a\vert{} < \frac{\epsilon}{2(\vert{}b\vert{} + 1)}$ for all $n \geq N_2$. Letting $N = \max(N_1, N_2)$, the sum collapses bounded underneath $\epsilon$ for all $n \geq N$.
- Question 2: $\log(xy) = \int_1^{xy} \frac{1}{t}dt = \int_1^x \frac{1}{t}dt + \int_x^{xy} \frac{1}{t}dt$. Apply coordinate transformation substitution $t = xu \implies dt = x\,du$ to the second integral block (adjusting boundaries from $[x, xy]$ down to $[1, y]$):  
    $$\int_x^{xy} \frac{1}{t}dt = \int_1^y \frac{1}{xu}(x\,du) = \int_1^y \frac{1}{u}du = \log y$$  
    Thus, $\log(xy) = \log x + \log y$.
- Question 3: Let $Y = F(X)$. The CDF of $Y$ for any $y \in (0,1)$ is $F_Y(y) = P(Y \leq y) = P(F(X) \leq y)$. Since $F$ is strictly increasing, its functional inverse inverse $F^{-1}$ is well-defined and preserves inequalities: $P(X \leq F^{-1}(y)) = F(F^{-1}(y)) = y$. Since $F_Y(y) = y$ for all $y \in (0,1)$, $Y \sim \text{Uniform}(0,1)$.
- Question 4: Relative Frequency is the ratio $\frac{f}{N}$, where $f$ tracks the absolute frequency count of an event occurring across $N$ independent identically distributed trial runs. Axioms: (1) $P(A) \geq 0$, (2) $P(\mathcal{C}) = 1$, (3) Countable additivity for mutually exclusive event streams.
- Question 5: A sequence $(a_n)$ converges to $a$ if for every $\epsilon > 0$, there exists a natural index cut-off $N \in \mathbb{N}$ such that $\vert{}a_n - a\vert{} < \epsilon$ for all indices $n \geq N$.
- Question 6: A Monotone Sequence is a sequence that moves exclusively in a single direction. A _non-decreasing sequence_ allows consecutive elements to be equal ($a_n \leq a_{n+1}$), whereas a _strictly increasing sequence_ forbids equality ($a_n < a_{n+1}$).
- Question 7: The theorem states that algebraic limits preserve non-strict bounds. If $a_n \geq 0$ for all $n$ and $a_n \to a$, then $a \geq 0$.
- Question 8: An estimator $\hat{\theta}$ is unbiased for a parameter $\theta$ if its mathematical expectation equals the true parameter value: $E[\hat{\theta}] = \theta$.
- Question 9: $\bar{X} = \frac{1}{n}\sum_{i=1}^n X_i$. Linear expectations ensure $E[\bar{X}] = \mu$, and the independence constraint across elements ensures $\text{Var}(\bar{X}) = \frac{\sigma^2}{n}$.

---

## 📅 Day 3

- Question 1: Let $a_n \to a$. Given $\epsilon > 0$, find $N$ such that $\vert{}a_k - a\vert{} < \frac{\epsilon}{2}$ for all $k \geq N$. For any $n, m \geq N$, the triangle inequality ensures: $\vert{}a_n - a_m\vert{} = \vert{}a_n - a + a - a_m\vert{} \leq \vert{}a_n - a\vert{} + \vert{}a - a_m\vert{} < \frac{\epsilon}{2} + \frac{\epsilon}{2} = \epsilon$.
    
    - _Positive Negation statement_: "There exists a static baseline error margin $\epsilon_0 > 0$ such that for every target index index checkpoint $N \in \mathbb{N}$, there exist two trailing indices $n, m \geq N$ that satisfy $\vert{}a_n - a_m\vert{} \geq \epsilon_0$."
    
- Question 2: Let $f(x) = \frac{e^x}{x^n}$. Applying L'Hôpital's Rule iteratively $n$ times as $x \to \infty$ yields $\lim_{x \to \infty} \frac{e^x}{n!} = \infty$. Thus, $e^x$ exhibits a higher order of magnitude than any polynomial scale: $x^n = o(e^x)$ or $e^x = O(x^n)$ is false since exponential growth completely dominates polynomials over the continuum.
- Question 3: Let $A = \{x : u(x) \geq c\}$. By definition of expected value:  
    $$E[u(X)] = \int_{-\infty}^\infty u(x)f(x)dx \geq \int_A u(x)f(x)dx \geq \int_A c \cdot f(x)dx = c \int_A f(x)dx = c \cdot P(u(X) \geq c)$$  
    Dividing by macro multiplier $c$ isolates $P(u(X) \geq c) \leq \frac{E[u(X)]}{c}$.
- Question 4: $M(t) = E[e^{tX}]$ defined across an open window around zero ($-h < t < h$). It serves as a moment generator because evaluating its $k$-th derivative at zero yields the $k$-th raw moment: $M^{(k)}(0) = E[X^k]$.
- Question 5: A sequence $(a_n)$ is Cauchy if $\forall \epsilon > 0, \exists N \in \mathbb{N}$ such that $\vert{}a_n - a_m\vert{} < \epsilon$ for all indices $n, m \geq N$.
- Question 6: A monotone sequence of real numbers converges if and only if it is bounded in the direction of its monotonic movement.
- Question 7: $P(\vert{}X - \mu\vert{} \geq k\sigma) \leq \frac{1}{k^2}$. It is derived by setting $u(X) = (X - \mu)^2$ and setting threshold constant $c = k^2\sigma^2$ in Markov's Inequality.
- Question 8: $S^2 = \frac{1}{n-1}\sum_{i=1}^n (X_i - \bar{X})^2$. The denominator correction $n-1$ compensates for the structural loss of independence (1 degree of freedom lost) resulting from using the sample estimator $\bar{X}$ instead of the true population parameter $\mu$.
- Question 9: $\text{Var}(X) = E[X^2] - (E[X])^2$.

---

## 📅 Day 4

- Question 1: Let $F$ be closed $\implies F^c$ is open. If $x_n \to x$ with $x_n \in F$, assume $x \notin F \implies x \in F^c$. Since $F^c$ is open, there is an $\epsilon$-neighborhood $V_\epsilon(x) \subseteq F^c$. Since $x_n \to x$, elements must enter $V_\epsilon(x)$, meaning $x_n \in F^c$, which contradicts $x_n \in F$.
    
    - _Conversely_: If $F$ contains its sequential limits, assume $F^c$ is not open. Then $\exists x \in F^c$ such that every neighborhood $V_{1/n}(x)$ hits an element $x_n \in F$. This forms a sequence $x_n \to x$, forcing limit $x \in F$, creating a contradiction.
    
- Question 2: Differentials: $\dot{x} = -3\cos^2 t \sin t$ and $\dot{y} = 3\sin^2 t \cos t$. Square and sum under square root:  
    $$\sqrt{\dot{x}^2 + \dot{y}^2} = \sqrt{9\cos^4 t \sin^2 t + 9\sin^4 t \cos^2 t} = 3\sin t \cos t \sqrt{\cos^2 t + \sin^2 t} = 3\sin t \cos t = \frac{3}{2}\sin(2t)$$  
    Integrate along tracking domain bounds: $s = \int_0^{\pi/2} \frac{3}{2}\sin(2t)dt = \left[ -\frac{3}{4}\cos(2t) \right]_0^{\pi/2} = \frac{3}{4} - (-\frac{3}{4}) = \frac{3}{2}$.
- Question 3: Express inverses: $X_1 = \frac{Y_1 + Y_2}{2}$ and $X_2 = \frac{Y_1 - Y_2}{2}$. Set up the Jacobian matrix layout of partial derivatives:  
    $$J = \begin{vmatrix} \partial X_1/\partial Y_1 & \partial X_1/\partial Y_2 \\ \partial X_2/\partial Y_1 & \partial X_2/\partial Y_2 \end{vmatrix} = \begin{vmatrix} 1/2 & 1/2 \\ 1/2 & -1/2 \end{vmatrix} = -\frac{1}{4} - \frac{1}{4} = -\frac{1}{2}$$  
    Taking the absolute value yields $\vert{}J\vert{} = \frac{1}{2}$. Thus, $f_{Y_1, Y_2}(y_1, y_2) = \frac{1}{2} f_{X_1, X_2}\left(\frac{y_1 + y_2}{2}, \frac{y_1 - y_2}{2}\right)$.
- Question 4:
    
    - - Neighborhood*: $V_\epsilon(x_0) = \{x \in \mathbb{R} : \vert{}x - x_0\vert{} < \epsilon\}$.
        
    - _Limit Point_: $x$ is a limit point of $A$ if every deleted neighborhood $V_\epsilon(x) \setminus \{x\}$ contains an element of $A$.
    - _Isolated Point_: An element $a \in A$ that is not a limit point of $A$ (isolated by a buffer zone).
    
- Question 5: An Open Set is a set where every point is an interior point: $\forall x \in O, \exists \epsilon > 0$ such that $V_\epsilon(x) \subseteq O$. The Closure ($\bar{A}$) is the union of the parent set with all its limit points: $\bar{A} = A \cup A'$.
- Question 6: An Open Cover for a set $A$ is a collection of open sets $\{O_\gamma\}$ whose global mathematical union entirely covers the space: $A \subseteq \bigcup_\gamma O_\gamma$.
- Question 7: Laws: $(A \cap B)^c = A^c \cup B^c$ and $(A \cup B)^c = A^c \cap B^c$.
    
    - _Proof Strategy_: Show containment both ways. If $x \in \left(A \cap B\right)^c \implies x \notin A \cap B \implies x$ is not in both sets simultaneously $\implies x \notin A$ or $x \notin B \implies x \in A^c$ or $x \in B^c \implies x \in A^c \cup B^c$. Repeat in reverse.
    
- Question 8: A Joint PDF measures concurrent intersection densities across multiple random variables over an area. A Marginal PDF tracks a single isolated random variable, found by completely integrating out the remaining dimensional vectors.
- Question 9: $\text{Cov}(X,Y) = E[(X - E[X])(Y - E[Y])] = E[XY] - E[X]E[Y]$.

---

## 📅 Day 5

- Question 1: Assume $\lim_{x \to c} f(x) = L$. Given $\epsilon > 0$, find $\delta > 0$ such that $0 < \vert{}x - c\vert{} < \delta \implies \vert{}f(x) - L\vert{} < \epsilon$. If $x_n \to c$ ($x_n \neq c$), find $N$ such that $0 < \vert{}x_n - c\vert{} < \delta$ for all $n \geq N$. Combining them implies $\vert{}f(x_n) - L\vert{} < \epsilon$, so $f(x_n) \to L$.
    
    - _Conversely_: Assume the functional limit fails $\implies \exists \epsilon_0 > 0$ such that for every $\delta = 1/n$, there is an $x_n$ satisfying $0 < \vert{}x_n - c\vert{} < 1/n$ but $\vert{}f(x_n) - L\vert{} \geq \epsilon_0$. This constructs a sequence $x_n \to c$ where $f(x_n) \not\to L$, a contradiction.
    
- Question 2: Statement: If $f$ is continuous on $[a,b]$, there exists $\xi \in (a,b)$ such that $\int_a^b f(x)dx = f(\xi)(b-a)$.
    
    - _Geometric interpretation_: The exact area under the continuous curve over $[a,b]$ can be matched by a single rectangle with width $(b-a)$ and height $f(\xi)$, representing the true average functional value.
    
- Question 3: Expand the sum: $\sum (X_i - \bar{X})^2 = \sum ((X_i - \mu) - (\bar{X} - \mu))^2 = \sum (X_i - \mu)^2 - n(\bar{X} - \mu)^2$. Linear expectation distributes across operations:  
    $$E\left[\sum (X_i - \bar{X})^2\right] = \sum E[(X_i - \mu)^2] - n E[(\bar{X} - \mu)^2] = \sum \sigma^2 - n \text{Var}(\bar{X}) = n\sigma^2 - n\left(\frac{\sigma^2}{n}\right) = (n-1)\sigma^2$$  
    Taking $E[S^2] = E\left[\frac{1}{n-1}\sum (X_i - \bar{X})^2\right] = \frac{n-1}{n-1}\sigma^2 = \sigma^2$.
- Question 4: A Statistic is any function of the observable random sample data that does not depend on any unknown parameters. An estimator $\hat{\theta}$ is Unbiased if its sampling distribution centers exactly on the parameter: $E[\hat{\theta}] = \theta$.
- Question 5: $\lim_{x \to c} f(x) = L$ if $\forall \epsilon > 0, \exists \delta > 0$ such that $0 < \vert{}x - c\vert{} < \delta \implies \vert{}f(x) - L\vert{} < \epsilon$.
- Question 6: $f$ is continuous at $c$ if $\lim_{x \to c} f(x) = f(c)$, meaning $\forall \epsilon > 0, \exists \delta > 0$ such that $\vert{}x - c\vert{} < \delta \implies \vert{}f(x) - f(c)\vert{} < \epsilon$.
- Question 7: The quantile function $q_p$ for $p \in (0,1)$ is the generalized inverse inverse of the CDF, defined as $q_p = \inf\{x \in \mathbb{R} : F(x) \geq p\}$.
- Question 8: $\rho = \frac{\text{Cov}(X,Y)}{\sigma_X \sigma_Y}$. Boundaries: $-1 \leq \rho \leq 1$.
- Question 9: If $f$ is continuous on $[a,b]$ and differentiable on $(a,b)$, there exists $c \in (a,b)$ such that $f'(c) = \frac{f(b)-f(a)}{b-a}$.

---

## 📅 Day 6

- Question 1: Let $f(x) = \frac{1}{x}$ on domain interval $A = (0, 1)$. Choose tracking sequences $x_n = \frac{1}{n}$ and $y_n = \frac{1}{n+1}$. The distance between sequences vanishes: $\vert{}x_n - y_n\vert{} = \frac{1}{n(n+1)} \to 0$. However, their functional outputs remain separated: $\vert{}f(x_n) - f(y_n)\vert{} = \vert{}n - (n+1)\vert{} = 1 \geq \epsilon_0$. This violates the uniform requirement.
- Question 2: Let curve rotation be mapped by orthogonal transformation matrices: $x' = x\cos\theta + y\sin\theta$ and $y' = -x\sin\theta + y\cos\theta$. Differentiating gives $\dot{x}' = \dot{x}\cos\theta + \dot{y}\sin\theta$ and $\dot{y}' = -\dot{x}\sin\theta + \dot{y}\cos\theta$. Squaring and summing variables balances under trigonometry rules:  
    $$(\dot{x}')^2 + (\dot{y}')^2 = (\dot{x}\cos\theta + \dot{y}\sin\theta)^2 + (-\dot{x}\sin\theta + \dot{y}\cos\theta)^2 = (\dot{x})^2(\cos^2\theta + \sin^2\theta) + (\dot{y})^2(\sin^2\theta + \cos^2\theta) = (\dot{x})^2 + (\dot{y})^2$$  
    Since the integrand $\sqrt{(\dot{x}')^2 + (\dot{y}')^2} = \sqrt{\dot{x}^2 + \dot{y}^2}$, the arc length integral remains perfectly invariant.
- Question 3: By definition of conditional expectations and joint integration density structures:  
    $$E[E[Y\vert{}X]] = \int_{-\infty}^\infty E[Y\vert{}x] f_X(x)dx = \int_{-\infty}^\infty \left[ \int_{-\infty}^\infty y \frac{f(x,y)}{f_X(x)} dy \right] f_X(x)dx$$  
    Canceling the marginal density denominator $f_X(x)$ yields:  
    $$= \int_{-\infty}^\infty \int_{-\infty}^\infty y f(x,y) \,dy\,dx = E[Y]$$
- Question 4: Continuous variables are independent if and only if their joint distribution is a multiplicative product of their marginals: $f(x,y) = f_X(x)f_Y(y)$ across their entire spatial support field.
- Question 5: Ordinary continuity permits $\delta$ to depend on both $\epsilon$ and the localized position coordinates $c$. Uniform Continuity enforces a higher standard where $\delta$ depends _strictly_ on $\epsilon$, applying universally across the entire set domain.
- Question 6: An open interval excludes endpoints; a closed interval includes them. The intersection $\bigcap_{n=1}^\infty (-\frac{1}{n}, \frac{1}{n})$ collapses to the singleton set $\{0\}$. Single points are closed sets, so it fails to remain open.
- Question 7: For continuous variables: $E[Y\vert{}x] = \int_{-\infty}^\infty y f_{Y\vert{}X}(y\vert{}x)dy = \int_{-\infty}^\infty y \frac{f(x,y)}{f_X(x)}dy$.
- Question 8: A matrix $\boldsymbol{\Sigma}$ where the element at row $i$, column $j$ is defined by $\Sigma_{ij} = \text{Cov}(X_i, X_j)$.
- Question 9: A collection of $n$ random variables $X_1, \dots, X_n$ that are independent and identically distributed (i.i.d.).

---

## 📅 Day 7

- Question 1: Let $(y_n)$ be a sequence in $f(K)$. Then $y_n = f(x_n)$ for some $x_n \in K$. Since $K$ is compact, it is sequentially compact, so $(x_n)$ has a subsequence $(x_{n_k})$ converging to some $x \in K$. Since $f$ is continuous, the sequential criterion ensures $f(x_{n_k}) \to f(x)$. Thus, the subsequence $(y_{n_k})$ converges to $f(x) \in f(K)$, proving $f(K)$ is compact.
- Question 2: Thomae's function outputs $1/q$ at rationals $p/q$ (in lowest terms) and $0$ at irrationals.
    
    - _Proof of Continuity at Irrational $c$_: Given $\epsilon > 0$, there are only finitely many rational fractions in $(0,1)$ with denominator $q \leq 1/\epsilon$. Choose $\delta > 0$ small enough so that the interval $(c-\delta, c+\delta)$ contains none of these finite rational points. For any $x$ in this delta neighborhood, if $x$ is rational, its denominator must satisfy $q > 1/\epsilon \implies f(x) = 1/q < \epsilon$. If $x$ is irrational, $f(x) = 0 < \epsilon$. Thus, $\vert{}f(x) - f(c)\vert{} < \epsilon$, establishing continuity. (Discontinuity at rationals follows because dense irrationals in any delta bubble output 0, preventing convergence to $1/q$).
    
- Question 3: The structural pivot variable is $T = \frac{\bar{X} - \mu}{S / \sqrt{n}}$. By Student's Theorem, $\bar{X}$ and $S^2$ are independent, and $\frac{(n-1)S^2}{\sigma^2} \sim \chi^2(n-1)$, which forces $T \sim t(n-1)$. Isolating $\mu$ yields:  
    $$P\left(-t_{\alpha/2, n-1} \leq \frac{\bar{X} - \mu}{S/\sqrt{n}} \leq t_{\alpha/2, n-1}\right) = 1 - \alpha \implies \bar{X} \pm t_{\alpha/2, n-1} \left(\frac{S}{\sqrt{n}}\right)$$
- Question 4:
    
    - _Perfect Set_: A closed set containing zero isolated points (every point is a limit point).
    - _Connected Set_: A set that cannot be separated into two non-empty disjoint parts that contain no limit points of each other.
    
- Question 5: A subset of $\mathbb{R}$ is compact if and only if it is closed and bounded.
- Question 6: A continuous function on a compact set attains its maximum and minimum values. The required domain constraint is compactness.
- Question 7: If $f$ is continuous on $[a,b]$ and $L$ is a value between $f(a)$ and $f(b)$, there exists $c \in (a,b)$ such that $f(c) = L$.
- Question 8: For any convex function $\phi$, $E[\phi(X)] \geq \phi(E[X])$.
- Question 9: The parameters are $\mu_1, \mu_2, \sigma_1^2, \sigma_2^2$, and $\rho$. The component that isolates the linear alignment factor is the correlation coefficient ($\rho$).

---

## 🚀 Optimization Follow-Ups

- Would you like to introduce asymptotic expansion patterns into next week's layout to prepare for multi-parameter variance tracking?
- Should we establish a self-grading rubric matching specific deduction points to proof holes (e.g., forgetting to assert independence during variance expansion)?
- Do you prefer to expand the definition list to cover Baire Category theorem layers or robustness tracking indices?
