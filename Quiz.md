## 📅 Day 1

1. According to Theorem 2.1, if $T: V \to W$ is a linear transformation, why must $T(0_V) = 0_W$ be true? Prove this in one line using scalar multiplication properties.
2. Theorem 2.2 states that if $\beta$ is a basis for $V$, then $R(T) = \text{span}(T(\beta))$. If $\beta$ is a linearly independent set but _not_ a basis for $V$, does $T(\beta)$ still span $R(T)$? Explain why or why not.
3. According to Theorem 2.8, $[T+U]_\beta^\gamma = [T]_\beta^\gamma + [U]_\beta^\gamma$. If you alter the internal sequencing of the ordered basis $\beta$, does the matrix equality still hold? What changes about the components of the matrix?
4. Theorem 2.7 establishes that any scalar combination $aT + U$ of linear transformations is also linear. What structural role does the zero transformation $T_0$ play in the resulting vector space $\mathcal{L}(V, W)$?
5. State the formal definition of a rearrangement of an infinite series using a bijection $f: \mathbb{N} \to \mathbb{N}$. What major criterion dictates whether a rearrangement alters the sum?
6. Reconstruct the operational extraction of variance to prove that $\text{Var}(X) = E(X^2) - [E(X)]^2$:
    
    - Let $\mu = E(X)$. By definition, $\text{Var}(X) = E[(X - \mu)^2]$.
    - Expand the internal polynomial within the expectation: $(X - \mu)^2 = X^2 - \underline{\quad\text{(a)}\quad} + \mu^2$.
    - Apply the linearity properties of the expectation operator $E$: $\text{Var}(X) = E(X^2) - E(2\mu X) + E(\mu^2)$.
    - Factor out deterministic constants to complete: $\text{Var}(X) = E(X^2) - 2\mu(\underline{\quad\text{(b)}\quad}) + \mu^2$.
    
7. Reconstruct the proof that the range $R(T)$ of a linear transformation $T: V \to W$ is a valid structural subspace of the codomain space $W$:
    
    - Verify non-emptiness: Since $T$ is linear, $T(0_V) = \underline{\quad\text{(c)}\quad}$, meaning that the zero vector belongs to the range.
    - Show addition closure: Let $x, y \in R(T)$. There must exist elements $v, w \in V$ such that $T(v) = x$ and $T(w) = y$.
    - Evaluate: $x + y = T(v) + T(w) = \underline{\quad\text{(d)}\quad}$. Because $v + w \in V$, it follows that $x + y \in R(T)$.
    - Show scalar closure: Let $c \in F$. Evaluate: $cx = c T(v) = \underline{\quad\text{(e)}\quad}$. Since $cv \in V$, $cx \in R(T)$.
    

---

## 📅 Day 2

1. State the exact algebraic balance equation of the Dimension Theorem (Theorem 2.3). If $T: \mathbb{R}^5 \to \mathbb{R}^3$ is surjective, what is the exact dimension of its null space?
2. According to Theorem 2.4, what is the unique necessary and sufficient condition for a linear transformation to be one-to-one? If a non-linear function satisfies this same kernel condition, does it guarantee injectivity?
3. If $V$ is an $n$-dimensional space and $W$ is an $m$-dimensional space, Theorem 2.8 implies $[T]_\beta^\gamma$ belongs to $M_{m \times n}(F)$. If $T$ is an entry in $\mathcal{L}(V, W)$, why are the rows determined by $\dim(W)$ and columns by $\dim(V)$, rather than vice-versa?
4. Based on Theorem 2.3, if $T: V \to W$ is a linear transformation and $\dim(V) < \dim(W)$, can $T$ ever be onto? Explain using the relationship between $\text{rank}(T)$ and $\dim(V)$.
5. Define an $\epsilon$-neighborhood $V_\epsilon(a)$. Rephrase the standard definition of sequence convergence using the phrase "all but a finite number of the terms".
6. Reconstruct the structural steps showing that the limit of a sequence is mathematically unique:
    
    - Assume distinct targets exist such that $(a_n) \to a$ and $(a_n) \to b$ where $a \neq b$.
    - Set a concrete strict target radius: $\epsilon = \frac{\vert{}a - b\vert{}}{2}$. Find thresholds $N_1, N_2$.
    - For all $n \geq \max\{N_1, N_2\}$, apply the Triangle Inequality to split the static distance:  
        $$\vert{}a - b\vert{} = \vert{}(a - a_n) + (a_n - b)\vert{} \leq \underline{\quad\text{(f)}\quad} + \underline{\quad\text{(g)}\quad} < \epsilon + \epsilon = \vert{}a - b\vert{}$$
    - Conclude why the statement $\vert{}a - b\vert{} < \vert{}a - b\vert{}$ resolves the proof.
    
