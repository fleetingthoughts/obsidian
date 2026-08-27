---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 2.1 Linear Transformations, Null Spaces, and Ranges]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch2
date_created: 2026-07-24
---
Prove the following. Let $V$ and $W$ be finite-dimensional vector spaces and $T:V \to W$ be a linear transformation. If $\dim(V) < \dim(W)$, $T$ cannot be onto. If $\dim(V) > \dim(W)$, $T$ cannot be one-to-one.
#### Notes
- **Rank-Nullity Foundation:** Invoke the Dimension Theorem: $\text{nullity}(T) + \text{rank}(T) = \dim(V)$.
    
- **Onto Impossibility Setup:** Assume $\dim(V) < \dim(W)$. Since $\text{nullity}(T) \ge 0$, the Dimension Theorem implies $\text{rank}(T) \le \dim(V)$.
    
- **Onto Conclusion:** By transitivity, $\text{rank}(T) \le \dim(V) < \dim(W)$. Because $\dim(R(T)) < \dim(W)$, $R(T)$ cannot be the entire space $W$, so $T$ is not onto.
    
- **One-to-One Impossibility Setup:** Assume $\dim(V) > \dim(W)$. Since $R(T)$ is a subspace of $W$, its dimension is bounded by $W$: $\text{rank}(T) \le \dim(W)$.
    
- **One-to-One Conclusion:** Substitute the rank bound into the Dimension Theorem: $\text{nullity}(T) = \dim(V) - \text{rank}(T) \ge \dim(V) - \dim(W)$. Since $\dim(V) > \dim(W)$, this difference is strictly greater than $0$. Thus $\text{nullity}(T) > 0$, meaning $N(T) \neq \{0\}$, so $T$ is not one-to-one.
