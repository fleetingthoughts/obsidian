---
parent:
tags:
  - "#flashcard"
date_created: "2026-09-27"
---
Prove: A function that is continuous on a compact set $K$ is uniformly continuous on $K$. **Back:**
#### Notes
- Assume for contradiction $f$ is continuous but fails to be uniformly continuous.
    
- Apply the sequential criterion to obtain $(x_n), (y_n) \subseteq K$ with $\vert{}x_n - y_n\vert{} \to 0$ and $\vert{}f(x_n) - f(y_n)\vert{} \ge \epsilon_0$.
    
- Use compactness to extract a convergent subsequence $x_{n_k} \to x \in K$. Limit theorems force $y_{n_k} \to x$.
    
- Apply continuity at $x$ to show both $f(x_{n_k})$ and $f(y_{n_k})$ converge to $f(x)$.
    
- Deduce $\lim \vert{}f(x_{n_k}) - f(y_{n_k})\vert{} = 0$, contradicting the $\epsilon_0$ separation.