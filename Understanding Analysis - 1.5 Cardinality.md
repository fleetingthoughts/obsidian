---
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
tags:
  - math
  - stephen_abbot
  - understanding_analysis
  - real_analysis
date_created:
---

We explore the big brain of Georg Cantor who found a way to compare infinities and show how some infinities are larger than others. In this section we develop the following:
- A method and definition to compare the "size" of a set to another set
- Use this method to show that $N$ is the same "size" as $Z,Q$ but $R$ is "larger" than $N$ which implies that there are way more irrational numbers than rational numbers

We use the idea of a function's 1-1 mapping to compare the size of a set by saying that a set can be thought of as equal "size" to another set if there exists a function such that every element in that set can be mapped out. 

We first define the tools we will use.

***Definition 1.5.1.*** a function $f: A\to B$ has a one-to-one (1-1, injective)  if $a_1\ne a_2$ then $f(a_1) \ne f(a_2)$. The function is "onto" (surjective) if for every $b \in B$ there exists an $a \in A$ such that $f(a) = b$ 

A function being [1-1](Surjectivity,%20Injectivity,%20and%20Bijectivity.md) means that if an element in $B$ is mapped, then precisely only one unique $a$ gets mapped by it. Every value in the domain gets its own unique value in the range and no two values in the domain map to the same range value. And [onto](Surjectivity,%20Injectivity,%20and%20Bijectivity.md)] means that the image of the function contains all of $B$. This is also called a surjective function and the implication is that EVERY element of  $B$ is being mapped. The set containing being mapped to, $B$, is called the codomain, and the elements in $B$ that are actually mapped are referred to as the  $image$ of the function, so for a surjective function, the entire codomain $B$ basically becomes the image. 

If a function $f: A\to B$  is 1-1 and onto (surjective and injective) then it is bijective. This implies that the function $f$ is invertible such that there exists another function $f^{-1}$ such that $f^{-1}: B \to A$ 

Note there is another term called the range of a function which is a bit ambiguous for whether it refers to the image or the codomain. Image and codomain are the more precise terms.

Using this definition we can now develop a definition to compare the size of a set using the following definition called cardinality

***Definition 1.5.2 Cardinality.*** A set $A$ has the same cardinality as a set $B$ if there exists a function $f: A\to B$ that is 1-1 and onto. This is denoted $A\sim B$ 



The onto property is called surjection and it means any image (the elements in the codomain actually being mapped to) is mapped by uniquely one and only one element from the first set, the domain. If we restrict the codomain set to just the image, then this technically means there is an invertible function that can take the image back to the domain.

If the function is surjective and injective, that means there is an invertible function that can take the entire codomain not just a portion of it back to the image. So $A\sim B$ implies there is an inverse function that is also 1-1 and onto so that $B \sim A$.

The important examples to put cardinality in action is to compare the size of $N$ to $Z$ and show that we can create a function to map all of $Z$. Notice that the definition for cardinality just dictates we have to find just one function. To do so, we have the function

$f(n)= (n-1)/2$   if $n$ is odd
$f(n) =-n/2$         if n is even

The book doesn't prove that this function is 1-1 and onto so just take it for granted that $N \sim Z$ . The wild thing is that we can map $N$ to $Q$ as well. 

A set being a similar size to $N$ is a special property that we give a definition

***Definition 1.5.5***. Countable. A set $A$ is countable if the set of natural numbers $N$ is $N\sim A$ .

We now prove by contradiction that the set of real numbers is NOT countable. Showing this gives some formal mathematical framework to show that the infinitely big set of real numbers is more than the infinitely big set of natural numbers. This proof is done by assuming we have a function that somehow maps 1-1 and onto the real numbers but that this set of real numbers does not satisfy the AoC namely the nested interval property. The nested interval property is for any arbitrary set of nested intervals, but we'll invoke a specific case of nested intervals as a specific counterexample of the property not being satisfied and so it violates the AoC.




