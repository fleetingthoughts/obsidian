---
parent: "[[Understanding Analysis - 3.2 Open and Closed Sets]]"
tags:
  - "#flashcard"
  - macro/math/
date_created: 2026-07-24
---
Prove that the definition of closure, $A \cup L$,  is closed where $L$ is the set of all limit points of $A$
#### Notes
**Exercise 3.2.7 (a): Show $L$ is closed.**

Let $x$ be a limit point of $L$. For any $\epsilon > 0$, the neighborhood $V_\epsilon(x)$ contains a point $y \in L$ ($y \neq x$). Because $V_\epsilon(x)$ is open, there is a smaller neighborhood $V_\delta(y) \subseteq V_\epsilon(x)$ that excludes $x$. Since $y$ is a limit point of $A$, $V_\delta(y)$ must contain a point $a \in A$ ($a \neq y$). Thus, $a \in V_\epsilon(x)$ and $a \neq x$. This means $x$ is a limit point of $A$ ($x \in L$). Since $L$ contains its limit points, it is closed. $\blacksquare$

 **Limit point of $A \cup L$ is in $L$.**

Let $x$ be a limit point of $A \cup L$. For any $\epsilon > 0$, $V_\epsilon(x)$ contains a point $y \in A \cup L$ ($y \neq x$).

- **If $y \in A$:** $V_\epsilon(x)$ immediately contains a point in $A$ distinct from $x$.
    
- **If $y \in L$:** A smaller open sub-neighborhood around $y$ (excluding $x$) must contain a point $a \in A$. Thus, $a \in V_\epsilon(x)$ and $a \neq x$.
    

In both cases, $V_\epsilon(x)$ intersects $A$ at a point other than $x$. Therefore, $x \in L$. $\blacksquare$


The closure is defined as $\overline{A} = A \cup L$. We just proved that any limit point of $A \cup L$ is in $L$. Since $L \subseteq A \cup L$, the set $A \cup L$ contains all of its limit points and is therefore closed. $\blacksquare$
