parent: [Book of Proof 3rd ed. - Richard Hammond](Book%20of%20Proof%203rd%20ed.%20-%20Richard%20Hammond.md)
tag: #textbook #math #analysis #proof

# 1.1 Sets
The cardinality or size of a finite set is the number of elements in the set $A$ denoted as $|A|$  so $A = \{1,2,a,p\}$ has cardinality of 4: $|A|$ = 4
# 1.2 Cartesian Product

We describe a process to create ordered pairs:
***Definition 1.1 (Ordered pairs).*** An ordered pair is a list of $(x,y)$ objects

***Definition 1.2 (Cartesian Product).*** The Cartesian product of two sets $A$ and $B$ is another set denoted $A \times B$ defined as $A \times B$ = $\{(a,b): a \in A, b \in B\}$ .

Note that the Cartesian product is not commutative.
# 1.3 Subsets
The empty set is a subset of all sets, that is $\emptyset \subseteq B$   for any set B. 

For any finite set with $n$ elements, there are $2^n$ possible subsets. This can be see by the binomial theorem.
# 1.4 Power Set
***Definition 1.4 (Power Sets).*** If $A$ is a set, the power set of $A$ denoted $P(A)$ is se of all subsets of $A$:
$$ P(A): \{X:X\subseteq A\}$$ The cardinality of $P(A)$ is therefore $|P(A)| = 2^{|A|}$ 

# 1.9 Sets That Are Number Systems
The sets that concern us are the familiar numbers systems. One postulate of the NATURAL NUMBERS is the well-ordering principle which states any non-empty set $A \subseteq N$ will have a smallest element. Indeed this is not a property we may find for real or rational numbers for consider the set $B \subseteq R$ such that $B =\{1/n: n\in N\}$ which will never have a smallest element for by the [Archimedean Principle](1.4%20Consequences%20of%20Completeness.md) if we assume the existence of a smallest number $x$ then we can always find a natural number $n > x$ which implies $1/n < x$ . A consequence of the well-ordering principle is the division algorithm:

***Fact 1.5 (Division Algorithm).*** Given integers $a$ and $b$ with $b>0$, there exists unique integers $q$ and $r$ for which $a=qb+r$ with $0 \le r\lt b$ .

# 1.10 Russel's Paradox
Some historical background that won't be developed showing how mathematicians realized the importance of carefully crafting axioms as some can lead to paradoxical results. Bertrand Russel provided this paradoxical set:$$A = \{X: X \text{ is a set } X \notin X\}$$
Reworded, this is the set of all sets that does not include itself as elements.

The paradox instigated a careful reformulation of the axioms for set theory called the Zermelo-Fraenkel axioms one of which is the well-ordering principle. Another axiom to eliminate Bertrand's paradox is the axiom of foundation which states no non-empty set $X$ can have the property $X \cap x \ne \emptyset$ . T