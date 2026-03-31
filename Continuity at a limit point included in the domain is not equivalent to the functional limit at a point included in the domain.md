---
tags:
  - math
  - real_analysis
  - calculus
date_created: 2026-03-29
---
Continuity and functional limits are definitions that are close but have a fickle relationship with each other and should be viewed as parallel properties to describe a function's behavior at a point. To illustrate, given a function $f: A\to \mathbb{R}$ if the point $x=c$ is a limit point contained in the domain, then: 
1) continuity implies a functional limit and $\lim\limits_{x\to c}f(x)=f(c)$. 
2) A functional limit at $x=c$ with point $c$ in the domain DOES NOT necessarily imply  $\lim\limits_{x\to c}f(x)=f(c)$ 

We had shown in [Understanding Analysis - 4.3 Continuous Functions](Understanding%20Analysis%20-%204.3%20Continuous%20Functions.md) that 1) is true. It is the extra constraint posed by continuity that forces and $\epsilon -\delta$ behavior around the limit point that makes the following equality true: $\lim\limits_{x\to c}f(x)=f(c)$. The functional limit itself says nothing about what actually happens at the exact point $f(c)$. 

The point to take away is that the functional limit says something about the local property around $x=c$ while continuity says something about the local property and $x=c$ itself.
