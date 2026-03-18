---
tags:
  - math
  - real_analysis
  - stephen_abbot
date_created: 2026-03-17
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
Continuing our development of properties to analytically describe mathematical infinity from 3.3, we now describe perfect sets and connected sets. The chapter is outlined as follows:
- Definition of perfect sets and their relationship to the infinity of uncountability
- Definition of connected sets and two equivalency conditions to connected sets
The entire chapter continues in the same vein as 3.3 where we aim to analytically describe the fundamental properties of mathematical objects that exhibit a phenomena of interest. The concept of closed intervals for instance exhibits the property of compactness, but we were able to derive equivalency conditions to show that other kinds of set can exhibit compactness as well so that compact sets can be seen as a generalization of closed intervals. 

We now try to crystallize another property similarly that generalizes a certain kind of infinity. ***Definition 3.4.1 (Perfect Sets)*** defines a perfect set and ***Theorem 3.4.3 (Sufficiency for uncountability)***, shows that perfect sets exhibit the phenomena of "infinite" in being uncountable.
# Connected sets and convergence and intervals containing infinity
***Definition 3.4.4*** defines the 3 properties and the following should be noted to better illustrate the definitions:
- Separated is a property between two sets while disconnectedness and connectedness are are mutually exclusive properties of a single set. 
- The separation of two sets is a stronger condition than being disjoint. While all separated sets are disjoint, disjoint sets are not necessarily separated.
To illustrate the definition better, its helpful to show how connectedness is proven. A set $E$ is shown to be connected or disconnected if:
1) It can be proven no matter how it is partitioned into two separate sets, it is always possible to show that at least one of the sets contains a limit point of the other.
- prove it is disconnected by providing a counter example of a partition into two sets that are not separated
Particularly for 1) it is something that can be generalized as demonstrated in ***Theorem 3.4.6 (process to prove connectedness)*** and it should be noted that we only need to show one such convergent sequence satisfies that criterion.

Another way to show connectedness is probably ***Theorem 3.4.7 (equivalency condition for connectedness)*** that allows us to demonstrate the connectedness using intervals in $\mathbb{R}$ and most notably for intervals containing infinity.
# Definitions
- ***Definition 3.4.1 (Perfect Sets).*** A perfect set $P \subseteq \mathbb{R}$ is perfect if it is closed and contains no isolated points.
- ***Theorem 3.4.3 (Property sufficient for uncountability).*** A nonempty perfect set is uncountable.
- ***Definition 3.4.4 (Connected, separated, and disconnected sets).*** 
	- Two nonempty sets $A, B \subseteq \mathbb{R}$ are separated if $\bar{A}\cap B = A \cap \bar{B}= \emptyset$ 
	- A set $E \subseteq \mathbb{R}$ is disconnected if it can be constructed as $E= A\cup B$ where $A$ and $B$ are separated
	- A set that is not disconnected is a connected set.
# Theorems
***Theorem 3.4.3 (Property sufficient for uncountability).*** A nonempty perfect set is uncountable.

***Theorem 3.4.6 (Criterion for convergent sequences as an equivalent condition for connectedness).*** A set $E \subseteq \mathbb{R}$ is connected <u>if and only if </u> for all nonempty disjoint sets $A$ and $B$ satisfying $E=A\cup B$, there always exists a convergent sequence $(x_n)\to x$ where the convergent sequence $(x_n)$ is contained in one set while the limit point $x$ is contained in the other.

***Theorem 3.4.7 (Equivalency condition for connectedness).***  A set $E \subseteq \mathbb{R}$ is connected <u>if and only if</u> whenever $a < c < b$ with $a, b \in E$, it follows that $c \in E$ as well.


