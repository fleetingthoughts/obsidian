---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.1 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch5
date_created: 2026-09-19
---
Prove the relationship between the eigenvector of a linear operator and the eigenvector of its corresponding matrix representation.
#### Notes
**Relation:**
A vector $v \in V$ is an eigenvector of a linear operator $T$ with eigenvalue $\lambda$ if and only if its coordinate vector $[v]_\beta$ is an eigenvector of the matrix representation $[T]_\beta$ with the same eigenvalue $\lambda$.

**Skeleton Proof:**

* **Setup:** Let $V$ be a vector space with basis $\beta$, and let $T: V \to V$ be a linear operator.
* **Forward Direction ($\Rightarrow$):**
* **Assume:** $v$ is an eigenvector of $T$. Therefore, $T(v) = \lambda v$, where $v \neq 0$.
* **Map to Coordinates:** Take the coordinate representation of both sides with respect to the basis $\beta$: $[T(v)]_\beta = [\lambda v]_\beta$.
* **Apply Isomorphism Properties:** Use the standard property of matrix representations to pull out the matrix and scalar: $[T]_\beta [v]_\beta = \lambda [v]_\beta$.
* **Conclude:** Because $v \neq 0$, its coordinate vector $[v]_\beta \neq 0$. Thus, $[v]_\beta$ satisfies the definition of an eigenvector for the matrix $[T]_\beta$.


* **Reverse Direction ($\Leftarrow$):**
* **Assume:** $[v]_\beta$ is an eigenvector of $[T]_\beta$. Therefore, $[T]_\beta [v]_\beta = \lambda [v]_\beta$, where $[v]_\beta \neq 0$.
* **Convert to Operator:** Apply the coordinate map properties in reverse to group the terms: $[T(v)]_\beta = [\lambda v]_\beta$.
* **Evaluate Isomorphism:** Because the coordinate mapping to $F^n$ is an isomorphism (strictly one-to-one), the vectors inside the brackets must be identical: $T(v) = \lambda v$.
* **Conclude:** Because $[v]_\beta \neq 0$, the original vector $v \neq 0$. Thus, $v$ satisfies the definition of an eigenvector for the linear operator $T$.
<!--SR:!fsrs,2026-10-09T03:11:25.138Z,8,8.2956,1,2,1,0,0,2026-10-01T03:11:25.138Z-->

- Suppose $v$ is an eigenvector of $T$ corresponding to $\lambda$, meaning $T(v) = \lambda v$.
    
- Then $A\phi_\beta(v) = L_A\phi_\beta(v) = \phi_\beta T(v) = \phi_\beta(\lambda v) = \lambda\phi_\beta(v)$.
    
- Now $\phi_\beta(v) \neq 0$ because $\phi_\beta$ is an isomorphism and $v \neq 0$. Hence, $\phi_\beta(v)$ is an eigenvector of $A$.
    
- This argument is reversible.
    

An equivalent formulation is that for an eigenvalue $\lambda$, a vector $y \in F^n$ is an eigenvector of $A \iff \phi_\beta^{-1}(y)$ is an eigenvector of $T$ corresponding to $\lambda$.

