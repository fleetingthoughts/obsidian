---
parent: "[[_Fleeting]]"
tags:
  - "#fleeting"
date_created: 2026-05-23
---
Here is your non-overlapping, fully interleaved weekly flashcard curriculum. It contains 35 distinct master cards (5 per day) engineered to cover your exact core syllabus bounds across Calculus, Real Analysis, Linear Algebra, and Mathematical Statistics.

---

## 📅 Day 1: Metrics, Mappings, and Core Dynamics

## Card 1 (Real Analysis)

- Front: State the Reverse Triangle Inequality for real numbers.
- Back:
    
    - Formula: $||a| - |b|| \leq |a - b|$ for all $a, b \in \mathbb{R}$.
    - Abbott Context: Essential variation of the standard Triangle Inequality used to establish absolute lower bounds for spatial distances.
    

## Card 2 (Linear Algebra)

- Front: What are the three specific properties required to show a subset $W$ is a subspace of a vector space $V$?
- Back:
    
    - Properties:
        
        1. The zero vector is inside the subset ($0 \in W$).
        2. $W$ is closed under vector addition ($x, y \in W \implies x + y \in W$).
        3. $W$ is closed under scalar multiplication ($c \in F, x \in W \implies cx \in W$).
        
    - Friedberg Context: Because global operations are inherited naturally, checking these three closure criteria is fully sufficient to declare a subspace structure.
    

## Card 3 (Math Stats)

- Front: State the strict definition of a Cumulative Distribution Function (CDF) for any random variable $X$.
- Back:
    
    - Formula: $F(x) = P(X \leq x)$ for all real numbers $-\infty < x < \infty$.
    - Hogg Context: Maps out the entire cumulative probability accumulation profile of a random variable across its support.
    

## Card 4 (Calculus)

- Front: State the mathematical formulation of the Chain Rule for the differentiation of composite functions.
- Back:
    
    - Formula: $\frac{d}{dx}[f(g(x))] = f'(g(x)) \cdot g'(x)$.
    - Courant Context: Breaks down a compound rate of change across nested functional linkages into a product of local derivative steps.
    

## Card 5 (Linear Algebra)

- Front: Define what it means for a scalar $\lambda$ and a non-zero vector $v$ to be an eigenvalue and eigenvector of a linear operator $T$.
- Back:
    
    - Definition: $T(v) = \lambda v$ where $v \neq 0$.
    - Friedberg Context: Identifies a characteristic spatial direction where the transformation acts as a simple scalar stretch or compression.
    

---

## 📅 Day 2: Counts, Lists, and Fundamental Inversions

## Card 6 (Real Analysis)

- Front: State the precise mathematical definition of a countable set.
- Back:
    
    - Definition: A set $A$ is countable if it has the same cardinality as the natural numbers ($\mathbb{N} \sim A$).
    - Abbott Context: Requires the existence of a bijective (1-1 and onto) function $f: \mathbb{N} \to A$, meaning its elements can be cleanly matched to an infinitely long list.
    

## Card 7 (Linear Algebra)

- Front: Define exactly what it means for a finite subset of vectors $\{u_1, u_2, \dots, u_n\}$ to be linearly independent.
- Back:
    
    - Definition: The vector equation $a_1 u_1 + a_2 u_2 + \dots + a_n u_n = 0$ forces all scalar coefficients to be zero ($a_1 = a_2 = \dots = a_n = 0$).
    - Friedberg Context: A configuration where no single vector inside the subset can be constructed as a linear combination of the remaining elements.
    

## Card 8 (Math Stats)

- Front: State the mathematical formulas used to count permutations ($P_k^n$) versus combinations ($\binom{n}{k}$).
- Back:
    
    - Formulas: $P_k^n = \frac{n!}{(n-k)!}$ versus $\binom{n}{k} = \frac{n!}{k!(n-k)!}$.
    - Hogg Context: Permutations track distinct ordered arrangements, whereas combinations ignore ordering to count unique subset configurations drawn from an asset pool.
    

## Card 9 (Calculus)

