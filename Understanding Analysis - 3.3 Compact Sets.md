---
tags:
  - math
  - real_analysis
  - stephen_abbot
date_created: 2026-03-16
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
Continuing our discussion on sets, we describe a property that will be used to ascribe a concrete analytical way to describe concepts related to mathematical infinity (e.g. limits, derivatives, integrals). The property developed and the focus of the chapter will be the property of "compact sets", but this property will be shown to be equivalent to other properties. The chapter will proceed as follows:
- Definition of compact sets
- Definition of bounded sets and equivalency condition with compactness in $\mathbb{R}$. 
- Alternative way to describe compactness with "open covers" and "finite subcovers".
- The equivalency of all three properties (Heine-Borel Theorem).

It should be noted the chapter will focus on sets with elements in $\mathbb{R}$ and so all the sets discussed will be subsets of $\mathbb{R}$. 
# Definition of compactness and the 1st equivalency condition
***Definition 3.3.1*** defines compactness as a set that has all its sequences contained in it converging to a limit that is also in the set. By the definition, the two main criteria to check for compactness are:
1) EVERY sequence has a subsequence that converges (not necessarily to the same limit)
2) the limit that the sequences converge to are contained in the set.
The most basic example of a compact set is the closed interval as boundedness of the guarantees convergence by the Boltzmann-Weierstrass theorem and the fact that its a closed set means it contains its limit points. It can be shown that these properties in general guarantee and are a equivalency condition to compactness. The advantage in defining the compact set as a stronger closed set (i.e. with the additional property of boundedness) is that it guarantees there are convergent subsequences in the set so that it'll have to have limit points. <u>The definition of a closed set can be closed by virtue of not having any limit points at all which is what the compact set bypasses</u>. ***Theorem 3.3.4.*** shows that compactness is equivalent to a set that has the following 2 properties:
- The set is bounded
- The set is closed

The relationship between compactness and closed sets is made clear by ***Theorem 3.3.4.*** which shows a compact set is equivalent to a closed interval. The equivalency between the two can be demonstrated by showing that a property closed intervals have in $\mathbb{R}$ is also shared by compact sets. ***Theorem 3.3.5 (The nested compact sets property)*** demonstrates that compact sets also have a "nested interval property" exhibited by closed intervals (again both the set and intervals are in the real).

# Definition of open covers and finite subcovers and the 2nd equivalency condition to compactness
The equivalency between compact sets and sets that are bounded and closed demonstrates that we could've defined bounded and closed sets first and show the exhibit the property of compactness, namely: "bounded and closed sets have a convergent subsequences with their limits in the set." We now describe a second set of properties that are also equivalent to compactness

***Definition 3.3.6*** defines two things:
- a relationship between a set, $A$, and a union of open sets called the open cover. 
- A finite subset of the open cover that still completely contains $A$ called the <u>finite subcover.</u>
Therefore to prove that a collection of open sets is an open cover for a set of interest we need to show that any arbitrary element of the set will be contained in the open cover. Note that it is not guaranteed any open set has a finite subcover

Now armed with this 3rd property of open sets  and finite subcovers, we establish an equivalency condition expressed as  ***Theorem 3.3.8 (Three equivalency conditions regarding sets in the real).*** that summarizes all 3 equivalencies called the Heine-Borel Theorem:
- A compact set
- A set that is closed and bounded
- Every open cover of the set has a finite subcover.
# Definitions 
***Definition 3.3.1 (Compactness).*** A set $K \subseteq \mathbb{R}$ is called "compact" if every sequence in $K$ has a subsequence that converges to a limit that is also in $K$.

***Definition 3.3.6 (Open sets and finite subcovers of a set in reals).*** An open cover for $A$ is a (possibly infinite) collection of open sets $\{O_{\lambda}:\lambda \in \Lambda\}$ whose union contains the set $A$, that is $A\subseteq \cup_{\lambda \in \Lambda} O_{\lambda}$. Given an open cover, a finite subcover is a finite subcollection of the original open cover that still contains $A$. 

# Theorems 
***Theorem 3.3.4. (Boundedness and Closedness as an equivalent condition to compactness).*** A set $K \subseteq \mathbb{R}$ is compact if and only if the set is closed and bounded

***Theorem 3.3.5. (Nested Compact Set Property).***

***Theorem 3.3.8 (Heine-Borel Theorem).*** Let $K \subseteq \mathbb{R}$. All of the following statements are equivalent in the sense that any of them implies the other:
1) $K$ is compact
2) $K$ is bounded and closed
3) $K$ any open cover of $K$ has a finite subcover.
