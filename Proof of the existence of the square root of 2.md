---
parent: "[[Understanding Analysis - 1.4 Consequences of Completeness]]"
tags:
  - "#flashcard"
  - macro/math/abbott/ch1
  - real_analysis
  - stephen_abbot
  - math
date_created: 2026-07-24
---
Prove the existence of irrational numbers like $\sqrt{2}$  using the axiom of completeness.
#### Notes
- Define the bounded, nonempty set $T = \{t \in \mathbf{R} : t^2 < 2\}$ and invoke the Axiom of Completeness to define the supremum $\alpha = \sup T$.
    
- Rule out $\alpha^2 < 2$: Demonstrate that this assumption allows finding an $n_0 \in \mathbf{N}$ such that $(\alpha + 1/n_0)^2 < 2$. This implies $\alpha + 1/n_0 \in T$, contradicting $\alpha$ as an upper bound.
    
- Rule out $\alpha^2 > 2$: Demonstrate that this assumption allows finding an $n_0 \in \mathbf{N}$ such that $(\alpha - 1/n_0)^2 > 2$. This implies $\alpha - 1/n_0$ is a smaller upper bound for $T$, contradicting $\alpha$ as the least upper bound.
    
- Conclude by trichotomy that $\alpha^2 = 2$, proving the existence of the square root
