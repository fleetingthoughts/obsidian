---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 5.1 Eigenvalues and Eigenvectors]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch5
date_created: 2026-09-19
---
Prove that the trace can be determined from the characteristic polynomial of a matrix
#### Notes
the characteristic polynomial can be expanded as $f(t) = (A_{11}-t)(A_{22}-t)\cdots(A_{nn}-t) + q(t)$, where $q(t)$ is a polynomial of degree at most $n-2$.

- Because $q(t)$ has a maximum degree of $n-2$, it does not contribute to the $t^{n-1}$ term of the polynomial.
    
- Therefore, the $t^{n-1}$ term must come entirely from expanding the product of the diagonal elements: $(A_{11}-t)(A_{22}-t)\cdots(A_{nn}-t)$.
    
- To form a $t^{n-1}$ term during this expansion, we must multiply $-t$ from $n-1$ of the factors by the constant $A_{ii}$ from the single remaining factor.
    
- Summing these possibilities across all $n$ factors gives: $A_{11}(-t)^{n-1} + A_{22}(-t)^{n-1} + \dots + A_{nn}(-t)^{n-1}$.
    
- This factors nicely into $(\sum_{i=1}^n A_{ii})(-1)^{n-1}t^{n-1}$.
    
- By definition, the sum of the diagonal entries $\sum_{i=1}^n A_{ii}$ is the trace of the matrix, written as $\text{tr}(A)$.
    
- Equating this to our coefficient $a_{n-1}$, we get $a_{n-1} = \text{tr}(A)(-1)^{n-1}$.
    
- Multiplying both sides of the equation by $(-1)^{n-1}$ gives the final result: $\text{tr}(A) = (-1)^{n-1}a_{n-1}$.
