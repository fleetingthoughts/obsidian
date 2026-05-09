---
tags:
  - "#math"
  - "#real_analysis"
  - "#stephen_abbot"
date_created: 2026-03-10
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
This chapter contains several definition and simple theorems whose main difficulty rely on you understanding the definitions really carefully. It is therefore useful to organize my thoughts by compiling all the definitions and theorems in separate lists colloquially restated. In this section, we defined open sets, closed sets, and how to prove whether a set is either of these.

We begin with a preliminary on what $\epsilon$-neighborhood of a point $x=a$ is and use it to define an open set. The definition leads us to the following examples of an open set:
- The set of real numbers $\mathbb{R}$ is an open set
- The empty set is an open set
- Open intervals on $\mathbb{R}$
From the definition, we can also show what kind of operations we can perform on open sets to preserve openness. In ***Theorem 3.2.3***, the union of  arbitrary number of open sets remains open, but the intersection of only a finite number of open sets remains open. The reason being that the proof involves a minimum operation on the collection of open sets because if a point is in the intersection of the set, then only the smallest neighborhood can be contained in all the sets and therefore be in the intersection. We can only perform the minimum operation on a finite collection.

A closed set is a set that contains all its limit points so we need to define a limit point and how to identify them. 
- ***Definition 3.2.4*** defines a limit point with respect to a set $A$ as a point that can be made infinitely close to $A$ in the sense that every neighborhood of the limit point has a non-empty intersection with $A$. 
- ***Theorem 3.2.5*** is an equivalence statement showing how we can identify a limit point of a set by showing that we have at least one sequence $(a_n)$ in $A$ that converges to the limit point and <u>the limit point is not contained in the sequence.</u> The limit of a sequence in $A$ is logically equivalent to a limit point.
A nuance we note in ***Theorem 3.2.5***  is that in identify limit points, we have to show there is a sequence $(a_n)$<u> that does not have the limit point in the sequence </u>with the limit point $a$ as a limit. If we allowed the limit point to be in the sequence, then our theorem becomes uninteresting because we can always construct the sequence of just the limit point $(a,a,a.,...)$ and it trivially converges. 

By setting the requirement that we need to find a sequence not containing the limit point, we can distinguish isolated points from limit points. As defined in ***Definition 3.2.6***, isolated points are always contained in the set, but a limit point doesn't have to be. This is a binary definition in the sense that for all points in a set $A$, it is either closed or isolated. There is no third option. Therefore to prove a point is isolated is to prove it is not a limit point and vice versa.

Closed sets end up playing an important role and so we look at the operation of closing a set by the union with its limit point. Note that ***Definition 3.2.11*** for the closure of a set only defines an operation and despite its no name, it doesn't guarantee that the resulting union is a closed set, but ***Theorem 3.2.12*** assures us this operation produces a closed set and is actually the smallest closed set containing the original open set.

To conclude, Abbott provides additional tools to identify whether a set is open or closed by looking at its complement:
- ***Theorem 3.2.13*** lets us identify whether a set is open or closed by looking at the complement of the set.
***Theorem 3.2.13*** is required to prove the conditions that allow us to preserve closedness under union or intersection of other closed sets. The conditions are the opposite of the open set:
- The intersection and union of a finite and infinite number of open sets respectively preserves openness
- Theorem intersection and union of an infinite and finite number of closed sets respectively preserves closedness.
The last point is formalized in ***Theorem 3.2.14*** and combines  ***Theorem 3.2.13 (Determination of closedness and openness of a set by its complement)*** and ***Theorem 3.23 (Conditions for the preservation of openness under union and intersection of open sets)*** and applies DeMorgan's law to say something about closed sets.


# Summary of computational or proof based aspects of this chapter
To prove a set is an open set:
- Prove straight from definition by showing any arbitrary point will have at least 1 neighborhood contained in the set
- Show the set is a union of an infinite or finite collection of open sets or an intersection of a finite number of open sets
- Prove the complement of the set is closed

To prove a set is a closed set:
- Show it is a union of a finite collection of closed sets or the intersection of an infinite or finite number of closed sets.
- Show that any sequence inside the set converges to a limit that is inside the set as well. Note that any finite sequence is trivially contained in the set so we look at infinite sequences instead (if any).
- Show that every Cauchy sequence in the set has a limit that is an element in the set.
- If the complement of the set is open

# Concepts from exercises and nuances
- A closed set can be closed by virtue of containing no limit points. It becomes [vacuously true](The%20Empty%20Set%20and%20Vacuous%20Truths.md) that it is empty
- To identify a closed set, you just have to show that there exists at least one sequence in the set that converges to a limit. So if your set is defined as a sequence itself, you need to check if the subsequence converges. By Bolzano-Weierstrass, any bounded sequence will have a convergent subsequence, so all bounded sequences will have limit points.
- ***Exercise 3.2.4 (The supremum and its relation to a bounded above open or closed set).*** If a set $A$ is bounded above, the exists a supremum of the $\sup{A}=s$. The existence of the supremum depends on whether the set is open or closed:
	- If $A$ is closed, $\sup(A)\in A$. Alternatively, if $A$ is open, then $\sup(A)\in \bar{A}$ 
	- If $A$ is open, $s \notin A$.