- Front: State the Fundamental Theorem of Calculus concerning the derivative of a functional accumulation area.
- Back:
    
    - Formula: $\frac{d}{dx} \left[ \int_{a}^{x} f(t) \, dt \right] = f(x)$, assuming $f$ is continuous.
    - Courant Context: Pairs rate changes with accumulations to formally demonstrate that differentiation and integration are direct inverse operators.
    

## Card 10 (Math Stats)

- Front: State the mathematical definition for the structural independence of two events $A$ and $B$.
- Back:
    
    - Formula: $P(A \cap B) = P(A)P(B)$.
    - Hogg Context: This multiplicative property holds true if and only if the occurrence of event $A$ provides absolutely zero predictive information about the likelihood of event $B$.
    

---

## 📅 Day 15: Neighborhoods, Dimensions, and Discreteness

## Card 11 (Real Analysis)

- Front: State the formal $\epsilon$-$N$ definition for the limit of a sequence $(a_n)$.
- Back:
    
    - Definition: $\forall \epsilon > 0, \exists N \in \mathbb{N}$ such that $\forall n \geq N$, $|a_n - L| < \epsilon$.
    - Abbott Context: The indexing tail coordinate $N$ forces the remaining infinite path of the sequence to stay entirely trapped inside an $\epsilon$-neighborhood around limit $L$.
    

## Card 12 (Linear Algebra)

- Front: State the Dimension Theorem (Rank-Nullity Theorem) for finite-dimensional spaces.
- Back:
    
    - Formula: $\dim(V) = \dim(N(T)) + \dim(R(T))$.
    - Friedberg Context: Proves that a linear transformation splits the domain space's degrees of freedom cleanly between collapsed elements (Null Space) and preserved outputs (Range).
    

## Card 13 (Math Stats)

- Front: State the probability mass function (PMF), mean, and variance of a Poisson Distribution.
- Back:
    
    - Formula: $p(x) = \frac{e^{-\lambda}\lambda^x}{x!}$ for $x \in \{0, 1, 2, \dots\}$, where $\lambda > 0$.
    - Parameters: Mean $\mu = \lambda$, Variance $\sigma^2 = \lambda$.
    - Hogg Context: Classic discrete model used to map out the occurrence rate of independent events falling within a fixed, continuous tracking domain.
    

## Card 14 (Calculus)

- Front: State the analytical formula for computing the derivative of an inverse function $f^{-1}(y)$.
- Back:
    
    - Formula: $(f^{-1})'(y_0) = \frac{1}{f'(x_0)}$ where $y_0 = f(x_0)$ and $f'(x_0) \neq 0$.
    - Courant Context: Geometrically, swapping your definition of independent coordinate axes naturally reciprocates the instantaneous tangent slopes along a smooth profile.
    

## Card 15 (Real Analysis)

- Front: Define an open set $O \subseteq \mathbb{R}$ using the concept of neighborhoods.
- Back:
    
    - Definition: A set $O$ is open if for every element $x \in O$, there exists an $\epsilon > 0$ such that the $\epsilon$-neighborhood $V_\epsilon(x) = (x-\epsilon, x+\epsilon)$ is entirely contained inside $O$.
    - Abbott Context: A configuration where _every point is an interior point_, creating a structural buffer zone around all elements.
    

---

## 📅 Day 4: Bounds, Bases, and Sample Variances

## Card 16 (Real Analysis)

- Front: State the Monotone Convergence Theorem for sequences.
- Back:
    
    - Theorem: A monotone sequence converges if and only if it is bounded.
    - Abbott Context: A direct consequence of the completeness of the real line, establishing that unidirectional real numbers cannot avoid hitting a limiting boundary if blocked.
    

## Card 17 (Linear Algebra)

- Front: Define how the entry elements of a matrix representation $[T]_\beta^\gamma$ are structurally determined.
- Back:
    
    - Definition: The $j$-th column of $[T]_\beta^\gamma$ is the coordinate vector of $T(v_j)$ relative to the ordered basis $\gamma$, where $v_j$ is the $j$-th vector of the ordered basis $\beta$.
    - Friedberg Context: Concrete translation mechanism that cleanly binds abstract linear operators directly to column-and-row matrix structures.
    

## Card 18 (Math Stats)

