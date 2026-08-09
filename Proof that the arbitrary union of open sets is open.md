---
parent: "[[Understanding Analysis - 3.2 Open and Closed Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbot/ch3
date_created: 2026-07-24
---
Prove that the arbitrary union of open sets whether it is an infinite or finite union is also open
#### Notes
- Let $O = \bigcup_{\lambda \in \Lambda} O_\lambda$, where each $O_\lambda$ is open, and let $a \in O$ be arbitrary.
    
- By definition of union, $a \in O_{\lambda'}$ for some specific $\lambda'$.
    
- Invoke the openness of $O_{\lambda'}$ to yield an $\epsilon$-neighborhood such that $V_\epsilon(a) \subseteq O_{\lambda'}$.
    
- Conclude that since $O_{\lambda'} \subseteq O$, it follows that $V_\epsilon(a) \subseteq O$, proving $O$ is open.
