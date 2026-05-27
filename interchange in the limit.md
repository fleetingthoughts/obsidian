---
tags:
date_created: "2026-05-27"
---


Let’s redo the rigorous justification for that limit interchange using only the exact symbols Courant uses in his text: $x, y, x_1, y_1, f(x),$ and $\phi(y)$.

---

## The Justification Using Courant's Notation

We want to rigorously justify the step at the bottom of the page:  
$$\lim_{x_1 \to x} \frac{x_1 - x}{y_1 - y} = \lim_{y_1 \to y} \frac{x_1 - x}{y_1 - y}$$

To do this, we apply the Limit of a Composite Function Theorem directly to Courant's expressions. Let the difference quotient be a function of $y_1$:  
$$\text{Difference Quotient} = \frac{\phi(y_1) - \phi(y)}{y_1 - y} = \frac{x_1 - x}{y_1 - y}$$

When viewed as a composite function depending on $x_1$ (since $y_1 = f(x_1)$), the theorem states that changing the limit variable from $x_1 \to x$ to $y_1 \to y$ is valid if and only if two specific conditions are satisfied:

## Condition 1: The Inner Limit Must Exist

As the outer variable $x_1$ approaches $x$, the inner variable $y_1$ must approach $y$.

- Courant’s Justification: $\lim_{x_1 \to x} f(x_1) = f(x) = y$.
- Why it holds: This is guaranteed because $y = f(x)$ is explicitly stated to be continuous.

## Condition 2: No Premature Reaching of the Limit Value

The inner function $y_1 = f(x_1)$ must never actually equal $y$ when $x_1 \neq x$ near the point of interest. If it did equal $y$, the denominator $(y_1 - y)$ would become zero, and the limit would be undefined.

- Courant’s Justification: The hypothesis states that either $f'(x) > 0$ or $f'(x) < 0$ throughout the interval.
- Why it holds: A derivative that never changes sign means $f(x)$ is strictly monotonic (strictly increasing or decreasing). Strictly monotonic functions are one-to-one. Therefore, if $x_1 \neq x$, then $f(x_1) \neq f(x)$, which guarantees that $y_1 \neq y$.

---

## Conclusion

Because both conditions of the composite limit theorem are fulfilled by Courant's hypotheses, the variable swap is mathematically rigorous:  
$$\lim_{x_1 \to x} \frac{x_1 - x}{y_1 - y} \equiv \lim_{y_1 \to y} \frac{x_1 - x}{y_1 - y}$$

Would you like to move on to the next step of Courant's proof where he evaluates this inverted limit, or do you want to look at another theorem from this chapter?

The formal rule governing this operation is known as the ==Change of Variables Theorem for Limits== (or the Limit of a Composite Function Theorem).

---

## Theorem: Change of Variables for Limits

Let $f$ and $G$ be real-valued functions. Let $x$, $y$, and $L$ be real numbers.

## Hypotheses (The Conditions)

The interchange of symbols is valid if and only if the following conditions are met:

1. Inner Limit Exists:  
    $$\lim_{x_1 \to x} f(x_1) = y$$
2. Outer Function is Continuous:  
    The function $G$ is continuous at $y$, meaning:  
    $$\lim_{y_1 \to y} G(y_1) = G(y)$$

## Conclusion (The Mathematical License)

If both conditions are true, then you are legally allowed to change the limit variables:  
$$\lim_{x_1 \to x} G(f(x_1)) = \lim_{y_1 \to y} G(y_1) = G(y)$$

---

## The Alternative "Deleted Neighborhood" Condition

If the outer function $G$ is not continuous at $y$, you can still perform this symbol change under one specific exception:

- The Rule: The inner function $f(x_1)$ must never actually hit the value $y$ when $x_1$ is near $x$.
- The Formal Phrasing: There must exist a punctured neighborhood of $x$ where $f(x_1) \neq y$ for all $x_1 \neq x$.

If either Continuity or this Punctured Neighborhood rule holds, the symbol swap is mathematically true. If both are broken, the operation fails completely.

---

If you want to see exactly how this works in practice, tell me:

- A specific limit problem you are trying to solve.
- Or if you want a numerical example where this rule breaks down.

I can break down the math for you step by step!