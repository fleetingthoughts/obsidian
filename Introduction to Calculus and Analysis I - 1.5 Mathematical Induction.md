---
tags:
  - "#math"
  - "#richard_courant"
  - "#real_analysis"
  - "#calculus"
date_created: 2026-02-19
parent: "[[Introduction to Calculus and Analysis I]]"
---
The principle  of mathematical induction is used to prove a statement that applies to infinite but countable cases. The statement applies to a set that has the same [cardinality](Understanding%20Analysis%20-%201.5%20Cardinality.md) as the natural numbers. The procedure used to prove this is mathematical induction, and while it can be used as a procedure, it follows from a fundamental axiom (The first 5 Peano axioms apparantly lead into it)
***Principle of Mathematical Induction.*** Given a set $S$, if $S$ has the following two properties, then it is the set of Natural numbers:
1) $S$ contains the number 1
2) Whenever $S$ contains a number $r$, then it must also contain $r+1$
And so this gives us a procedure to prove a hypothesis for set of infinitely countable cases. We have to prove that the statement implies it for one case, our base case (i.e. $S$ contains 1). Then we have to show that if it applies to the case $r$, then it must also imply the case $r+1$.

The author goes through some examples of proof by mathematical induction, the results of which are worth remembering:
- [Sum of Squares](Sum%20of%20Squares.md): 
- [Sum of cubes](Sum%20of%20cubes.md)
- [Binomial Theorem](Binomial%20Theorem.md)
- 