# Review concepts used as preliminaries
- Reminder that what a neighborhood of a point is. The $\epsilon$-neighborhood of a point $x= a$, denoted $V_{\epsilon}(a)$, can be seen as a function where you input the following:
	- A point $x=a$
	- A parameter $\epsilon$
	The function outputs an interval of length $\epsilon$ centered on $a$.

- The rational and irrationals are infinitely dense on the real number line in the sense that for any two real numbers no matter how close, you can always find a rational or irrational number between them.

# Definitions
- ***Reminder of definition (Neighborhood of a point)***: a $\epsilon$-neighborhood of a point $a$ is denoted $V_{\epsilon}$ and is the set $V_{\epsilon}=\{x\in \mathbb{R}:|x-a|<\epsilon\}$ 
- ***Definition 3.2.1 (Open Sets).*** A set $O\subseteq \mathbb{R}$ is open if for every point $a\in O$, a neighborhood of a is contained in $O$ as well. Clarification of this definition. To prove a set is open, you only need to show any arbitrary point has at least 1 neighborhood that is completely contained in the set. This breaks down in closed intervals because any neighborhood around the endpoints will contain points outside the set.
- ***Definition 3.2.4 (Limit Points).*** A point, $x$ that has the condition that every $V_{\epsilon}(x)$ intersects with $O$ other than at $x$ itself. You can think of it as a point infinitely close to $O$ but is yet not in it OR a point that is right at the edge (i.e. endpoint of closed interval). In other words, it is like a limit and this limit can be contained in the set or not contained in the set.
- ***Definition 3.2.6 (Isolated point).*** An <u>isolated point of a set</u> (isolated point is defined relative to a certain set), is a point in the set that is not a limiting point.
- ***Definition 3.2.7 (Closed Sets).*** A set $F \in \mathbb{R}$ is closed if it contains its limit points.
- ***Definition 3.2.11 (Closure).*** Let there be a set $A$ with the set of limit points $L$. The closure of  is denoted $\bar{A}=A \cup L$. The closure is basically the original set + all its limit points. 

# Theorems
- ***Theorem 3.2.3 (Unions and intersections of open sets are themselves open sets).*** The union of an arbitrary collection of open sets is open. But the <u>intersection of a finite collection</u> of open sets is open
- ***Theorem 3.2.5 (relationship between limit points and limit operator).*** A point is a limit point for a set <u>if and only if </u>there is some sequence contained in the set that has the limit point as a limit. Also the sequence does not contain the limit point.
- ***Theorem 3.2.8 (criteria for a closed set).*** A set $F \subseteq R$ is closed if and only if every Cauchy sequence contained in $F$ has a limit that is also an element of $F$. 
	- The nuance here is that every convergent sequence is a Cauchy sequence by [Understanding Analysis - 2.6 The Cauchy Criterion](Understanding%20Analysis%20-%202.6%20The%20Cauchy%20Criterion.md), but Cauchy sequences are only convergent if the metric space is complete (i.e. in the reals which is assumed in the theorem).
	- One interesting result of this criteria is that the set of $\mathbb{Q}$ has all of $\mathbb{R}$ as its limit points. With any arbitrary real number, $y$, you can always have a rational contained in a $V_{\epsilon}(y)$ by the AoC (and Archimedean property). Notice that this also means the set of rational numbers has itself as limit points as well!
- ***Theorem 3.2.10 (Density of the rational numbers in the real reformulated in topological terms).*** For every real number, there exists a sequence of rational numbers that converges to it.
- ***Theorem 3.2.12 (the closure as the smallest closed version of a set).*** For any $A \subseteq R$, the closure $\bar{A}$ is a closed set and is the smallest closed set containing $A$.
- ***Theorem 3.2.13 (Determining closure of a set based on its complement).*** A set is open if its complement is closed. Likewise, a set is closed if its complement is open.
- ***Theorem 3.2.14 (Closure of a union and intersection of sets).*** Applying DeMorgan's laws and Theorem 3.2.3, the union of a finite collection of closed sets is closed. The intersection of an arbitrary collection of closed sets is closed.

Some other notes to further understand these theorems and definitions:
- Regarding Theorem 3.2.12. While we defined the limit points and isolated points as being the complement of each other, note that we made no such definition with closed or open sets and indeed there are sets that are simultaneously closed and open. The set of rational numbers is simultaneously closed and open. I think of it as sets that contain an infinite number of "holes" inside of it are weird like that. The set containing the terms of the harmonic series is neither open or closed for it doesn't contain its limit point 0 and it consists only of isolated points so it never contains a neighborhood for there will always be another rational number in between its terms.
- The use of the complement of a set does provide a relationship between open and closed sets if it applies to its complement.

