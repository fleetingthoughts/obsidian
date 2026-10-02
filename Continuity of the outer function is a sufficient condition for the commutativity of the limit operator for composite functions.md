---
parent: "[[Understanding Analysis - 4.3 Continuous Functions]]"
tags:
  - "#flashcard"
  - micro/math/abbott/ch4
date_created: 2026-09-27
---
Prove: Let $f: A \to B$ and $g: B \to \mathbb{R}$. If $\lim_{x \to c} f(x) = q$ and $g$ is continuous at $q$, then $\lim_{x \to c} g(f(x)) = g(q)$
#### Notes
The theorem in image_dc82f7.png requires proving that for every $\epsilon > 0$, there exists a $\delta > 0$ such that if $0 < \vert{}x - c\vert{} < \delta$, then $\vert{}g(f(x)) - g(q)\vert{} < \epsilon$. The macro skeleton of this proof works backward from the outer function $g$ to the inner function $f$ using the $\epsilon-\delta$ definitions.

**Phase 1: Unpack the Outer Function (Continuity of $g$)**

* **Given:** $g$ is continuous at $q$.


* **Definition:** Let $\epsilon > 0$ be given. Because $g$ is continuous at $q$, there exists some $\eta > 0$ such that for all $y \in B$, if $\vert{}y - q\vert{} < \eta$, then $\vert{}g(y) - g(q)\vert{} < \epsilon$.
* *Strategic Purpose:* This establishes the final target inequality. The variable $y$ represents the output of the inner function, which will eventually be substituted with $f(x)$.

**Phase 2: Unpack the Inner Function (Limit of $f$)**

* **Given:** $\lim_{x \to c} f(x) = q$.


* **Definition:** For any chosen output tolerance, there exists a $\delta > 0$ such that if $0 < \vert{}x - c\vert{} < \delta$, then $\vert{}f(x) - q\vert{}$ is less than that tolerance.
* *Strategic Purpose:* We must constrain $f(x)$ so that its output falls perfectly within the $\eta$-neighborhood required by the outer function $g$ in Phase 1.

**Phase 3: The Synthesis (Linking the Definitions)**

* **Action:** Apply the limit definition of $f$ using $\eta$ (from Phase 1) as the chosen tolerance.
* **Logic:** Because $\lim_{x \to c} f(x) = q$, there must exist a $\delta > 0$ such that if $0 < \vert{}x - c\vert{} < \delta$, then $\vert{}f(x) - q\vert{} < \eta$.


* **Conclusion:** By letting $y = f(x)$, we have satisfied the condition $\vert{}y - q\vert{} < \eta$. As established in Phase 1, this guarantees that $\vert{}g(f(x)) - g(q)\vert{} < \epsilon$. This successfully completes the $\epsilon-\delta$ definition for $\lim_{x \to c} g(f(x)) = g(q)$.
    
- By the sequential criterion for limits, $\lim f(x_n) = q$.
    
- Apply the sequential criterion for continuity to $g$ at $q$ to deduce that the image sequence converges: $\lim g(f(x_n)) = g(q)$.
    
- Conclude via the sequential criterion for limits that the functional limit $\lim_{x \to c} g(f(x))$ exists and equals $g(q)$.
