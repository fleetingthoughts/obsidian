---
parent:
tags:
  - "#flashcard"
date_created: 2026-07-24
---
Prove one of the implications (Finite Subcover $\implies$ Closed and Bounded)
#### Notes
- **Boundedness**: Define an open cover for $K$ using radius-1 neighborhoods $O_x = V_1(x)$. Extract a finite subcover. $K$ is contained in a finite union of bounded sets, hence bounded.
    
- **Closedness**: Let $(y_n)$ be a Cauchy sequence in $K$ converging to $y \notin K$ (assume for contradiction).
    
- Define the open interval $O_x = V_{\vert{}x-y\vert{}/2}(x)$ for each $x \in K$ to create an open cover.
    
- Extract a finite subcover and define the minimum radius $\epsilon_0 = \min\{\vert{}x_i-y\vert{}/2\}$.
    
- Find $y_M$ satisfying $\vert{}y_M-y\vert{} < \epsilon_0$. This term cannot belong to any $O_{x_i}$ in the finite subcover, yielding a contradiction. Thus $K$ is closed.