- Front: State the strict mathematical definition of Convergence in Probability ($X_n \xrightarrow{p} X$).
- Back:
    
    - Definition: $\lim_{n \to \infty} P(|X_n - X| \geq \epsilon) = 0$ for all $\epsilon > 0$.
    - Hogg Context: Asymptotic evaluation mode used to establish _estimator consistency_, ensuring tracking errors collapse to zero as your data pool expands.
    

## Card 19 (Calculus)

- Front: State the general formula for Integration by Parts on a bounded definite segment.
- Back:
    
    - Formula: $\int_a^b u \, dv = [uv]_a^b - \int_a^b v \, du$.
    - Courant Context: Structural integration maneuver used to crack complex product profiles by systematically reversing the differential product rule.
    

## Card 20 (Linear Algebra)

- Front: List the three properties required to define an Inner Product $\langle x, y \rangle$ on a real vector space.
- Back:
    
    - Properties:
        
        1. Linearity: $\langle cx+y, z \rangle = c\langle x, z \rangle + \langle y, z \rangle$.
        2. Symmetry: $\langle x, y \rangle = \langle y, x \rangle$.
        3. Positive-Definiteness: $\langle x, x \rangle \geq 0$, and $\langle x, x \rangle = 0 \iff x = 0$.
        
    - Friedberg Context: Mathematical scaffolding needed to introduce spatial constraints—like metrics, lengths, and orthogonal angles—to linear vector domains.
    

---

## 📅 Day 5: Subsequences, Adjoints, and Average Trends

## Card 21 (Real Analysis)

- Front: State the Bolzano–Weierstrass Theorem for real sequences.
- Back:
    
    - Theorem: Every bounded sequence contains a convergent subsequence.
    - Abbott Context: Core topological property of $\mathbb{R}$: trapping an infinite sequence inside a closed boundary forces its components to cluster somewhere.
    

## Card 22 (Linear Algebra)

- Front: Define the Adjoint $T^*$ of a linear operator on an inner product space.
- Back:
    
    - Definition: The unique linear operator satisfying $\langle T(x), y \rangle = \langle x, T^*(y) \rangle$ for all vectors $x, y \in V$.
    - Friedberg Context: The absolute structural counterpart to an operator, allowing mappings to slide smoothly across inner product pairings.
    

## Card 23 (Math Stats)

- Front: State the mathematical requirement for an estimator $\hat{\theta}$ to be considered unbiased.
- Back:
    
    - Definition: An estimator satisfies $E[\hat{\theta}] = \theta$ for all parameter values in the parameter space.
    - Hogg Context: Guarantees that the estimator's sampling distribution centers accurately on the true target without introducing systematic distortion.
    

## Card 24 (Calculus)

- Front: State the Mean Value Theorem for derivatives.
- Back:
    
    - Formula: $f'(c) = \frac{f(b) - f(a)}{b - a}$ for at least one point $c \in (a, b)$.
    - Preconditions: $f$ is continuous on $[a, b]$ and differentiable on $(a, b)$.
    - Courant Context: Mechanical verification that a smooth curve must possess a point where its local tangent mirrors its regional chord.
    

## Card 25 (Math Stats)

- Front: State the analytical formula for Fisher Information $I(\theta)$ within a single observation.
- Back:
    
    - Formula: $I(\theta) = E\left[\left(\frac{\partial}{\partial \theta} \log f(X;\theta)\right)^2\right] = -E\left[\frac{\partial^2}{\partial \theta^2} \log f(X;\theta)\right]$.
    - Hogg Context: Measures the expected informational payload of a single sample, defining the variance baseline for parameter estimation.
    

---

## 📅 Day 6: Compactness, Decoupling, and Sufficiency

## Card 26 (Real Analysis)

- Front: State the topological characterization of a compact set in $\mathbb{R}$ via the Heine–Borel Theorem.
- Back:
    
    - Theorem: A subset of $\mathbb{R}$ is compact if and only if it is both closed and bounded.
    - Abbott Context: Closed and bounded structures lock down infinite topologies, ensuring that any open cover can be safely reduced down to a finite subcover.
    

## Card 27 (Linear Algebra)

- Front: State the operational definition of a diagonalizable linear operator $T$.
- Back:
    
    - Definition: An operator is diagonalizable if there exists an ordered basis $\beta$ such that $[T]_\beta$ is a diagonal matrix.
    - Friedberg Context: This condition requires the vector space to possess a basis consisting entirely of eigenvectors, decoupling complex systems into independent scalar paths.
    

