---
parent: "[[Understanding Analysis - 3.2 Open and Closed Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbot/ch3
date_created: 2026-07-24
---
Prove that $x$ is a limit point of a set $A \subseteq \mathbb{R}$ if and only if there exists a sequence in $A$ that converges to $x$.
#### Notes
**Forward Direction ($\implies$):**
1. Assume $x$ is a limit point of $A$. Construct a sequence of neighborhoods $V_{1/n}(x)$ for each $n \in \mathbf{N}$.
2. Choose $a_n \in V_{1/n}(x) \cap A$ with $a_n \neq x$.
3. For arbitrary $\epsilon > 0$, choose $N \in \mathbf{N}$ such that $1/N < \epsilon$. Verify $\vert{}a_n - x\vert{} < 1/n \leq 1/N < \epsilon$ for all $n \geq N$, proving $(a_n) \to x$.
    
**Backward Direction ($\impliedby$):**
1. Assume there exists $(a_n) \subseteq A$ with $a_n \neq x$ for all $n \in \mathbf{N}$ and $\lim a_n = x$. Let $V_\epsilon(x)$ be an arbitrary neighborhood.
2. By sequential convergence, choose $N \in \mathbf{N}$ such that $a_N \in V_\epsilon(x)$.
3. Because $a_N \in A$ and $a_N \neq x$, the neighborhood $V_\epsilon(x)$ intersects $A$ at a point other than $x$, proving $x$ is a limit point.
