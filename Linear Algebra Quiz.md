

## 📅 Day 1: Basis Mechanics & Dimension Subsets (Sec 1.6)

## 📝 Structural Mechanics

- Q1.1: Reconstruct the Theorem 1.8 vector deletion algorithm (friedberg_... p. 6). If a finite set $G$ generates a vector space $V$, detail the exact sequential path used to trim elements from $G$ to form a basis (friedberg_... p. 6). Which precise dependency criterion dictates whether a vector can be safely removed without altering the span?
- Q1.2: If $W$ is a subspace of a finite-dimensional vector space $V$, Theorem 1.11 establishes that $\dim(W) \leq \dim(V)$ (friedberg_... p. 6). Construct a precise counterexample showing why the second clause of this theorem ($\dim(W) = \dim(V) \implies W = V$) completely collapses if $V$ is an infinite-dimensional vector space.
- Q1.3: When extending a linearly independent subset $I$ of a finite-dimensional space $V$ by extracting vectors from a known generating set $G$, what explicit structural containment condition prevents a particular vector $v \in G$ from being appended to $I$?

## 📜 Non-Major Theorem Recall

- T1.1 (Theorem 1.8 - Generating Subset Reduction): State Theorem 1.8 exactly as presented (friedberg_... p. 6). If the original generating set $G$ contains the zero vector $0$, trace how the mechanical loop of the theorem handles its presence and eventual elimination.
- T1.2 (Theorem 1.11 Corollary - Subspace Basis Extension): State the corollary asserting that any basis for a subspace $W$ can be extended to a basis for the parent space $V$. If $W = \{0\}$ (the trivial zero subspace), outline how this extension process interacts with a known ordered basis for $V$.
- T1.3 (Theorem 1.9 Corollary 2 - The Exact Dimension Basis Shortcut): State the corollary establishing that if $\dim(V) = n$, any linearly independent set containing exactly $n$ vectors is automatically a basis. Explain why this property fails to hold if the subset contains $n+1$ vectors.

---

## 📅 Day 2: Mapping Formulations & Range Spans (Sec 2.1–2.2)

## 📝 Structural Mechanics

- Q2.1: Let $T: V \to W$ be a linear transformation (friedberg_... p. 6). If $\beta$ is a linearly independent subset of $V$ that does _not_ span $V$, Theorem 2.5 analyzes range generation (friedberg_... p. 6). What exact containment relationship holds between the subspace $\text{span}(T(\beta))$ and the true range $\text{R}(T)$ (friedberg_... p. 6)?
- Q2.2: In Theorem 2.4, a unique linear transformation is constructed by defining arbitrary target values on a basis (friedberg_... p. 6). Why does this uniqueness guarantee fail if the target vectors are assigned to a domain subset that is merely linearly independent instead of a full basis?

## 📜 Non-Major Theorem Recall

- T2.1 (Theorem 2.4 - Linear Map Existence and Uniqueness): State Theorem 2.4 exactly (friedberg_... p. 6). What does the theorem assert if all the arbitrarily chosen target vectors $w_1, w_2, \dots, w_n \in W$ are selected to be the zero vector $0 \in W$?
- T2.2 (Theorem 2.5 - Range of a Spanning Set): State Theorem 2.5 regarding the image of a generating set (friedberg_... p. 6). Use this theorem to prove why the nullity of a zero transformation must equal the full dimension of its domain space.

---

## 📅 Day 3: Identity Operators & Change of Basis Mappings (Sec 2.3–2.5)

## 📝 Structural Mechanics

