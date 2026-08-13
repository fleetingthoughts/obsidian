---
parent: "[[Understanding Analysis - 3.2 Open and Closed Sets]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch3
date_created: 2026-07-24
---
If $x$ is a limit point of $A \cup B$, prove that $x$ is either a limit point of $A$ or $B$ or both
#### Notes
### Brief Proof by Contradiction

Assume $x$ is a limit point of $A \cup B$, but is **neither** a limit point of $A$ **nor** a limit point of $B$.

By definition, there must exist open neighborhoods $U_A$ and $U_B$ containing $x$ such that:

$$(U_A \setminus \{x\}) \cap A = \emptyset$$

$$(U_B \setminus \{x\}) \cap B = \emptyset$$

Let $U = U_A \cap U_B$. Since the finite intersection of open sets is open, $U$ is a valid open neighborhood of $x$.

Test $U$ against the union $A \cup B$:

$$(U \setminus \{x\}) \cap (A \cup B) = \Big((U \setminus \{x\}) \cap A\Big) \cup \Big((U \setminus \{x\}) \cap B\Big)$$

Since $U \subseteq U_A$ and $U \subseteq U_B$, both intersections on the right side are empty:

$$\emptyset \cup \emptyset = \emptyset$$

This shows $(U \setminus \{x\}) \cap (A \cup B) = \emptyset$, meaning $x$ is not a limit point of $A \cup B$. This directly contradicts our initial assumption, completing the proof. $\blacksquare$
