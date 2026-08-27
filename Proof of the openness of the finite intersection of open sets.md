---
parent: "[[Understanding Analysis - 3.2 Open and Closed Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-07-24
---
Prove that the finite intersection of open sets is open and which part of the proof requires the union to be finite.
#### Notes
- Let $\{O_1, O_2, \dots, O_N\}$ be a finite collection of open sets, and let $a \in \bigcap_{k=1}^N O_k$ be arbitrary.
    
- For every $k \in \{1, \dots, N\}$, use the openness of $O_k$ to obtain radii $\epsilon_k > 0$ such that $V_{\epsilon_k}(a) \subseteq O_k$.
    
- Define $\epsilon = \min\{\epsilon_1, \epsilon_2, \dots, \epsilon_N\}$. (Note that $\epsilon > 0$ strictly because the collection is finite).
    
- Establish that $V_\epsilon(a) \subseteq V_{\epsilon_k}(a) \subseteq O_k$ for all $k$, which implies $V_\epsilon(a) \subseteq \bigcap_{k=1}^N O_k$, proving openness.
