parent:[_Fleeting MOC](_Fleeting%20MOC.md)  [Understanding Analysis - Abbot, Stephen 2nd Ed](Understanding%20Analysis%20-%20Abbot,%20Stephen%202nd%20Ed.md) 
tag: #textbook #math #stephen_abbot #understanding_analysis

Now we arrive at the formalization of mathematics summarizing the work done by the following people:
- Augustin Louis Cauchy
- Berhard Bolzano
- Niels Henrick Abel
- Peter Lejeune Dirichlet
- Karl Weiesrstrass
- Bernhard Riemann
Each of these people help provide a more concrete definitions and axioms from which we can formulate the mathematical concepts that were informally developed previously such as the majority of calculus from the "infinitesimally small" quantities from Newton and Leibnitz's time

We assume that $R$ is an ordered field which contains $Q$ as a subfield (until explored in section 8). This lets us perform the basic algebraic and inequality math on any elements within the set. We now formulate the Axiom of Completeness (AoC)

***Axiom of Completeness***. **Every nonempty set of real numbers that is bounded has a least upper bound**

To develop some understanding of this. We first need to understand what the least upper bound is which is also referred to as the supremum:

***Definition 1.3.1***. A set $A$ $\subseteq$ $R$ is bounded above if there exists a number $b$ $\in$ $R$ such that $a\le b$ for all $a \in A$ . The number $b$ is called an upper bound for $A$. 

***Definition 1.3.2***. A real number $s$ is the least upper bound for a set $A \subseteq R$ if it satisfies the following two conditions for all $a \in A$ :
1) $a \le s$. $s$ is an upper bound for all $A$ 
2) if any other $b$ is an upper bound for $A$ then $s \le b$ 

The least upper bound $s$ of a set $A$ is denoted $s = sup(A)$ but it is archaically denoted $s=lub(A)$ as well. An analogous greatest lower bound or infimum denoted $inf(A)$ can be defined as well. 

The supremum can be thought of as the hypothetical maximum that A can approach (like a limit) but is not necessarily an element in the set. All maximums of a set are supremum but not all supremum are maximum which can easily be seen when considering the maximum and supremum for an open and closed bounded interval on the real line such as $\{x\in R: 0\le2\}$  which has the maximum  and supremum 2 and $\{x\in R: 0\lt 2\}$  which doesn't have a maximum but has a supremum of 2

Armed with these definitions, we see that the AoC essentially gives us an inequality with the supremum with the properties defined in 1.3.2 to do math with.

The AoC axiom and the algebraic manipulation of the $R$ field lets us prove some following properties of infimums and supremums for all bounded subsets $A, B$ of $R$  
- $sup(A+c) = sup(A) +c$  $where$  $\{c+a:a\in A\}$
- $sup(A+B)=sup(A)+sup(B)$ (see exercise 1.3.6 on p. 19)
- $sup(cA)=c*sup(A)$ for $c \gt 0$ (see exercise 1.3.5 on p.19)
- $sup(cA)=c*inf(A)$ and $c*sup(A)=inf(cA)$ for $c \lt 0$ (see exercise 1.3.5 on p.19)

Note that no where in AoC do we postulate the existence of an infimum. All we need is the definition of an infimum, assume the existence of the supremum and apply the property of multiplication by constant on the supremum to produce the infimum.

Property 2) of Definition 1.3.2 of the supremum can be reformulated as this lemma:

***Lemma 1.3.8***. Assume $s\in R$ is an upper bound for $A\in R$ then $s=sup(A)$ if and only if for any arbitrary $\epsilon \gt0$, there exists an element $a\in A$ such that $a \ge s-\epsilon$ . 

Note that the lemma calls for any arbitrary epsilon and that $A$ has to be in the real for 