7. Reconstruct the proof that the null space $N(T)$ of a linear map $T: V \to W$ is a structural subspace of the domain space $V$:
    
    - Verify non-emptiness: Since $T(0_V) = 0_W$, the zero vector belongs to the set: $\underline{\quad\text{(h)}\quad} \in N(T)$.
    - Show addition closure: Let $x, y \in N(T)$. This implies $T(x) = 0_W$ and $T(y) = 0_W$.
    - By linearity, evaluate: $T(x + y) = T(x) + T(y) = 0_W + 0_W = \underline{\quad\text{(i)}\quad}$, so $x + y \in N(T)$.
    - Show scalar closure: Let $c \in F$ and $x \in N(T)$. Evaluate: $T(cx) = c T(x) = c(0_W) = \underline{\quad\text{(j)}\quad}$, confirming $cx \in N(T)$.
    

---

## 📅 Day 3

1. State the three equivalent conditions given in Theorem 2.5 for vector spaces of _equal finite dimension_. Why is the requirement of "equal dimension" absolutely vital for these equivalences to hold?
2. According to Theorem 2.6, a linear transformation is uniquely determined by its action on what specific subset of the domain vector space? If two transformations agree on a linearly independent set that does not span $V$, must they be identical?
3. The Corollary to Theorem 2.5 shows that two finite-dimensional vector spaces are isomorphic if and only if they share what numerical trait?
4. If $\beta = \{v_1, \dots, v_n\}$ is a basis for $V$ and $T: V \to W$ is an isomorphism, Theorem 2.2 paired with injectivity characteristics proves that the set $T(\beta) = \{T(v_1), \dots, T(v_n)\}$ forms what special subset structure in $W$?
5. Explain the mathematical principle behind the assertion that changing the first ten thousand terms of a sequence has absolutely no effect on its convergence properties or its limit.
6. Reconstruct the identity showing how the first derivative of an MGF evaluates directly to the distribution mean, $M'(0) = E(X)$:
    
    - By definition of a continuous continuous MGF: $M(t) = \int_{-\infty}^{\infty} e^{tx} f(x) \, dx$.
    - Compute the derivative with respect to $t$ and interchange operators: $M'(t) = \frac{d}{dt} \int_{-\infty}^{\infty} e^{tx} f(x) \, dx = \int_{-\infty}^{\infty} \left( \underline{\quad\text{(k)}\quad} \right) f(x) \, dx$.
    - Evaluate this resultant integral expression explicitly at the point $t = 0$:  
        $$M'(0) = \int_{-\infty}^{\infty} x \cdot e^{0} \cdot f(x) \, dx = \int_{-\infty}^{\infty} \underline{\quad\text{(l)}\quad} \, dx$$
    
7. Reconstruct the proof that if $\beta = \{v_1, \dots, v_n\}$ is a basis for $V$, then $R(T) = \text{span}(T(\beta))$:
    
    - Since each $v_i \in \beta$, $T(v_i) \in R(T)$. Because $R(T)$ is a subspace, it must naturally contain the set: $\underline{\quad\text{(m)}\quad} \subseteq R(T)$.
    - Now let $w \in R(T)$. By definition, there exists a vector $v \in V$ such that $w = \underline{\quad\text{(n)}\quad}$.
    - Represent $v$ through the basis scalars: $v = \sum_{i=1}^n a_i v_i$.
    - Apply the transformation map and expand via linearity to finalize:  
        $$w = T\left(\sum_{i=1}^n a_i v_i\right) = \sum_{i=1}^n a_i T(v_i) \in \underline{\quad\text{(o)}\quad}$$
    

---

## 📅 Day 4

