---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - math
  - stephen_abbot
  - understanding_analysis
  - real_analysis
date_created:
---
The final consequence of the AoC is the size of infinity it produces in the real numbers. We explore the work of Georg Cantor and show how the size of infinite sets can be compared. In this section we develop the following:
1) A method and definition to compare the "size" of a set to another set by cardinality.
2) Use the method of 1) to show that $\mathbb{N}$ is the same "size" as $\mathbb{Z}$ and $\mathbb{Q}$,  but $\mathbb{R}$ is "larger" than $\mathbb{N}$ which implies that there are way more irrational numbers than rational numbers.

We use the idea of a function's 1-1 mapping to compare the size of a set by saying that a set can be thought of as equal "size" to another set if there exists a function such that every element in that set can be mapped out. 

We first define the tools we will use in ***Definition 1.5.1.***  Given a function $f: A\to B$ , the following is defined
1) The function is one-to-one (1-1, injective)  if $a_1\ne a_2$ then $f(a_1) \ne f(a_2)$. 
2) The function is "onto" (surjective) if for every $b \in B$ there exists an $a \in A$ such that $f(a) = b$ 

 If an element in $B$ is mapped by a [1-1](Surjectivity,%20Injectivity,%20and%20Bijectivity.md) function, then precisely one unique $a$ gets mapped to it. Every value in the domain gets its own unique value in the range and no two values in the domain map to the same range value. And [onto](Surjectivity,%20Injectivity,%20and%20Bijectivity.md) means that the image of the function contains all of $B$. This is also called a surjective function and the implication is that EVERY element of  $B$ is being mapped. The set containing being mapped to, $B$, is called the codomain, and the elements in $B$ that are actually mapped are referred to as the  $image$ of the function, so for a surjective function, the entire codomain $B$ basically becomes the image.

If a function $f: A\to B$  is 1-1 and onto (surjective and injective) then it is bijective. This implies that the function $f$ is invertible such that there exists another function $f^{-1}$ such that $f^{-1}: B \to A$ 

Note there is another term called the range of a function which is a bit ambiguous for whether it refers to the image or the codomain. Image and codomain are the more precise terms.

Using this definition we can now develop a definition to compare the size of a set using the following definition called cardinality

***Definition 1.5.2 Cardinality.*** A set $A$ has the same cardinality as a set $B$ if there exists a function $f: A\to B$ that is 1-1 and onto. This is denoted $A\sim B$ 

The onto property is called surjection and it means any image (the elements in the codomain actually being mapped to) is mapped by uniquely one and only one element from the first set, the domain. If we restrict the codomain set to just the image, then this technically means there is an invertible function that can take the image back to the domain.

If the function is surjective and injective, that means there is an invertible function that can take the entire codomain not just a portion of it back to the image. So $A\sim B$ implies there is an inverse function that is also 1-1 and onto so that $B \sim A$.

The important examples to put cardinality in action is to compare the size of $N$ to $Z$ and show that we can create a function to map all of $Z$. Notice that the definition for cardinality just dictates we have to find just one function. To do so, we have the function

$f(n)= (n-1)/2$   if $n$ is odd
$f(n) =-n/2$         if n is even

The book doesn't prove that this function is 1-1 and onto so just take it for granted that $\mathbb{N} \sim \mathbb{Z}$ . The wild thing is that we can map $\mathbb{N}$ to $\mathbb{Q}$ as well. 

A set being a similar size to $\mathbb{N}$ is a special property that we give a definition

***Definition 1.5.5***. Countable. A set $A$ is countable if the set of natural numbers $\mathbb{N}$ is $\mathbb{N}\sim A$ .

We now prove by contradiction that the set of real numbers is NOT countable. Showing this gives some formal mathematical framework to show that the infinitely big set of real numbers is more than the infinitely big set of natural numbers. This proof is done by assuming we have a function that somehow maps 1-1 and onto the real numbers but that this set of real numbers does not satisfy the AoC namely the nested interval property by producing a counter example of a infinitely nested closed set that cannot contain any elements. The nested interval property is for any arbitrary set of nested closed intervals, but we'll invoke a specific case of nested intervals as a specific counterexample of the property not being satisfied and so it violates the AoC.

