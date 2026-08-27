---
parent: "[[Understanding Analysis - 3.3 Compact Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-07-24
---
Prove that if a set in the reals is closed and bounded, then every open cover of the set has a finite subcover. 
#### Notes
- Assume $K$ is closed and bounded but has an open cover with no finite subcover. Let $I_0$ be a closed interval containing $K$.
    
- Bisect $I_0$ recursively, selecting the nested half $I_n$ where $I_n \cap K$ cannot be covered finitely.
    
- The intersection $\bigcap_{n=0}^\infty I_n$ contains a unique point $x \in K$ (since $K$ is closed and $\lim\vert{}I_n\vert{} = 0$).
    
- The point $x$ must belong to some open set $O_{\lambda_0}$ in the cover, meaning $V_\epsilon(x) \subseteq O_{\lambda_0}$.
    
- For sufficiently large $n$, $I_n \subseteq V_\epsilon(x) \subseteq O_{\lambda_0}$, contradicting the assumption that $I_n \cap K$ requires infinitely many cover sets.
