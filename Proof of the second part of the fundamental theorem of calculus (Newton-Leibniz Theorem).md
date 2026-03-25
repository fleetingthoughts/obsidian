---
tags:
  - proof
  - calculus
  - real_analysis
date_created: 2026-03-24
---
The second part of the mean value theorem shows the general form of all primitive functions (i.e. antiderivatives) of $f(x)$. The proof employs the same strategy as other uniqueness theorems: 
1) Prove existence: show there is at least one solution
2) Assume two solutions of a general form exist and show they are identical directly or by contradiction.
For 1), the first part of the fundamental theorem of calculus guarantees there is at least one solution in the form of the integral, but while the theorem demonstrates all indefinite integrals are primitive functions, not all primitive functions are that specific integral, that is, it is possible there are multiple solutions. 

For 2) The second part of the mean value theorem like [[Proof of the first part of the fundamental theorem of calculus]] employs the mean value theorem. We can instead show that if $F(x)$ and $G(x)$ are two primitive functions of $f(x)$, then we can prove directly what form they take. In Richard Courant's calculus book, the "leap of faith" or informed guess we take is that the primitive functions must only differ by a constant because we guess that all primitive functions must be an indefinite integral with a different lower bound so that they differ by a constant. So we set up the proof by demonstrating the difference between the primitive functions only differ by a constant: $$F'(x)-G'(x)=f(x)-f(x)= 0 \text{\quad for all x}$$
From the mean value theorem, we can show that the function whose derivative results in 0 is a constant, so $F(x)-G(x)=c$ .