# Summary of concepts and nuances
- All closed or open interval of real numbers have the same cardinality even if their lengths are different
- ***The set of irrationals is "more infinite" than $\mathbb{Q}$ .*** The set of reals is defined as the union of the rationals and the irrationals. Since the union of countable sets is countable and $\mathbb{Q}$ is countable, the set of irrational numbers is uncountable and a larger cardinality than the rationals. 
# Summary of proof strategies
- ***Prove a set is countable.*** To prove a set is countable, we can demonstrate the following:
	1) $\exists$  a bijective function that maps a domain in $\mathbb{N}$ to the set
	2) The set is a union of countable sets
	3) The set is a subset of a countable set
- ***Finite sets are not countable.*** Countability is defined by the ability for a function to map bijectively from the entire domain of $\mathbb{N}$. If the set is finite, then at some point, we run out of points to keep mapping from $\mathbb{N}$.

# Concepts from exercises
- The majority of the exercises require constructive proofs and are exercises in creativity and to pull mathematical objects out of thin air. This includes:
	- Using existence theorems or properties like the Archimedean property and the well-ordering principle to guarantee the ability to construct or find a certain number
- ***Exercise 1.5.1 (Application of the well-ordering principle).*** The well-ordering principle and the logically equivalent principle of induction is an defined property of natural numbers only and certain subsets of the natural numbers, but It does not apply to countable sets in general. The well-ordering principle does not apply to integers for instance.
- ***Exercise 1.5.2 (The NIP does not apply to $\mathbb{Q}$).*** You can construct closed intervals centered around a irrational number so that no rational numbers is contained in it.
- ***Exercise 1.5.3 (The cardinality of the cartesian product of natural numbers)***. The Cantor triangular array (or the Cantor enumeration array) of natural numbers demonstrates that the ordered pair of natural numbers is countable: $\mathbb{N} \times \mathbb{N}\sim \mathbb{N}$ . The cardinality between the two allows us to show the infinite union of countable sets is countable as [induction cannot prove statements about infinity](Why%20Induction%20Stops%20at%20Infinity.%20The%20Finite-Step%20Fallacy..md)
- ***Exercise 1.5.4 (The cardinality of open and closed intervals and the Hilbert's Grand Hotel technique).*** The cardinality of any arbitrary open intervals are obviously equal but interestingly the cardinality of closed or half-closed intervals is also equal to open intervals. Closed intervals differ from open intervals by a finite number of points, so we have to show that we can always "shift" the infinite open set a countable number of times to make room for the finite points. The shifting to make room for a countable number of elements is called the Hilbert Grand Hotel Technique and is summarized as follows:
	1) Produce a sequence (function of the natural numbers) contained in the open interval that follows some rule for a index $n\in \mathbb{N}$ 
	2) We can map an $m$ number of points to the sequence in 1) by mapping it to the first few terms $m$ and shifting the mapping of the other points down to $n+m$
	The concept is that the size of the real numbers always gives us room to add a countable number of points.
- ***Exercise 1.5.4 (Equipollence and countability is an equivalence relation).*** Because we have the following 3 relationships, Cantor's relation between infinite sets is an equivalence relation:
	1) ***Reflexivity.*** A set has the same cardinality with itself
	2) ***Symmetry.*** If a set has the same cardinality as another set, then the converse is true
	3) ***Transitivity.*** 


# Definitions

***Definition 1.5.1.*** a function $f: A\to B$ has a one-to-one (1-1, injective)  if $a_1\ne a_2$ then $f(a_1) \ne f(a_2)$. The function is "onto" (surjective) if for every $b \in B$ there exists an $a \in A$ such that $f(a) = b$ 

***Definition 1.5.2 Cardinality.*** A set $A$ has the same cardinality as a set $B$ if there exists a function $f: A\to B$ that is 1-1 and onto. This is denoted $A\sim B$ 

***Definition 1.5.5***. Countable. A set $A$ is countable if the set of natural numbers $N$ is $N\sim A$ .

# Theorems

***Theorem 1.5.6 (The Rationals are countable and the reals are uncountable)***

***Theorem 1.5.7 (The subset of a countable set is also countable or finite).***

***Theorem 1.5.8 (Countability is preserved under union).***


