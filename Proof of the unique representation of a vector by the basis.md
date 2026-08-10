---
parent: "[[Linear Algebra by Friedberg, Insel, and Spence - 1.6 Bases and Dimension]]"
tags:
  - "#flashcard"
  - macro/math/friedberg/ch1
date_created: 2026-07-24
---
Prove that a set of vectors is a basis if and only if it uniquely represents any vector in the vector space
#### Notes
- **Forward ($\Rightarrow$):** Assume $\beta$ is a basis. It spans $V$, so any $v \in V$ can be written as $v = \sum a_i u_i$.
    
- To prove uniqueness, assume $v = \sum b_i u_i$.
    
- Subtract the two representations: $0 = \sum (a_i - b_i) u_i$.
    
- Because $\beta$ is linearly independent, all coefficients $(a_i - b_i)$ must equal zero. Thus $a_i = b_i$.
    
- **Reverse ($\Leftarrow$):** Assume unique representation. This implies spanning is trivial. Setting $v=0$ requires all coefficients to be $0$, proving independence.
