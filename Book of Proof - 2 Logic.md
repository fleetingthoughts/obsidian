---
parent: "[[Book of Proof 3rd ed. - Richard Hammond]]"
tags:
  - mathematical_logic
  - richard_hammond
  - math
  - proof
---
# 2.1 Statements
- Statements are either definitely true or definitely false
- Statements can be represented by symbols
- If a statement $P$ says something about a variable x, we can write $P(x)$ 
# 2.2 And, Or, Not
- $P$ AND $Q$ is denoted $P \land Q$ 
- $P$ OR $Q$ is denoted $P \lor Q$ 
- NOT $P$ or the negation of $P$ is denoted $\lnot P$ 

# 2.3 Conditional Statements

The conditional statement "If $P$ then $Q$" is denoted by $P \implies Q$. This phrase has several different grammatical ways of being stated such as all the following:

- $P$ implies $Q$.
- If $P$, then $Q$ .
- $Q$ if $P$.
- $Q$ whenever $P$.
- $Q$, provided that $P$.
- Whenever $P$, then also $Q$.
- <u> $P$ is a sufficient condition for $Q$.</u>
- <u> For Q , it is sufficient that P.</u>
- <u> Q is a necessary condition for P</u>
- For P, it is necessary that Q.
- P only if Q.
Of the above list, one of the most common is relating the statements by "necessity and sufficiency".  In this case $P \implies Q$ means $P$ is <u>sufficient</u> for $Q$ or it can also be stated $Q$ is <u>necessary</u> for $P$ . Below is the truth table showing the relationship for sufficiency. Notice that if $P \implies Q$ , $P$ is not an absolute requirement for $Q$ for indeed $Q$ can be true without $P$ being true.
![](Pasted%20image%2020251031000353.png)
# 2.4 Biconditional Statements
It should be noted that $P \implies Q$ is not the same as $Q \implies P$  for one is called the <u>converse</u> of the other. In other words, a condition and its converse express entirely different things.
We now speak of the situation where $(P\implies Q)\land (Q \implies P)$ which is denoted and grammatically referred to as:
- $P\iff Q$ 
- "$P$ if and only if $Q$." (the most common one)
- "$P$ is a necessary and sufficient condition for $Q$" (necessity and sufficiency way of stating it)
- "$P$ is equivalent to $Q$"
- "If $P$, then $Q$, and conversely"
![](Pasted%20image%2020251031001105.png)
# 2.6 Logical Equivalence
Two statements are logically equivalent if their truth values match identically line-for-line in a truth table. As an example we have that the following two statements are equivalent:
$$P \implies Q = (P \land Q) \lor (\lnot P \lor \lnot Q)$$
![](Pasted%20image%2020251031002237.png)
A certain pair of logically equivalent statements have special names got the DeMorgan's laws:

***Fact 2.1 (DeMorgan's Laws).*** 
1. $\lnot (P \lor Q) = (\lnot P \land \lnot Q)$ 
2. $\lnot (P \land Q) = (\lnot P \lor \lnot Q)$ 
![](Pasted%20image%2020251031003047.png)
We also find that these logical operators have the usual algebraic commutative, distributive, and associative laws:
![](Pasted%20image%2020251031003304.png)
But we must be careful with these properties for example, a mix of $\land$ and $\lor$ operators are NOT commutative for indeed $P\land (Q \lor R) \ne (P \land Q) \lor R$ 
# 2.7 Quantifiers
To make statements that apply to a very broad or even an infinite set, our current set of operators isn't sufficient for to make a statement about the infinite set of integers $X = \{ x_1, x_2, ...\}$ would require an infinite number of logical operators. To over come this, we introduce quantifier symbols
***Definition 2.1 (Quantifiers).*** The symbols $\forall$ and $\exists$ are called quantifiers:
- $\forall$ stands for the phrase "For all" or "for every" or "For each"
- $\exists$ stands for the phrase "There exists a" or "There is a"
As an example, the phrase "For every $n \in Z$, $2n$ is even" can be expressed as follows if we have the statement $E(x)$ means $x$ is even:
$$\forall n \in Z, E(2n)$$
These symbols are referred to as quantifiers because they refer in some sense to some quantity (or all) the variables. The symbol $\forall$ is called the <u>universal quantifier</u> and results in a <u>universally quantified statement</u> and $\exists$ is called the <u>existential quantifier</u> and results in an <u>existentially quantified statement</u>. 

Note that the order of quantifiers has significance for indeed the statement $\forall x \in R, \exists y \in R, y^3 =x$ is a true statement but reversing the order of a quantifiers results in a false statement: $\exists y \in R, \forall x \in R, y^3 = x$.
# 2.8 More on Conditional Statements
A brief aside on a common truncation used by mathematicians concerning implications between open statements

Open statements are statements $P$ on some variable $x$  that are only true for certain values of  denoted as $P(x)$. These statements are open because they are NOT generally true but are only true for certain cases of $x$. Importantly this leads to other open sentences such as $P(x) \implies Q(x)$ may itself be an open statement that is true for certain $x$. But often times mathematicians don't care for these kinds of open statements. Whenever we have two open statements concerning elements in some set $x \in X$, mathematicians are often in more general statements that concern all the variables of interest such as $\forall x \in X, P(x) \implies Q(x)$. This is used so often that they simply truncate it to $P(x) \implies Q(x)$. This leads to the following interpretation of conditional statements.

***Definition 2.2 (truncation of of open statements).*** If $P$ and $Q$ are statements or open sentences, then "If $P$, then $Q$," is a statement. This statement is equivalent to $P$ being sufficient for $Q$. 

So whenever see statements $P$ or $Q$ that are perhaps only true for certain variables, (i.e. if they are open statements), it is by convention understood that $P \implies Q$ does not refer to another open statement, but instead a logical statement that is absolutely true or absolutely false for all elements $x \in X$ that are of interest.
# 2.9 Translating English to Symbolic Logic

***Fact 2.2. (A Universally Quantified Statement as a Conditional Statement).*** Suppose $X$ is a set and $Q(x)$ is a statement about $x$ for each $x \in X$. The following statements mean the same thing:
- $\forall x \in X, Q(x)$
- $(x\in X)\implies Q(x)$
# 2.10 Negating Statements
DeMorgan's laws are useful to consider to rephrase the negation of statements.

When quantifiers are involved, note that:
1) $\lnot (\forall x\in X, P(x)) = \exists x \in X, \lnot P(x)$
2)  $\lnot (\exists x \in X, P(x)) = \forall x\in X, \lnot P(x)$

When conditional statements are involved, observation of the truth table shows that there is one way for $(P \implies Q)$ to be false which is :
$$\lnot (P\implies Q) = P \land \lnot Q$$
# 2.11 Logical Inference