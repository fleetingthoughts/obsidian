---
parent: "[[Understanding Analysis - 4.3 Continuous Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch3
date_created: 2026-09-19
---
Prove: If $f_1, f_2, \dots, f_n$ are continuous functions, then $g(x) = \max\{f_1(x), f_2(x), \dots, f_n(x)\}$ is a continuous function.
#### Notes
- Establish the base case $n=2$ by expressing $\max\{f_1(x), f_2(x)\}$ using the algebraic identity $\frac{1}{2}[(f_1(x)+f_2(x)) + \vert{}f_1(x)-f_2(x)\vert{}]$.
    
- Apply the Algebraic Continuity Theorem to verify the continuity of the sum and difference of continuous functions.
    
- Apply the composition theorem for continuous functions to verify the absolute value term is continuous, thereby proving the base case.
    
- Formulate an inductive hypothesis for $k$ continuous functions.
    
- Express the $k+1$ case as $\max\{\max\{f_1, \dots, f_k\}, f_{k+1}\}$ and apply the base case to complete the induction.
