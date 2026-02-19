---
tags:
  - "#math"
  - "#richard_courant"
  - "#real_analysis"
  - "#calculus"
date_created: 2026-02-17
parent: "[[Introduction to Calculus and Analysis I]]"
---
A review of some fundamentals for real analysis. The relevant concepts that this chapter goes over:
- monotonic functions and one-to-one mapping
- Even functions $f(-x)=f(x)$
- Odd Functions: $f(-x)=-f(x)$

***Continuity of a Univariate Function (p.33)*** The function $f(x)$ is continuous at $f(x_o)$ if for any arbitrary $\epsilon >0$, there exists a $\delta >0$ such that:
$$|f(x)-f(x_o)|<\epsilon \text{\quad when\quad}|x-x_o|<\delta$$
Continuity can be thought of in terms of a neighborhood of a point as follows: for any arbitrary $\epsilon$-neighborhood $J$ of point $y_0=f(x_0)$ (i.e. the interval $(y_o-\epsilon, y_o+\epsilon)$), we can find a $\delta$-neighborhood of $x$ that maps to $J$

The author goes through examples to prove the continuity of a function. In general, the strategy will be to describe an upper bound or equality of the function in terms of $|x-x_o|$. 

The $\delta$ in the definition of continuity is referred to as the "modulus of continuity", and we define different types of continuity on the way way $\delta$ changes with $\epsilon$.

***Definition of Uniformly Continuous (p.41).*** A function $f:x\to y$ is uniformly continuous if the modulus of continuity only depends on the choice of $\epsilon>0$ . That is we can determine $\delta =\delta(\epsilon)$ 

***Theorem on sufficient conditions for a Uniformly continuous function(p.42).*** Any closed and bounded interval is uniformly continuous in that interval.

***Definition of Lipschitz Continuity (p.43).*** A function $y=f(x)$ is considered Lipschitz continuous if the modulus of continuity is directly proportional to the choice of $\epsilon>0$, that is, $\delta(\epsilon)=\frac{\epsilon}{L}$ :
$$|f(x)-f(x_0)|\le L|x_2-x_1| < \epsilon \text{\quad for\quad}L\in \mathbb{R}$$
***Definition of Holder-Continuous Function (p.44).*** A function $f(x)$ is considered Holder continuous if the modulus of continuity depends on the choice of $\epsilon>0$ by $\delta=L^{-1/a}\epsilon^{1/a}$ or in other words:
$$|f(x)-f(x_0)| \le L|x-x_o|^a<\epsilon$$
A property of continuous functions is the fact that it has no "jumps" so that if it passes through any two numbers, it must also have gone through all the numbers in between.
***Intermediate Value Theorem (p.44)***. Given a function $f(x)$ that is continuous at every point in the interval $(a,b)$. Let $\theta$ be a number in $(f(a), f(b))$, then there must exist a number $\gamma$ such that $a< \gamma < b$ so that $\theta = f(\gamma)$.

 In the definition of continuity, we are effectively determining whether there's a function that maps our choice of $\epsilon>0$ to $\delta$ (i.e. find $\delta(\epsilon)$ ) Note that this does not mean the converse is true, that is, for function that is continuous by our original definition, given a $\delta>0$ we may not necessarily find a $\epsilon$ . We for instance cannot reverse the roles of $\delta$ and $\epsilon$ in the definition of continuity as :

***Definition of Continuity that is not equivalent*** Given a $\delta>0$, there exists a $\epsilon$ such that:
$$|x-x_o|<\delta \text{\quad when\quad} |f(x)-f(x_o)|<\epsilon$$
A counter-example of a function that is continuous by the original definition but not this definition is the continuous function $f(x)=c$. The case where this alternate definition does hold is if $f(x)$ is an invertible function. The nuance here is that in the original definition of continuity, the modulus forced the $f(x)$ to be close to $f(x_o)$ (i.e. $|x-x_o| < \delta \implies |f(x)-f(x_o)|$)

***Theorem on the Continuity of Invertible Functions (p.46).*** Given a function $y=f(x)$ that is monotonically increasing or decreasing in the interval $[x_1,x_2]$, the inverse function $x=g(y)$ must be continuous in the interval $[y_1= f(x_1), y_2=f(x_2)]$. The [Proof of the Continuity of Inverse Functions](Proof%20of%20the%20Continuity%20of%20Inverse%20Functions.md) is the case where our alternate definition is permissible.
	
