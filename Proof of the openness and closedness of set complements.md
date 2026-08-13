---
parent: "[[Understanding Analysis - 3.2 Open and Closed Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-07-24
---
Prove that the complement of an open set is closed and vice versa.
#### Notes
**Forward Direction (If $O$ is open, then $O^c$ is closed):**
1. Assume $O$ is open, and let $x$ be an arbitrary limit point of $O^c$.
2. Assume for contradiction that $x \in O$. Since $O$ is open, there exists $V_\epsilon(x) \subseteq O$.
3. This neighborhood contains no points of $O^c$, contradicting that $x$ is a limit point of $O^c$. Conclude $x \in O^c$.
**Backward Direction (If $O^c$ is closed, then $O$ is open):**
4. Assume $O^c$ is closed, and let $x \in O$ (so $x \notin O^c$).
5. Since $O^c$ is closed, $x$ cannot be a limit point of $O^c$.
6. Negate the limit point definition to obtain an $\epsilon$-neighborhood $V_\epsilon(x)$ that does not intersect $O^c$.
7. Conclude $V_\epsilon(x) \subseteq O$, proving $O$ is open.