## Card 28 (Math Stats)

- Front: State the Fisher–Neyman Factorization Theorem for parameter sufficiency.
- Back:
    
    - Theorem: A statistic $u(\mathbf{X})$ is sufficient for $\theta$ if and only if the joint density factors into: $f(\mathbf{x};\theta) = g(u(\mathbf{x});\theta) \cdot h(\mathbf{x})$.
    - Hogg Context: Isolating the parameter link into a dedicated kernel function proves that the remaining raw sample data features contain zero extra parameter insights.
    

## Card 29 (Calculus)

- Front: State the Mean Value Theorem for Integrals.
- Back:
    
    - Formula: $\int_a^b f(x) \, dx = f(c)(b - a)$ for some point $c \in [a, b]$.
    - Precondition: $f$ must be continuous on $[a, b]$.
    - Courant Context: Geometrically proves that the total accumulated area under a continuous profile can always be exactly matched by a single rectangle evaluated at an intermediate point.
    

## Card 30 (Real Analysis)

- Front: State the structural definition of Uniform Continuity across a domain $A$.
- Back:
    
    - Definition: $\forall \epsilon > 0, \exists \delta > 0$ such that $\forall x, y \in A$, $|x - y| < \delta \implies |f(x) - f(y)| < \epsilon$.
    - Abbott Context: Differs from local continuity by locking down a single, global distance control $\delta$ that operates independently of position in the set.
    

---

## 📅 Day 7: Limits, Complements, and Errors

## Card 31 (Real Analysis)

- Front: State the theorem regarding Uniform Convergence and Differentiation for functional series.
- Back:
    
    - Theorem: If $f_n \to f$ pointwise, $f_n'$ converges uniformly to a function $g$ on $[a, b]$, then $f_n \to f$ uniformly, $f$ is differentiable, and $f' = g$.
    - Abbott Context: Outlines the explicit conditions required to safely swap limit operators and derivative steps without causing functional distortion.
    

## Card 32 (Linear Algebra)

- Front: Define the Orthogonal Complement $W^\perp$ of a subspace $W$ within an inner product space $V$.
- Back:
    
    - Definition: $W^\perp = \{x \in V : \langle x, y \rangle = 0 \text{ for all } y \in W\}$.
    - Friedberg Context: Isolates independent geometric environments, cleanly partitioning vectors into linear combinations of orthogonal projections.
    

## Card 33 (Math Stats)

- Front: State the classical univariate Central Limit Theorem (CLT).
- Back:
    
    - Theorem: Let $X_1, \dots, X_n$ be an i.i.d. sequence with mean $\mu$ and finite variance $\sigma^2 > 0$. As $n \to \infty$, $\frac{\bar{X}_n - \mu}{\sigma/\sqrt{n}} \xrightarrow{d} \mathcal{N}(0, 1)$.
    - Hogg Context: Large averages of independent random risks naturally track normal profiles at the limit, regardless of the population's starting shape.
    

## Card 34 (Calculus)

- Front: State the Fundamental Theorem of Calculus for evaluating definite integrals via primitives.
- Back:
    
    - Formula: $\int_a^b f(x) \, dx = F(b) - F(a)$, where $F'(x) = f(x)$.
    - Precondition: $f$ must be continuous on $[a, b]$.
    - Courant Context: Major computational shortcut, bypassing tedious Riemann grid summation limits through direct antiderivative evaluation.
    

## Card 35 (Math Stats)

- Front: Differentiate between statistical Type I Errors and Type II Errors.
- Back:
    
    - Type I Error: Rejecting a null hypothesis $H_0$ when $H_0$ is actually true (Probability = $\alpha$).
    - Type II Error: Retaining a null hypothesis $H_0$ when $H_0$ is actually false (Probability = $\beta$).
    - Hogg Context: Testing architectures must balance these competing error types to structure robust boundaries for statistical decisions.
    

---

Would you like to expand this system? We can target a sub-deck for Calculus numerical approximations or work out step-by-step proofs for the active limits found on Day 4 and Day 7!