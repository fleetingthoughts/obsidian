---
tags:
  - math
  - real_analysis
date_created: 2026-03-26
parent: "[[Understanding Analysis 2nd ed. - Abbot, Stephen]]"
---
We define the property of continuity that will be used to counter the pathological functions. In this chapter the following is done:
- The definition of continuity and how it is distinguished from the definition of the functional limit.
- The nuance between the definitions of continuity and the definition of a functional limit in that the target point in the domain does NOT need to be a limit point for continuity but a functional limit requires it.
- The equivalent conditions for continuity, particularly in convergence of sequences, and when the functional limit at a point is equivalent to the continuity at the point
- How to disprove continuity by disproving any of the aforementioned equivalent statements
- The algebraic properties of continuous functions

The definition for continuity is provided in ***Definition 4.3.1.*** While the definition looks very similar to that of the functional limit, there is one distinguishing feature:
- We only require the target point $c$ to be in the domain of $A$
- $c$ is not defined to be a limit point of $A$ while in the definition of the [functional limit](Understanding%20Analysis%20-%204.2%20Functional%20Limits.md), we require it to be a limit point
As such it is tempting to say that if $f(x)$ is continuous at $x=c$ then since $c \in A$ , it would be wrong to assume $\lim\limits_{x \to c}f(x)=f(c)$ because $c$ may not be a limit point. The only difference in the definitions is whether $c$ is a limit point (functional definition) or $c$ is simply in the domain and is an isolated point instead. The scenarios are as follows:
1) If $c$ is neither a limit point or isolated point, then neither continuity (not in $A$) or functional limit (not a limit point) apply.
2) If $c$ is not a limit point but is an isolated point, then we automatically don't have a functional limit because the definition requires it. But if $c$ is an isolated point then it is [vacuously true](The%20Empty%20Set%20and%20Vacuous%20Truths.md) that the function is continuous at $x=c$ 
3) If $c$ is a limit point, then as derived in ***Theorem 4.3.2***, continuity at $x=c$ implies a functional limit at $c$ as well. 

Points 2) and 3) are worth expounding. In 2), it was noted that it was always true that a function is continuous at its isolated point, this is because in our application of the continuity criteria $|x-c|<\delta \implies 0<|f(x)-f(c)|<\epsilon$, we note that $|x-c| = {\emptyset}$. In this case, it is an empty set so that $|f(x)-f(c)|<\epsilon$ become [vacuously true](The%20Empty%20Set%20and%20Vacuous%20Truths.md) since we can't find any counter examples of $x$ that defy this criteria. Point 3), is the same condition as for functional limits in which the definition of continuity in "trapping" all points to the target point $c$. In our sequential formulation in ***theorem 4.3.2.***, if the $c$ is not a limit point, then the statement is still vacuously true as we have no sequences in the domain that converge to the isolated point. Point 4) is then a result of us "filling" in the definition of continuity by requiring $c\in A$ to be a limit point that was in the definition of the functional limit.

Since all 4 statements in ***Theorem 4.3.2*** are equivalency statements (if and only if), then it holds that if any of those conditions are false, we no longer have continuity. ***Corollary 4.3.3*** Therefore provides a condition to disprove continuity.

Some interesting notes from exercises:
- [[Continuity at a limit point included in the domain is not equivalent to the functional limit at a point included in the domain]]


# Definitions
***Definition 4.3.1 (Continuity)*** A function $f:A \to R$ is "continuous at a point $c\in A$"  if for all $\epsilon>0$, there exists a $\delta >0$ such that: $$|f(x)-f(c)| <\epsilon \text{\quad if \quad} |x-c|<\delta$$
# Theorems
***Theorem 4.3.2 (Equivalent statements to the condition of continuity).*** Let $f: A\to \mathbb{R}$, and let $c\in A$. The function $f$ is continuous at $c$ if and only if any of the three conditions is met:
1) For all $\epsilon>0$ there exists a $\delta$ such that when $|x-c|< \delta$ then $|f(x)-f(c)|<\epsilon$ and $x\in A$.
2) For all $V_{\epsilon}(f(c))$ there exists a $\delta$ such that whenever $x\in V_\delta(c)$ and $x\in A$ then $f(x) \in V_{\epsilon}(f(c))$ 
3) If $(x_n) \to c$ with $x_n \in A$ then $f(x_n) \to c$
If $c$ is a limit point of $A$, then the above conditions are equivalent to:
4) $\lim\limits_{x\to c}f(x)=f(c)$ 


***Corollary 4.3.3 (Criterion for Discontinuity).*** Let $f: A\to \mathbb{R}$, and let $c\in A$ be a limit point of $A$. If there exists a sequence $(x_n)\subseteq A$ where $(x_n)\to c$ such that $f(x_n)$ does not converge to $f(c)$, then $f$ is not continuous at $x=c$ 

***Theorem 4.3.4 (Algebraic Continuity Theorem).*** Assume $f: A\to R$ and $g: A\to R$ are continuous at point $c\in A$. Then we have the following properties:
- Scalar multiplication: $kf(x)$ is continuous at $c$ for all $k\in \mathbb{R}$
- Addition of continuous functions: $f(x)+g(x)$ is continuous at $c$
- Multiplication of continuous functions: $f(x)g(x)$ is continuous at $c$
- Division of continuous functions: $f(x)/g(x)$ is continuous at $c$, provided the quotient is defined