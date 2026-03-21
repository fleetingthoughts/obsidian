---
tags:
  - "#math"
  - "#real_analysis"
  - "#stephen_abbot"
date_created: 2026-03-10
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
This chapter contains several definition and simple theorems whose main difficulty rely on you understanding the definitions really carefully. It is therefore useful to organize my thoughts by compiling all the definitions and theorems in separate lists colloquially restated. In this section, we defined open sets, closed sets, and how to prove whether a set is either of these.

To prove a set is an open set:
- Prove straight from definition by showing any arbitrary point will have at least 1 neighborhood contained in the set
- Show the set is a union of an infinite or finite collection of open sets or an intersection of a finite number of open sets
- If the complement of the set is closed

To prove a set is a closed set:
- Show it is a union of a finite collection of closed sets or the intersection of an infinite or finite number of closed sets.
- Show that any sequence inside the set converges to a limit that is inside the set as well. Note that any finite sequence is trivially contained in the set so we look at infinite sequences instead (if any).
- Show that every Cauchy sequence in the set has a limit that is an element in the set.
- If the complement of the set is open

# Definitions
- Reminder of definition of neighborhood of a point: a $\epsilon$-neighborhood of a point $a$ is denoted $V_{\epsilon}$ and is the set $V_{\epsilon}=\{x\in \mathbb{R}:|x-a|<\epsilon\}$ 
- ***Definition 3.2.1 (Open Sets).*** A set $O\subseteq \mathbb{R}$ is open if for every point $a\in O$, a neighborhood of a is contained in $O$ as well. Clarification of this definition. To prove a set is open, you only need to show any arbitrary point has at least 1 neighborhood that is completely contained in the set. This breaks down in closed intervals because any neighborhood around the endpoints will contain points outside the set.
- ***Definition 3.2.4 (Limit Points).*** A point, $x$ that has the condition that every $V_{\epsilon}(x)$ intersects with $O$ other than at $x$ itself. You can think of it as a point infinitely close to $O$ but is yet not in it OR a point that is right at the edge (i.e. endpoint of closed interval). In other words, it is like a limit and this limit can be contained in the set or not contained in the set.
- ***Definition 3.2.6 (Isolated point).*** An <u>isolated point of a set</u> (isolated point is defined relative to a certain set), is a point in the set that is not a limiting point.
- ***Definition 3.2.7 (Closed Sets).*** A set $F \in \mathbb{R}$ is closed if it contains its limit points.
- ***Definition 3.2.11 (Closure).*** Let there be a set $A$ with the set of limit points $L$. The closure of  is denoted $\bar{A}=A \cup L$. The closure is basically the original set + all its limit points. 

# Theorems
- ***Theorem 3.2.3 (Unions and intersections of open sets are themselves open sets).*** The union of an arbitrary collection of open sets is open. But the <u>intersection of a finite collection</u> of open sets is open
- ***Theorem 3.2.5 (relationship between limit points and limit operator).*** A point is a limit point for a set <u>if and only if </u>there is some sequence contained in the set that has the limit point as a limit. Also the sequence does not contain the limit point.
- ***Theorem 3.2.7 (criteria for a closed set).*** A set $F\in R$ is closed if and only if every Cauchy sequence contained in $F$ has a limit that is also an element of $F$. 
	- One interesting result of this criteria is that the set of $\mathbb{Q}$ has all of $\mathbb{R}$ as its limit points. With any arbitrary real number, $y$, you can always have a rational contained in a $V_{\epsilon}(y)$ by the AoC (and Archimedean property). Notice that this also means the set of rational numbers has itself as limit points as well!
- ***Theorem 3.2.10 (Density of the rational numbers in the real reformulated in topological terms).*** For every real number, there exists a sequence of rational numbers that converges to it.
- ***Theorem 3.2.12 (the closure as the smallest closed version of a set).*** For any $A \subseteq R$, the closure $\bar{A}$ is a closed set and is the smallest closed set containing $A$.
- ***Theorem 3.2.13 (Determining closure of a set based on its complement).*** A set is open if its complement is closed. Likewise, a set is closed if its complement is open.
- ***Theorem 3.2.14 (Closure of a union and intersection of sets).*** Applying DeMorgan's laws and Theorem 3.2.3, the union of a finite collection of closed sets is closed. The intersection of an arbitrary collection of closed sets is closed.

Some other notes to further understand these theorems and definitions:
- Regarding Theorem 3.2.12. While we defined the limit points and isolated points as being the complement of each other, note that we made no such definition with closed or open sets and indeed there are sets that are simultaneously closed and open. The set of rational numbers is simultaneously closed and open. I think of it as sets that contain an infinite number of "holes" inside of it are weird like that. The set containing the terms of the harmonic series is neither open or closed for it doesn't contain its limit point 0 and it consists only of isolated points so it never contains a neighborhood for there will always be another rational number in between its terms.
- The use of the complement of a set does provide a relationship between open and closed sets if it applies to its complement.