1. Theorem 2.9 asserts that the composition $UT$ of two linear transformations is also a linear transformation. If $T$ is one-to-one and $U$ is _not_ one-to-one, can the composition $UT$ still be one-to-one? Provide a clear constraint.
2. State Theorem 2.11, which defines the matrix representation of a composition: $[UT]_\alpha^\gamma = [U]_\beta^\gamma [T]_\alpha^\beta$. Explain why the matching ordered basis $\beta$ must be shared across the inner dimensions.
3. Theorem 2.12 states that matrix multiplication distributes over addition ($A(B+C) = AB + AC$). What underlying property of functional composition on linear spaces does this matrix theorem reflect?
4. According to Theorem 2.12(c), $I_m A = A = A I_n$ for any $m \times n$ matrix $A$. What is the corresponding identity transformation composition mapping from Section 2.3?
5. State the Monotone Convergence Theorem (Theorem 2.4.2). Give a simple, explicit counterexample of a sequence that is bounded but diverges because it lacks monotonicity.
6. Reconstruct the integral subset partition strategy that bounds probability outcomes via Markov's Inequality:
    
    - Let $u(X)$ be nonnegative, and let $A = \{x : u(x) \geq c\}$ for a positive constant $c$.
    - Separate the integral: $E[u(X)] = \int_{A} u(x)f(x) \, dx + \int_{A^c} u(x)f(x) \, dx$.
    - Drop the complement and state why direction is preserved: $\int_{A^c} u(x)f(x) \, dx \geq \underline{\quad\text{(p)}\quad}$.
    - Within region $A$, bound the function: $\forall x \in A, u(x) \geq \underline{\quad\text{(q)}\quad}$.
    - Complete the step: $E[u(X)] \geq \int_{A} c \cdot f(x) \, dx = c \cdot \underline{\quad\text{(r)}\quad}$.
    
7. Reconstruct the proof that a linear transformation $T$ is one-to-one if and only if $N(T) = \{0\}$:
    
    - $(\implies)$ Assume $T$ is one-to-one. Let $x \in N(T)$. This means $T(x) = \underline{\quad\text{(s)}\quad}$.
    - Since we know $T(0) = 0$, the assumption that $T$ is one-to-one immediately forces $x = 0$.
    - $(\impliedby)$ Assume $N(T) = \{0\}$. Suppose $T(x) = T(y)$.
    - Collect terms on one side and apply linearity: $T(x) - T(y) = \underline{\quad\text{(t)}\quad} = 0$.
    - This shows the vector difference must reside in the set: $(x - y) \in \underline{\quad\text{(u)}\quad}$.
    - Conclude that $x - y = 0$, which yields the final tracking result: $x = y$.
    

---

## 📅 Day 5

1. Theorem 2.13 shows that column $j$ of a matrix product $AB$ can be explicitly represented as a matrix-vector product involving $A$ and a column of $B$. Translate this statement: Column $j$ of $AB$ is a linear combination of which specific set of vectors?
2. State Theorem 2.14, which deals with evaluating an abstract vector mapping: $[T(u)]_\gamma = [T]_\beta^\gamma [u]_\beta$. If you change the vector $u$, does the operator matrix component $[T]_\beta^\gamma$ alter?
3. Theorem 2.12(b) notes $a(AB) = (aA)B = A(aB)$. If we switch to left-multiplication mapping representations via Section 2.3, what property of the scalar multiple of a linear operator transformation ($aT$) does this represent?
4. According to Theorem 2.13(b), the $j$-th column of a matrix $B$ is equal to $B e_j$. If we compose this with left-multiplication maps ($L_B$), what is the coordinates structure of $L_B(e_j)$?
5. State the Cauchy Criterion for Sequences (Theorem 2.6.4). What is the core philosophical advantage of using a Cauchy property over the standard definition of convergence when proving a limit exists?
6. Reconstruct the structural steps proving that every convergent sequence is bounded:
    
    - Assume $(x_n) \to l$. Fix a standard radius choice: $\epsilon = \underline{\quad\text{(v)}\quad}$.
    - There exists an $N \in \mathbb{N}$ such that if $n \geq N$, then $\vert{}x_n - l\vert{} < 1$, implying $\vert{}x_n\vert{} < \underline{\quad\text{(w)}\quad}$.
    - To account for all terms before the index threshold, define the finite maximum:  
        $$M = \max\{ \underline{\quad\text{(x)}\quad}, \vert{}l\vert{}+1 \}$$
    - Conclude why $\vert{}x_n\vert{} \leq M$ holds for all $n \in \mathbb{N}$.
    
