---
parent: "[[Understanding Analysis - 3.4 Perfect Sets and Connected Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-09-11
---
Prove that a set $E \subseteq \mathbf{R}$ is connected if and only if whenever $a < c < b$ with $a, b \in E$, it follows that $c \in E$ as well.
#### Notes
- _Forward Direction ($\implies$):_
    1. Assume $E$ is connected, let $a, b \in E$ with $a < c < b$, and assume for contradiction that $c \notin E$.
    2. Define $A = (-\infty, c) \cap E$ and $B = (c, \infty) \cap E$, observing that $a \in A$ and $b \in B$ so that $A$ and $B$ are nonempty, disjoint, and $E = A \cup B$.
    3. Verify that $\bar{A} \subseteq (-\infty, c]$ is disjoint from $B$ and $\bar{B} \subseteq [c, \infty)$ is disjoint from $A$, proving $A$ and $B$ are separated and $E$ is disconnected, contradicting the hypothesis.
- _Backward Direction ($\impliedby$):_
    1. Assume $E$ is an interval, and partition $E$ into nonempty disjoint sets $A$ and $B$ with $a_0 \in A$ and $b_0 \in B$ where $a_0 < b_0$, so that $I_0 = [a_0, b_0] \subseteq E$.
    2. Bisect $I_0$ repeatedly to produce nested closed intervals $I_n = [a_n, b_n]$ with $a_n \in A$, $b_n \in B$, and lengths $\lim (b_n - a_n) = 0$.
    3. Apply the Nested Interval Property to obtain $x \in \bigcap_{n=0}^\infty I_n$ such that $\lim a_n = x = \lim b_n$.
    4. Observe that $x \in E = A \cup B$ must belong to $A$ (making it a limit point of $B$) or $B$ (making it a limit point of $A$), fulfilling the sequential criterion for connectedness.
