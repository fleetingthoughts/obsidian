---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.3 Subspaces]]"
tags:
  - "#flashcard"
  - micro/math/friedberg/ch1
date_created: 2026-07-24
---
State the condition for the union of two subspaces to be a subspace
#### Notes
Let $V$ be a vector space and $W_1, W_2$ be subspaces of $V$. The union $W_1 \cup W_2$ is a subspace of $V$ if and only if one subspace is contained within the other, meaning either $W_1 \subseteq W_2$ or $W_2 \subseteq W_1$.

### Rigorous proof

**Forward implication (If $W_1 \cup W_2$ is a subspace, then $W_1 \subseteq W_2$ or $W_2 \subseteq W_1$):**

We will prove this by contradiction. Assume that $W_1 \cup W_2$ is a subspace, but neither is a subset of the other. That is, assume $W_1 \not\subseteq W_2$ and $W_2 \not\subseteq W_1$.

Because $W_1 \not\subseteq W_2$, there must exist some vector $x \in W_1$ such that $x \notin W_2$.

Similarly, because $W_2 \not\subseteq W_1$, there must exist some vector $y \in W_2$ such that $y \notin W_1$.

Since $x \in W_1$ and $y \in W_2$, both $x$ and $y$ are elements of the union $W_1 \cup W_2$. Because we assumed $W_1 \cup W_2$ is a subspace, it must be closed under vector addition. Therefore, the sum $(x + y)$ must also be in $W_1 \cup W_2$.

By the definition of a union, this means either $x + y \in W_1$ or $x + y \in W_2$.

1. **Case 1: Suppose $x + y \in W_1$.**
    
    Since $W_1$ is a subspace, it is closed under scalar multiplication and addition, so its additive inverse $-x \in W_1$. Therefore, $(x + y) + (-x) \in W_1$, which simplifies to $y \in W_1$. This directly contradicts our initial premise that $y \notin W_1$.
    
2. **Case 2: Suppose $x + y \in W_2$.**
    
    Since $W_2$ is a subspace, $-y \in W_2$. Therefore, $(x + y) + (-y) \in W_2$, which simplifies to $x \in W_2$. This directly contradicts our initial premise that $x \notin W_2$.
    

In both cases, we reach a logical contradiction. Therefore, our initial assumption must be false, proving that it must be true that either $W_1 \subseteq W_2$ or $W_2 \subseteq W_1$.

**Reverse implication (If $W_1 \subseteq W_2$ or $W_2 \subseteq W_1$, then $W_1 \cup W_2$ is a subspace):**

This direction is straightforward.

If $W_1 \subseteq W_2$, then $W_1 \cup W_2 = W_2$. Since $W_2$ is given as a subspace, the union is automatically a subspace.

If $W_2 \subseteq W_1$, then $W_1 \cup W_2 = W_1$. Since $W_1$ is given as a subspace, the union is automatically a subspace.