7. Reconstruct the independent verification stage from the proof of the Dimension Theorem:
    
    - Let $\{v_1, \dots, v_k\}$ be a basis for $N(T)$, extended to a full basis $\beta = \{v_1, \dots, v_n\}$ for $V$.
    - To show $S = \{T(v_{k+1}), \dots, T(v_n)\}$ is linearly independent, set up: $\sum_{i=k+1}^n b_i T(v_i) = 0$.
    - Pull the scalars inside the operator via linearity: $T\left( \underline{\quad\text{(y)}\quad} \right) = 0$.
    - This forces the vector combination into the kernel set: $\left(\sum_{i=k+1}^n b_i v_i\right) \in \underline{\quad\text{(z)}\quad}$.
    - Thus, express this as a linear combination of the kernel basis: $\sum_{i=k+1}^n b_i v_i = \sum_{i=1}^k c_i v_i$.
    - Equate to zero: $\sum_{i=1}^k (-c_i)v_i + \sum_{i=k+1}^n b_i v_i = 0$. Since $\beta$ is a basis, conclude why $b_i = 0$.
    

---

## 📅 Day 6

1. Theorem 2.15 summarizes the properties of the left-multiplication map $L_A$. If $A$ is an $m \times n$ matrix, state its formal domain and codomain. Under what clear metric condition is $L_A$ guaranteed to be an isomorphism?
2. According to Theorem 2.15(b), $L_A = L_B$ if and only if $A = B$. If two linear maps from $\mathbb{R}^n \to \mathbb{R}^m$ yield identical outputs for all vectors, why does this require their matrix representations to be identical down to the element?
3. Theorem 2.15(d) proves that if $T: F^n \to F^m$ is a linear transformation, there exists a unique matrix $C$ such that $T = L_C$. What is this matrix $C$ explicitly constructed from?
4. Theorem 2.15(f) states $L_{I_n} = I_{F^n}$. How does this solidify the identification of matrix fields with abstract functional mappings under composition?
5. Define what a _peak term_ is within an arbitrary sequence. How does the categorization of whether a sequence contains infinitely many or finitely many peak terms provide a separate, elegant alternative proof of the Bolzano-Weierstrass Theorem?
6. Reconstruct the identity showing that the expectation of a conditional expectation collapses to the absolute marginal mean, $E[E(Y\vert{}X)] = E(Y)$:
    
    - Expand via marginal densities: $E[E(Y\vert{}X)] = \int_{-\infty}^{\infty} \left[ \int_{-\infty}^{\infty} y \frac{f(x, y)}{f_X(x)} \, dy \right] f_X(x) \, dx$.
    - Cancel the matching algebraic density terms from the integrand:  
        $$E[E(Y\vert{}X)] = \int_{-\infty}^{\infty} \int_{-\infty}^{\infty} y \cdot \underline{\quad\text{(aa)}\quad} \, dy \, dx$$
    - Change integration order to isolate $y$: $\int_{-\infty}^{\infty} y \left[ \int_{-\infty}^{\infty} f(x, y) \, dx \right] dy$.
    - Recognize the internal marginal structure to reduce to a single integral loop:  
        $$\int_{-\infty}^{\infty} y \cdot \underline{\quad\text{(bb)}\quad} \, dy = E(Y)$$
    
7. Reconstruct the proof that matrix coordinate evaluation satisfies $[T(u)]_\gamma = [T]_\beta^\gamma [u]_\beta$:
    
    - Fix $u \in V$. Define the linear paths $f: F \to V$ by $f(a) = au$ and $g: F \to W$ by $g(a) = aT(u)$.
    - Let $\alpha = \{1\}$ be the standard ordered basis for the field $F$. Note that composition yields $g = \underline{\quad\text{(cc)}\quad}$.
    - Evaluate via the compositional representation theorem (Theorem 2.11):  
        $$[T(u)]_\gamma = [g(1)]_\gamma = [g]_\alpha^\gamma = [\underline{\quad\text{(dd)}\quad}]_\alpha^\gamma$$
    - Break the composition apart into its independent matrix components to complete the identity:  
        $$[T]_\beta^\gamma [f]_\alpha^\beta = [T]_\beta^\gamma [f(1)]_\beta = [T]_\beta^\gamma [\underline{\quad\text{(ee)}\quad}]_\beta$$
    

---

## 📅 Day 7