- Q3.1: Theorem 2.11 notes that $[I_V]_\beta = I_n$ (friedberg_... p. 6). If the ordered basis on the left is altered to a different ordering or a completely distinct basis $\beta'$ while the right remains $\beta$, explain why the matrix representation fails to be the identity matrix $I_n$ (friedberg_... p. 6).
- Q3.2: Let $Q = [I_V]_{\beta'}^\beta$ be a change of coordinate matrix (friedberg_... p. 6). If $v \in V$ is a vector whose coordinate vector under $\beta'$ is the elementary standard vector $e_1$, what does the product $Q e_1$ explicitly isolate among the columns of $Q$?

## 📜 Non-Major Theorem Recall

- T3.1 (Theorem 2.11 - Identity Representation Mechanics): State Theorem 2.11 exactly (friedberg_... p. 6). How does this theorem ensure that composing any operator $T$ with the identity map preserves its matrix coordinates?
- T3.2 (Theorem 2.18 - Vector Space Isomorphism Criteria): State Theorem 2.18 relating functional isomorphisms between spaces to matrix invertibility (friedberg_... p. 6). If $\dim(V) \neq \dim(W)$, explain why the matrix representation of a mapping between them cannot be invertible (friedberg_... p. 6).
- T3.3 (Theorem 2.22 - Change of Coordinates Inversion): State Theorem 2.22 concerning coordinate changes (friedberg_... p. 6). Use the composition property of identity maps to prove that $Q^{-1} = [I_V]_\beta^{\beta'}$ (friedberg_... p. 6).

---

## 📅 Day 4: Range Inclusions & Operator Product Ranks (Sec 3.1–3.2)

## 📝 Structural Mechanics

- Q4.1: Show how the linear map range inclusion $\text{R}(L_A L_B) \subseteq \text{R}(L_A)$ directly leads to the product rank bound $\text{rank}(AB) \leq \text{rank}(A)$ from Theorem 3.4 (friedberg_... p. 7).

## 📜 Non-Major Theorem Recall

- T4.1 (Theorem 3.2 - Elementary Inverses): State Theorem 3.2 regarding elementary matrix inverses (friedberg_... p. 7). How does the type of row operation executed relate to the type of its corresponding inverse matrix (friedberg_... p. 7)?
- T4.2 (Theorem 3.4 - Product Rank Bounds): State Theorem 3.4 bounding the rank of a matrix product (friedberg_... p. 7). If $A$ is an $n \times 1$ column vector and $B$ is a $1 \times n$ row vector, what is the maximum possible rank of $AB$?

---

## 📅 Day 5: Solution Set Structure & Surjectivity Conditions (Sec 3.2–3.3)

## 📝 Structural Mechanics

- Q5.1: Theorem 3.6 asserts that multiplying by invertible matrices preserves rank ($\text{rank}(PAQ) = \text{rank}(A)$) (friedberg_... p. 7). Why does this fail to hold if $P$ or $Q$ has a non-trivial null space?
- Q5.2: If a matrix $A \in \text{M}_{m\times n}(F)$ has $\text{rank}(A) = m$, Theorem 3.9 ensures $Ax = b$ is consistent for all $b$ (friedberg_... p. 7). Translate this into the mapping vocabulary of Chapter 2 regarding surjectivity (friedberg_... pp. 6-7).
- Q5.3: Let $Ax = 0$ be a homogeneous system (friedberg_... p. 7). If $\text{rank}(A) = r$, Theorem 3.11 fixes the solution space dimension at $n-r$ (friedberg_... p. 7). Map this result directly to the Rank-Nullity theorem using the operator $L_A$ (friedberg_... pp. 6-7).

## 📜 Non-Major Theorem Recall

- T5.1 (Theorem 3.6 - Invertible Multiplication Invariance): State Theorem 3.6 exactly (friedberg_... p. 7). If an operator multiplies a matrix on both sides by non-invertible operators, what inequality bounds the resulting rank?
- T5.2 (Theorem 3.9 - Full Row Rank Consistency): State Theorem 3.9 regarding consistency conditions (friedberg_... p. 7). What does this theorem imply about the existence of free variables if $n > m$?
- T5.3 (Theorem 3.11 - Homogeneous System Dimensions): State Theorem 3.11 governing homogeneous spaces (friedberg_... p. 7). If a system has 5 variables and a coefficient matrix of rank 3, what is the dimension of its solution space?

---

## 📅 Day 6: Echelon Uniqueness & Equivalence of Systems (Sec 3.4)

## 📝 Structural Mechanics

- Q6.1: Theorem 3.14 notes the uniqueness of the reduced row echelon form (RREF) (friedberg_... p. 7). Explain how the location of pivot columns in the RREF maps to the linear independence behavior of the columns in the original matrix.
- Q6.2: Theorem 3.16 links matrix invertibility to the identity matrix $I_n$ via RREF (friedberg_... p. 7). If an $n \times n$ matrix reduces to a form with a zero row on the bottom, what does this tell you about its rank?

## 📜 Non-Major Theorem Recall

- T6.1 (Theorem 3.14 - RREF Uniqueness): State Theorem 3.14 regarding row echelon forms (friedberg_... p. 7). Why is uniqueness lost if we omit the requirement that the first non-zero entry of each row must equal 1?
- T6.2 (Theorem 3.16 - Invertibility RREF Characterization): State Theorem 3.16 exactly (friedberg_... p. 7). If a matrix is not invertible, what is the maximum number of pivot elements its RREF can contain?
- T6.3 (Theorem 3.15 - Equivalence of Systems): State the theorem clarifying that row operations preserve solution sets (friedberg_... p. 7). If a system is inhomogeneous, why must the operations be performed identically on the vector $b$?

---

Here is the high-density, abstract algebra-focused key. It explicitly references Friedberg's core architecture, omitting computational coordinate shuffling.

---

## 📅 Day 1: Basis Mechanics & Dimension Subsets (Sec 1.6)

## 📝 Structural Mechanics

## Q1.1: Reconstruct the Theorem 1.8 vector deletion algorithm.

- Solution: Let $G$ generate $V$. If $G$ is linearly dependent, Theorem 1.7 (Sec 1.5) guarantees $\exists v \in G$ such that $v \in \text{span}(G \setminus \{v\})$. Let $G' = G \setminus \{v\}$. By Theorem 1.5 (Sec 1.4), $\text{span}(G') = \text{span}(G) = V$. Iterating this removal preserves the spanning property. Because $G$ is finite, the loop terminates when no dependent elements remain, yielding a basis.
- Text Location: Section 1.6, Theorem 1.8 (p. 43).

## Q1.2: Infinite-dimensional counterexample to Theorem 1.11.

- Solution: Let $V = \text{P}(\mathbb{R})$ with basis $\beta = \{1, x, x^2, \dots\}$, so $\dim(V) = \infty$. Define proper subspace $W = \{f(x) \in \text{P}(\mathbb{R}) : f(0) = 0\} = \text{span}(\{x, x^2, \dots\})$. $W$ has basis $\{x, x^2, \dots\}$, so $\dim(W) = \infty$. Thus $\dim(W) = \dim(V) = \infty$, but $W \neq V$ since $1 \in V \setminus W$.
- Text Location: Section 1.6, Theorem 1.11 (p. 48).

## Q1.3: Constraint preventing extension of an independent set.

- Solution: Theorem 1.6 (Sec 1.5) establishes that $I \cup \{v\}$ is linearly independent if and only if $v \notin \text{span}(I)$. Therefore, the exact constraint blocking inclusion is $v \in \text{span}(I)$.
- Text Location: Section 1.6, Corollary 1 to Theorem 1.11 context (p. 48).

## 📜 Non-Major Theorem Recall

## T1.1: Theorem 1.8 (Generating Subset Reduction)

- Statement: Any finite generating set $G$ of a vector space $V$ contains a subset that is a basis for $V$.
- Zero Vector Action: The zero vector satisfies $1 \cdot 0 = 0$, violating linear independence. By Theorem 1.7 (Sec 1.5), $0 \in \text{span}(G \setminus \{0\})$. Thus, the deletion engine removes $0$ in the first iteration without reducing the span (Theorem 1.5, Sec 1.4).
- Text Location: Section 1.6, Theorem 1.8 (p. 43).

## T1.2: Theorem 1.11 Corollary (Subspace Basis Extension)

- Statement: Every linearly independent subset of a finite-dimensional vector space $V$ can be extended to a basis for $V$.
- Trivial Subspace $W=\{0\}$ Interaction: The basis for $W$ is $\emptyset$. The algorithm starts with $\emptyset$. Given ordered basis $\beta = \{v_1, \dots, v_n\}$ for $V$, the engine tests each $v_i$. Since $\text{span}(\emptyset) = \{0\}$ and $v_1 \neq 0$, $v_1$ is appended via Theorem 1.6 (Sec 1.5). Inductively, every $v_i \notin \text{span}(\{v_1, \dots, v_{i-1}\})$, fully reconstructing $\beta$.
- Text Location: Section 1.6, Corollary 1 to Theorem 1.11 (p. 48).

## T1.3: Theorem 1.9 Corollary 2 (Dimension Basis Shortcut)

- Statement: If $\dim(V) = n$, any linearly independent subset of $V$ containing exactly $n$ vectors is a basis.
- Failure at $n+1$ vectors: The Replacement Theorem (Theorem 1.9) states that if $V$ is generated by $n$ vectors, no independent subset can exceed size $n$. Since $\dim(V)=n$, the maximal size of any independent set is $n$; thus, $n+1$ vectors must be dependent.
- Text Location: Section 1.6, Corollary 2 to Theorem 1.9 (p. 47).

---

## 📅 Day 2: Mapping Formulations & Range Spans (Sec 2.1–2.2)

## 📝 Structural Mechanics

## Q2.1: Containment relation when domain basis properties fail.

- Solution: By definition, $\text{R}(T) = \{T(v) : v \in V\}$. Since $\text{span}(\beta) \subsetneq V$, $\exists u \in V \setminus \text{span}(\beta)$. The set containment is strictly $\text{span}(T(\beta)) \subseteq \text{R}(T)$ because $T(u)$ is in $\text{R}(T)$ but its containment in $\text{span}(T(\beta))$ is not guaranteed.
- Text Location: Section 2.1, Theorem 2.5 infrastructure (p. 68).

## Q2.2: Loss of unique map construction on non-spanning independent sets.

- Solution: If $S = \{v_1, \dots, v_k\}$ is independent but does not span, Theorem 1.11 Corollary (Sec 1.6) extends it to a basis $\beta = S \cup \{u_{k+1}, \dots, u_n\}$. Theorem 2.4 requires specifying target images for all basis vectors. Assigning different values to $\{T(u_j)\}$ creates distinct transformations that match on $S$, destroying uniqueness.
- Text Location: Section 2.1, Theorem 2.4 framework (p. 67).

## 📜 Non-Major Theorem Recall

## T2.1: Theorem 2.4 (Linear Map Existence and Uniqueness)

- Statement: Let $\beta=\{v_1, \dots, v_n\}$ be a basis for $V$. For any vectors $\{w_1, \dots, w_n\} \subseteq W$, $\exists ! T: V \to W$ such that $T(v_i) = w_i$.
- Zero Vector Targets: When $w_i = 0$ $\forall i$, the unique map is the zero transformation ($T_0$), since linearity requires $T(\sum c_i v_i) = \sum c_i T(v_i) = 0$.
- Text Location: Section 2.1, Theorem 2.4 (p. 67).

## T2.2: Theorem 2.5 (Range of a Spanning Set)

- Statement: If $\beta = \{v_1, \dots, v_n\}$ spans $V$, then $\text{R}(T) = \text{span}(\{T(v_1), \dots, T(v_n)\})$.
- Zero Operator Nullity Proof: For $T_0$, $T_0(v_i) = 0$ $\forall v_i \in \beta$. Theorem 2.5 states $\text{R}(T_0) = \text{span}(\{0\}) = \{0\}$, so $\text{rank}(T_0) = 0$. The Dimension Theorem (Rank-Nullity, Theorem 2.3) states $\text{rank}(T_0) + \text{nullity}(T_0) = \dim(V)$, yielding $\text{nullity}(T_0) = \dim(V)$.
- Text Location: Section 2.1, Theorem 2.5 (p. 68).

---

## 📅 Day 3: Identity Operators & Change of Basis Mappings (Sec 2.3–2.5)

## 📝 Structural Mechanics

## Q3.1: Why change-of-basis matrix representations fail to equal $I_n$.

- Solution: The $j$-th column of $[I_V]_{\beta'}^\beta$ is the coordinate vector $[I_V(v_j')]_\beta = [v_j']_\beta$, where $v_j' \in \beta'$. Since $\beta' \neq \beta$, $v_j'$ is generally a non-trivial linear combination of multiple vectors in $\beta$, creating non-zero off-diagonal entries.
- Text Location: Section 2.5, Change of Coordinates (p. 111).

## Q3.2: Column isolation mechanics via elementary standard coordinates.

- Solution: Let $Q = [I_V]_{\beta'}^\beta$. By matrix multiplication design, $Q e_1$ computes a linear combination of the columns of $Q$ using the entries of $e_1 = (1, 0, \dots, 0)^t$ as weights. This isolates the first column of $Q$, which represents $[v_1']_\beta$.
- Text Location: Section 2.5, Theorem 2.22 matrix mechanics (p. 112).

## 📜 Non-Major Theorem Recall

## T3.1: Theorem 2.11 (Identity Representation)

- Statement: For any finite-dimensional space $V$ with ordered basis $\beta$, $[I_V]_\beta = I_n$.
- Coordinate Preservation: Given $T: V \to V$, the composition is $I_V \circ T = T$. By Theorem 2.11 (Sec 2.3), $[I_V \circ T]_\beta = [I_V]_\beta [T]_\beta = I_n [T]_\beta = [T]_\beta$. The matrix identity $I_n$ acts as the identity element in the ring $\text{M}_{n\times n}(F)$.
- Text Location: Section 2.3, Theorem 2.11 (p. 81).

## T3.2: Theorem 2.18 (Operator Isomorphism Criteria)

- Statement: Finite-dimensional spaces $V$ and $W$ over $F$ are isomorphic $\iff \dim(V) = \dim(W)$.
- Dimension Mismatch Rectangularity: If $\dim(V) \neq \dim(W)$, any matrix representation $[T]_\beta^\gamma$ is non-square ($m \times n$ where $m \neq n$). In matrix algebra, invertibility is strictly defined for square matrices; non-square transformations cannot hold a two-sided inverse, mirroring the fact that no bijective linear map can link spaces of unequal dimension.
- Text Location: Section 2.4, Theorem 2.18 (p. 102).

## T3.3: Theorem 2.22 (Change of Coordinates Inversion)

- Statement: If $Q = [I_V]_{\beta'}^\beta$, then $Q$ is invertible and $Q^{-1} = [I_V]_\beta^{\beta'}$.
- Proof via Composition: Because $I_V \circ I_V = I_V$, applying Theorem 2.11 (Sec 2.3) yields $[I_V \circ I_V]_\beta^\beta = [I_V]_{\beta'}^\beta [I_V]_\beta^{\beta'} \implies I_n = Q [I_V]_\beta^{\beta'}$. By uniqueness of the inverse element in a matrix group, $[I_V]_\beta^{\beta'} = Q^{-1}$.
- Text Location: Section 2.5, Theorem 2.22 (p. 112).

---

## 📅 Day 4: Range Inclusions & Operator Product Ranks (Sec 3.1–3.2)

## 📝 Structural Mechanics

## Q4.1: Range inclusion mapping to matrix product rank inequalities.

- Solution: By definition, $\text{R}(L_{AB}) = \text{R}(L_A L_B) = \{L_A(L_B(x)) : x \in F^n\}$. Since every vector is an image under $L_A$, $\text{R}(L_A L_B) \subseteq \text{R}(L_A)$. By Theorem 1.11 (Sec 1.6), a subspace containment implies a dimension inequality: $\dim(\text{R}(L_{AB})) \leq \dim(\text{R}(L_A))$. Since rank is defined as range dimension, $\text{rank}(AB) \leq \text{rank}(A)$.
- Text Location: Section 3.2, Theorem 3.4 proof mechanics (p. 153).

## 📜 Non-Major Theorem Recall

## T4.1: Theorem 3.2 (Elementary Inverses)

- Statement: Every elementary matrix is invertible, and its inverse is an elementary matrix of the same type.
- Operation Type Preservation: The inverse reverses the geometric transformation: Type 1 (row swap) is its own inverse; Type 2 (row scaling by $c \neq 0$) has inverse scaling by $\frac{1}{c}$; Type 3 (adding $c \cdot \text{row } j$ to $\text{row } i$) has inverse adding $-c \cdot \text{row } j$ to $\text{row } i$. All operations maintain their structural class.
- Text Location: Section 3.1, Theorem 3.2 (p. 150).

## T4.2: Theorem 3.4 (Product Rank Bounds)

- Statement: If $AB$ is defined, $\text{rank}(AB) \leq \text{rank}(A)$ and $\text{rank}(AB) \leq \text{rank}(B)$.
- Outer Product Limit: Let $A$ be $n \times 1$ and $B$ be $1 \times n$. Since $\dim(\text{columns}(A)) = 1$, $\text{rank}(A) \leq 1$. Similarly, $\text{rank}(B) \leq 1$. By Theorem 3.4, $\text{rank}(AB) \leq \min(\text{rank}(A), \text{rank}(B)) \leq 1$. The outer product matrix has an absolute maximum rank of $1$.
- Text Location: Section 3.2, Theorem 3.4 (p. 153).

---

## 📅 Day 5: Solution Set Structure & Surjectivity Conditions (Sec 3.2–3.3)

## 📝 Structural Mechanics

## Q5.1: Failure of rank preservation under non-invertible multiplications.

- Solution: If $P$ or $Q$ is non-invertible, they possess non-trivial kernels ($\text{N}(L_P) \neq \{0\}$ or $\text{N}(L_Q) \neq \{0\}$). left-multiplication by $P$ can map vectors in $\text{R}(A)$ to zero, compressing the image space. Right-multiplication by $Q$ restricts the effective domain to a proper subspace of $F^n$, preventing the full span of columns from being reached.
- Text Location: Section 3.2, Theorem 3.6 boundary conditions (p. 156).

## Q5.2: Row rank consistency translated to surjective mappings.

- Solution: The system $Ax = b$ ($A \in \text{M}_{m\times n}(F)$) is consistent $\forall b \in F^m \iff L_A: F^n \to F^m$ is surjective. Full row rank means $\text{rank}(A) = \dim(\text{R}(L_A)) = m$. Since $\dim(F^m) = m$, the image space must equal the codomain ($\text{R}(L_A) = F^m$), ensuring every target vector has a valid pre-image.
- Text Location: Section 3.3, Theorem 3.9 transformation meaning (p. 172).

## Q5.3: Mapping homogeneous solution space proofs to Rank-Nullity.

- Solution: The homogeneous solution set is $K = \{x \in F^n : Ax = 0\}$, which is exactly the kernel $\text{N}(L_A)$ of the operator $L_A: F^n \to F^m$. By definition, $\text{rank}(A) = \dim(\text{R}(L_A)) = r$. The Dimension Theorem (Theorem 2.3) requires $\dim(\text{R}(L_A)) + \dim(\text{N}(L_A)) = \dim(\text{Domain}) \implies r + \dim(K) = n \implies \dim(K) = n - r$.
- Text Location: Section 3.3, Theorem 3.11 proof context (p. 173).

## 📜 Non-Major Theorem Recall

## T5.1: Theorem 3.6 (Invertible Multiplication Invariance)

- Statement: If $P$ and $Q$ are invertible, $\text{rank}(PAQ) = \text{rank}(A)$.
- Non-Invertible Bound: When invertibility is removed, we must appeal to the sub-multiplicative rank inequality derived from Theorem 3.4: $\text{rank}(PAQ) \leq \min(\text{rank}(P), \text{rank}(A), \text{rank}(Q))$.
- Text Location: Section 3.2, Theorem 3.6 (p. 156).

## T5.2: Theorem 3.9 (Full Row Rank Consistency)

- Statement: If $A$ is an $m \times n$ matrix with $\text{rank}(A) = m$, then $Ax=b$ is consistent $\forall b$.
- Free Variable Dimension: If $n > m$, the column dimension exceeds the row dimension. Since $\text{rank}(A) = m$, there are exactly $m$ pivot columns. By Rank-Nullity mapping, the dimension of the null space (free variables) is exactly $n - m$, creating an infinite solution space over infinite fields.
- Text Location: Section 3.3, Theorem 3.9 (p. 172).

## T5.3: Theorem 3.11 (Homogeneous System Dimensions)

- Statement: The solution space of a homogeneous system $Ax = 0$ in $n$ variables has dimension $n - \text{rank}(A)$.
- Calculation: Given $n = 5$ variables and $\text{rank}(A) = 3$, the theorem asserts $\dim(\text{Solution Space}) = 5 - 3 = 2$.
- Text Location: Section 3.3, Theorem 3.11 (p. 173).

---

## 📅 Day 6: Echelon Uniqueness & Equivalence of Systems (Sec 3.4)

## 📝 Structural Mechanics

## Q6.1: How RREF pivot geometry maps column independence invariants.

- Solution: Row reduction operates via left multiplication by invertible elementary matrices, preserving the kernel of column dependencies ($Ax = 0 \iff \text{RREF}(A)x = 0$). If column $j$ in the RREF contains a pivot, it cannot be formed by the preceding columns. Because kernel relations are invariant under invertible operations, column $j$ in the original matrix $A$ is guaranteed to be linearly independent of its preceding columns.
- Text Location: Section 3.4, Theorem 3.14 proof engine (p. 185).

## Q6.2: Echelon zero-row logic applied to invertibility constraints.

- Solution: A zero row in an $n \times n$ matrix RREF means the number of non-zero rows is $\leq n-1$. Because matrix rank equals the number of non-zero rows in RREF, $\text{rank}(A) < n$. Theorem 3.16 requires $\text{rank}(A) = n$ for invertibility; thus, the matrix is strictly singular.
- Text Location: Section 3.4, Theorem 3.16 implications (p. 189).

## 📜 Non-Major Theorem Recall

## T6.1: Theorem 3.14 (RREF Uniqueness)

- Statement: The reduced row echelon form of any matrix is unique.
- Loss of Uniqueness: If leading coefficients can equal any non-zero value $c \neq 1$, scaling a leading row by different elements creates non-identical row entries that still satisfy all other echelon sorting properties, destroying unique structural assignment.
- Text Location: Section 3.4, Theorem 3.14 (p. 185).

## T6.2: Theorem 3.16 (Invertibility RREF Characterization)

- Statement: An $n \times n$ matrix $A$ is invertible $\iff \text{RREF}(A) = I_n$.
- Non-Invertible Pivot Ceiling: If $A$ is non-invertible, $\text{RREF}(A) \neq I_n$, implying $\text{rank}(A) < n$. Since the number of pivot elements matches the rank exactly, the absolute maximum number of pivots is $n - 1$.
- Text Location: Section 3.4, Theorem 3.16 (p. 189).

## T6.3: Theorem 3.15 (Equivalence of Systems)

- Statement: If two systems are row-equivalent, they possess identical solution sets.
- Inhomogeneous Synchronization: An inhomogeneous system represents $L_A(x) = b$. An elementary row operation modifies this equation via left multiplication by an elementary matrix $E$, yielding $E L_A(x) = E b$. Failing to apply the operation to $b$ yields $E L_A(x) = b$, which constructs an entirely different geometric problem with a modified solution space.
- Text Location: Section 3.4, Theorem 3.15 (p. 187).

---


