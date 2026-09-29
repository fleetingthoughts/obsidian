---
parent: "[[Understanding Analysis - 4.4 Continuous Functions on Compact Sets]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-27
---
Prove: If $f : A \to \mathbf{R}$ is continuous on $A$ and $K \subseteq A$ is compact, then $f(K)$ is compact.
#### Notes
- Take an arbitrary sequence $(y_n) \subseteq f(K)$ and select preimages $(x_n) \subseteq K$.
    
- Use the compactness of $K$ to extract a convergent subsequence $x_{n_k} \to x \in K$.
    
- Apply sequential continuity of $f$ at $x$ to deduce $y_{n_k} \to f(x)$.
    
- Conclude $f(x) \in f(K)$, showing every sequence in $f(K)$ has a convergent subsequence, rendering $f(K)$ compact.