1. State Theorem 2.18, which connects operator invertibility to matrix representations. If $[T]_\beta^\gamma$ is invertible, what matrix represents the structural inverse operator $[T^{-1}]_\gamma^\beta$?
2. Theorem 2.17 establishes that if a linear transformation $T$ is invertible, its structural inverse $T^{-1}$ is automatically linear. If you know $T$ is invertible and finite-dimensional, what does the corollary to Theorem 2.17 state about the dimension of the domain versus the codomain?
3. According to the proof of Theorem 2.18, if $T$ is an invertible operator on an $n$-dimensional space $V$, what matrix calculation identity forms the baseline check for $[T^{-1}]_\beta [T]_\beta$?
4. Corollary 2 to Theorem 2.18 establishes that a matrix $A$ is invertible if and only if $L_A$ is invertible. If this holds, what is the operator definition of $(L_A)^{-1}$?
5. State the structural hypothesis required for the Cauchy Condensation Test (Theorem 2.4.6) to remain non-vacuous. Provide a classic series example where the terms tend to zero, yet the test fails because the terms are not monotone decreasing.
6. Reconstruct the parameter scaling that derives Chebyshev's Inequality from Markov's Inequality:
    
    - In Markov's Inequality, map the function and constant choices: set $u(X) = (X - \mu)^2$ and select $c = \underline{\quad\text{(ff)}\quad}$.
    - Substitute these targets directly into the general formula:  
        $$P[(X - \mu)^2 \geq k^2\sigma^2] \leq \frac{E[(X - \mu)^2]}{\underline{\quad\text{(gg)}\quad}}$$
    - Recognize that the numerator expression is the definition of $\underline{\quad\text{(hh)}\quad}$.
    - Simplify the fraction to establish the final metric: $P(\vert{}X - \mu\vert{} \geq k\sigma) \leq \frac{1}{k^2}$.
    
7. Reconstruct the operator composition steps proving that matrix multiplication is associative, $A(BC) = (AB)C$:
    
    - Map the matrix multiplication to its matching left-multiplication transformation: $L_{A(BC)} = \underline{\quad\text{(ii)}\quad}$.
    - Apply the composition property of transformations (Theorem 2.15e): $L_A L_{BC} = L_A ( \underline{\quad\text{(jj)}\quad} )$.
    - Invoke the associative property of functional composition: $(L_A L_B) L_C$.
    - Convert this combined operator term back into its single matrix product format:  
        $$(L_A L_B) L_C = L_{AB} L_C = L_{\underline{\quad\text{(kk)}\quad}}$$
    - Apply the uniqueness of left-multiplication matrices (Theorem 2.15b) to conclude that the matrix inputs must be equal.


---

## 📅 Day 1 Solutions

## 1. Friedberg (Subspace Properties)

- Solution: $T(0_V) = 0_W$ because $T(0_V) = T(0 \cdot 0_V) = 0 \cdot T(0_V) = 0_W$.
- Explanation: This follows directly from the definition of linearity under scalar multiplication, where pulling out the scalar 0 ∈ F maps any vector product to the zero element of the codomain space.

## 2. Friedberg (Spanning Images)

- Solution: No. T(β) will span R(T) if and only if β spans V.
- Explanation: If β does not span V, there exists a vector x ∈ V outside span(β). If T(x) is not contained within $\text{span}(T(\beta))$, then T(β) fails to cover the full image space R(T).

## 3. Friedberg (Matrix Properties)

- Solution: Yes, the matrix equation still holds, but the individual matrix components will change.
- Explanation: Permuting the ordering of the basis elements in β systematically shuffles the column locations of both $[T]_\beta^\gamma$ and $[U]_\beta^\gamma$. Because the shuffling is identical for both operators, their sum remains perfectly preserved.

## 4. Friedberg (Linearity of Combinations)

- Solution: It acts as the unique additive identity (zero vector) of the vector space $\mathcal{L}(V, W)$.
- Explanation: For any linear transformation $T \in \mathcal{L}(V, W)$, $(T + T_0)(v) = T(v) + T_0(v) = T(v) + 0_W = T(v)$ for all vectors v ∈ V.

## 5. Abbott (Rearrangement Definition)

