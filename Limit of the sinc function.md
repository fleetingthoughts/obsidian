---
parent: "[[Introduction to Calculus I by Fritz and Courant - 1.7 Discussion of the Concept of Limit]]"
tags:
  - "#flashcard"
  - micro/math/courant_calc1/ch1
  - calculus
  - richard_courant
date_created: 2026-07-24
---
What is limit of the $sinc(x)$ function as $x$ goes to $0$ and how is it proven geometrically? Use this result to then prove the following limits:
- $\lim\limits_{x \to 0}\frac{tan(x)}{x}$
- $\lim\limits_{x \to 0}\frac{1-\cos x}{x}$
- $\lim\limits_{x \to 0}\frac{1-\cos x}{x^2}$
#### Notes
**The Limit:**
$$\lim_{x \to 0} \frac{\sin x}{x} = 1$$
**Geometric Proof Summary (Squeeze Theorem):**

On a unit circle with a small angle $x > 0$ (in radians), compare three areas:
1. **Inner Triangle:** Base 1, height $\sin x \rightarrow$ Area $= \frac{\sin x}{2}$
2. **Circular Sector:** Radius 1, angle $x \rightarrow$ Area $= \frac{x}{2}$
3. **Outer Triangle:** Base 1, height $\tan x \rightarrow$ Area $= \frac{\tan x}{2}$
Visually, the areas form an inequality:
$$\frac{\sin x}{2} < \frac{x}{2} < \frac{\tan x}{2}$$
Multiply by $\frac{2}{\sin x}$:
$$1 < \frac{x}{\sin x} < \frac{1}{\cos x}$$
Take reciprocals (flipping the inequalities):
$$\cos x < \frac{\sin x}{x} < 1$$
By the **Squeeze Theorem**, as $x \to 0$, both bounding functions ($\cos x$ and $1$) approach $1$. Therefore, the middle term also converges to $1$.

### 2. Derived Limits
**Proof 1: Tangent Limit**
Rewrite $\tan x$ as $\frac{\sin x}{\cos x}$ and evaluate:
$$\lim_{x \to 0} \frac{\tan x}{x} = \lim_{x \to 0} \left( \frac{\sin x}{x} \cdot \frac{1}{\cos x} \right)$$
$$= (1) \cdot \left(\frac{1}{1}\right) = 1$$
**Proof 2: Cosine Limit (Linear denominator)**
Multiply the numerator and denominator by the conjugate $(1+\cos x)$, then apply the Pythagorean identity $(1 - \cos^2 x = \sin^2 x)$:
$$\lim_{x \to 0} \frac{1-\cos x}{x} = \lim_{x \to 0} \frac{1-\cos^2 x}{x(1+\cos x)}$$
$$= \lim_{x \to 0} \left( \frac{\sin x}{x} \cdot \frac{\sin x}{1+\cos x} \right)$$
$$= (1) \cdot \left(\frac{0}{1+1}\right) = 0$$
**Proof 3: Cosine Limit (Squared denominator)**
Using the same conjugate method as above:
$$\lim_{x \to 0} \frac{1-\cos x}{x^2} = \lim_{x \to 0} \frac{1-\cos^2 x}{x^2(1+\cos x)}$$
$$= \lim_{x \to 0} \left( \left(\frac{\sin x}{x}\right)^2 \cdot \frac{1}{1+\cos x} \right)$$
$$= (1)^2 \cdot \left(\frac{1}{1+1}\right) = \frac{1}{2}$$