- Solution: A rearrangement of $\sum_{n=1}^\infty a_n$ is a series $\sum_{n=1}^\infty a_{f(n)}$, where $f: \mathbb{N} \to \mathbb{N}$ is a bijection. The overarching criterion is absolute convergence. If a series converges absolutely, any rearrangement yields the exact same sum. If it converges conditionally, rearrangements can alter the sum to any real number (Riemann's Rearrangement Theorem).

## 6. Proof 1: Statistical Variance Shorthand

- (a) 2μ X
- (b) E(X)
- Full Step Verification:  
    $$\text{Var}(X) = E[X^2 - 2\mu X + \mu^2] = E(X^2) - 2\mu E(X) + \mu^2 = E(X^2) - 2\mu(\mu) + \mu^2 = E(X^2) - \mu^2$$

## 7. Proof 2: Range Spaces (Friedberg Theorem 2.1)

- (c) $0_W$
- (d) T(v + w)
- (e) T(cv)

---

## 📅 Day 2 Solutions

## 1. Friedberg (Dimension Theorem)

- Solution: $\text{nullity}(T) + \text{rank}(T) = \dim(V)$. If $T: \mathbb{R}^5 \to \mathbb{R}^3$ is surjective, $\text{rank}(T) = \dim(\mathbb{R}^3) = 3$. Therefore, nullity(T) = 5 - 3 = 2.

## 2. Friedberg (Injectivity Characterization)

- Solution: $N(T) = \{0_V\}$. No, if a function is non-linear, a trivial kernel does not guarantee injectivity.
- Explanation: For example, the non-linear function f(x) = x² maps only 0 to 0 on $\mathbb{R}$, yet f(-2) = f(2) = 4, making it non-injective. Trivial kernels only characterize injectivity when linear structural preservation holds.

## 3. Friedberg (Matrix Size Constants)

- Solution: Because matrix-vector operations map an input column vector to an output column vector via the equation $[T(v)]_\gamma = [T]_\beta^\gamma [v]_\beta$.
- Explanation: To convert an n × 1 coordinate matrix into an m × 1 output matrix, the transformation matrix must have exactly m rows and n columns to satisfy structural matrix multiplication rules.

## 4. Friedberg (Rank Constraints)

- Solution: No. By the Dimension Theorem, $\text{rank}(T) = \dim(V) - \text{nullity}(T) \leq \dim(V)$. If $\dim(V) < \dim(W)$, then $\text{rank}(T) < \dim(W)$, which mathematically prevents the image space from matching the size of the codomain.

## 5. Abbott (Topological Thresholds)

- Solution: $V_\epsilon(a) = \{x \in \mathbb{R} : \vert{}x - a\vert{} < \epsilon\}$. Convergence rephrased: A sequence $(a_n)$ converges to a if, for every open neighborhood $V_\epsilon(a)$, all but a finite number of the terms of the sequence are trapped inside $V_\epsilon(a)$.

## 6. Proof 1: Uniqueness of Analysis Limits (Abbott Theorem 2.2.7)

- (f) $\vert{}a_n - a\vert{}$
- (g) $\vert{}a_n - b\vert{}$
- Full Step Verification: The absolute triangle breakout forces $\vert{}a - b\vert{} \leq \vert{}a - a_n\vert{} + \vert{}a_n - b\vert{} < \frac{\vert{}a-b\vert{}}{2} + \frac{\vert{}a-b\vert{}}{2} = \vert{}a-b\vert{}$. The statement |a-b| < |a-b| is a flat logical impossibility, proving the limits cannot be distinct.

## 7. Proof 2: Null Spaces (Friedberg Theorem 2.1)

- (h) $0_V$
- (i) $0_W$
- (j) $0_W$

---

## 📅 Day 3 Solutions

## 1. Friedberg (Finite-Dimensional Equivalence)

- Solution: The three conditions are: (1) T is one-to-one, (2) T is onto, (3) $\text{rank}(T) = \dim(V)$.
- Explanation: If dimensions are not equal, an operator can easily be injective without being surjective (e.g., embedding $\mathbb{R}^2$ into $\mathbb{R}^3$) or surjective without being injective (e.g., projecting $\mathbb{R}^3$ onto $\mathbb{R}^2$).

## 2. Friedberg (Basis Determination)

- Solution: An ordered basis β. No, they do not have to be identical.
- Explanation: If two transformations match on a linearly independent set that does not span the space, they can diverge completely on any vectors outside that span, since those outside elements cannot be built from the matched set.

## 3. Friedberg (Isomorphism Dimensions)

- Solution: $\dim(V) = \dim(W)$.
- Explanation: Two finite-dimensional vector spaces over the same field are isomorphic if and only if their dimensions are structurally identical.

## 4. Friedberg (Basis Transformations)

- Solution: An ordered basis for the target space W.
- Explanation: Isomorphisms map bases to bases because they preserve both linear independence and spanning parameters across vector systems.

## 5. Abbott (The Limit Tail)

- Solution: Convergence is an asymptotic property dictated entirely by the "tail" of the sequence (n → ∞). Altering a finite number of starting terms changes the initial index threshold N for a chosen ε, but it does not change the fact that a valid structural cutoff index N exists.

## 6. Proof 1: Moment Generation Derivatives

- (k) $\frac{d}{dt}(e^{tx}) = x e^{tx}$
- (l) x f(x)

## 7. Proof 2: Direct Spanning Maps (Friedberg Theorem 2.2)

- (m) $\text{span}(T(\beta))$
- (n) T(v)
- (o) $\text{span}(T(\beta))$

---

## 📅 Day 4 Solutions

## 1. Friedberg (Composition Linearity)

- Solution: No. The composition UT can never be one-to-one if U is not one-to-one on the range space R(T).
- Explanation: If U maps two distinct vectors w₁, w₂ ∈ R(T) to the same output, and there exist v₁, v₂ ∈ V such that T(v₁) = w₁ and T(v₂) = w₂, then UT(v₁) = UT(v₂), which violates injectivity.

## 2. Friedberg (Composition Matrix Representations)

- Solution: $[UT]_\alpha^\gamma = [U]_\beta^\gamma [T]_\alpha^\beta$. The shared basis β must match exactly because the output coordinates of T (evaluated relative to β) must serve directly as the entry inputs for the outer operator U.

## 3. Friedberg (Distributive Multiplications)

- Solution: It reflects the linear distribution property of functional mappings over vector additions: U(T₁ + T₂) = UT₁ + UT₂ and (U₁ + U₂)T = U₁T + U₂T.

## 4. Friedberg (Identity Multiplications)

- Solution: $I_W T = T = T I_V$, where $I_V$ and $I_W$ represent the identity transformations on the domain and codomain vector spaces, respectively.

## 5. Abbott (Monotone Convergence)

- Solution: If a sequence is monotone and bounded, it converges. Counterexample: $a_n = (-1)^n$. This sequence is bounded ($\vert{}a_n\vert{} \leq 1$), but it diverges by oscillating continually between -1 and 1 due to its lack of monotonicity.

## 6. Proof 1: Expectation Partition Bounding (Markov's Inequality)

- (p) 0 (or $\int_{A^c} u(x)f(x)\,dx \geq 0$)
- (q) c
- (r) $P[u(X) \geq c]$

## 7. Proof 2: Injectivity and Kernel Triviality (Friedberg Theorem 2.4)

- (s) $0_W$
- (t) T(x - y)
- (u) N(T)

---

## 📅 Day 5 Solutions

## 1. Friedberg (Column Transformations)

- Solution: A linear combination of the columns of matrix A.
- Explanation: Specifically, column j of AB is the weighted vector combination $\sum_{i} B_{ij} A_{*,i}$, where the scalars are drawn from column j of matrix B.

## 2. Friedberg (Vector Representation Maps)

- Solution: No, the matrix representation $[T]_\beta^\gamma$ remains completely constant.
- Explanation: The matrix is defined entirely by how the transformation maps the static base vectors of β into the coordinate frameworks of γ. Changing u only updates the coordinate column inputs and outputs ($[u]_\beta$ and $[T(u)]_\gamma$).

## 3. Friedberg (Scalar Matrix Multiples)

- Solution: It represents the scalar scaling properties of transformation composition: a(UT) = (aU)T = U(aT).

## 4. Friedberg (Column Index Extraction)

- Solution: $L_B(e_j)$ evaluates directly to the j-th column vector of matrix B.
- Explanation: Multiplying a matrix by the j-th standard basis vector isolates and extracts that specific column.

## 5. Abbott (The Intrinsic Cauchy State)

- Solution: A sequence converges if and only if it is a Cauchy sequence. The philosophical advantage is that the Cauchy criterion allows you to prove convergence by analyzing the internal behavior of the sequence terms relative to one some other, without requiring prior knowledge of the actual limit value.

## 6. Proof 1: Boundedness of Convergent Real Sequences (Abbott Theorem 2.3.2)

- (v) 1 (Choosing ε = 1)
- (w) |l| + 1
- (x) $\{\vert{}x_1\vert{}, \vert{}x_2\vert{}, \dots, \vert{}x_{n-1}\vert{}\}$

## 7. Proof 2: Extension Independence Bases (Friedberg Theorem 2.3)

- (y) $\sum_{i=k+1}^n b_i v_i$
- (z) N(T)

---

## 📅 Day 6 Solutions

## 1. Friedberg (Left-Multiplication Properties)

- Solution: Domain: $F^n$, Codomain: $F^m$. $L_A$ is guaranteed to be an isomorphism if and only if A is a square (n = n) invertible matrix.

## 2. Friedberg (Unique Left Multiplications)

- Solution: Because the columns of A and B are determined by evaluating the mappings at the standard basis vectors ($A_{*,j} = L_A(e_j)$ and $B_{*,j} = L_B(e_j)$). If $L_A(v) = L_B(v)$ for all vectors, then $L_A(e_j) = L_B(e_j)$ for all components, forcing every column to match perfectly.

## 3. Friedberg (Linear Operator Maps)

- Solution: The columns of matrix C are the coordinate vector outputs obtained by evaluating the transformation T at each standard basis vector of the domain: $C = \left( T(e_1) \;\vert{}\; T(e_2) \;\vert{}\; \dots \;\vert{}\; T(e_n) \right)$.

## 4. Friedberg (Identity Left Operators)

- Solution: It confirms that the identity matrix acts as a functional identity operator under mapping composition, meaning matrix multiplication aligns with function composition.

## 5. Abbott (The Peak Term Subsequence)

- Solution: A term $a_m$ is a peak term if $a_m \geq a_n$ for all n > m. If a sequence has infinitely many peaks, they form a monotone decreasing subsequence. If it has finitely many peaks, you can construct a monotone increasing subsequence from the remaining terms. Since any bounded monotone sequence converges, this guarantees a convergent subsequence exists.

## 6. Proof 1: Bivariate Iterated Expectation Loop

- (aa) f(x, y)
- (bb) $f_Y(y)$

## 7. Proof 2: Matrix Coordinates Evaluation (Friedberg Theorem 2.14)

- (cc) Tf
- (dd) Tf
- (ee) u

---

## 📅 Day 7 Solutions

## 1. Friedberg (Matrix Invertibility Operators)

- Solution: The matrix inverse of the forward representation: $[T^{-1}]_\gamma^\beta = \left( [T]_\beta^\gamma \right)^{-1}$.

## 2. Friedberg (Inverse Map Linearity)

- Solution: It states that if V and W are finite-dimensional vector spaces, then V is isomorphic to W if and only if $\dim(V) = \dim(W)$.

## 3. Friedberg (Identity Representations)

- Solution: $[T^{-1}]_\beta^\gamma [T]_\beta^\gamma = I_n$, where $I_n$ represents the n × n identity matrix.

## 4. Friedberg (Left-multiplication Inverses)

- Solution: $(L_A)^{-1} = L_{A^{-1}}$. The inverse of a left-multiplication operator matches left-multiplication by the inverse matrix.

## 5. Abbott (The Condensate Test)

- Solution: The sequence of terms $(a_n)$ must be positive and monotone decreasing ($a_1 \geq a_2 \geq a_3 \geq \dots \geq 0$). Counterexample: $a_n = \frac{(-1)^n}{n}$. This series converges conditionally, but the condensation test cannot be applied directly because the terms oscillate and are not monotone decreasing.

## 6. Proof 1: Variance Dispersion Metrics (Chebyshev's Inequality)

- (ff) k²σ²
- (gg) k²σ²
- (hh) σ² (or Var(X))

## 7. Proof 2: Associativity Matrices (Friedberg Theorem 2.16)

- (ii) $L_A L_{BC}$
- (jj) $L_B L_C$
- (kk) (AB)C

---

To ensure your review schedule is optimized for your goals, consider these strategic follow-up steps:

- Would you like me to create an applied calculations worksheet computing specific matrices and coordinates to test how you apply these theorems?
- Do you want to add an extra day of retrieval questions explicitly covering Friedberg Section 2.5 (Change of Coordinate Matrix)?
- Should we design a diagnostic scoring matrix to help you isolate whether any remaining gaps are in matrix mechanics or real analysis topology?