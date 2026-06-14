---
parent: "[[_Fleeting]]"
tags:
  - "#fleeting"
date_created: 2026-06-14
---
Here is the finalized weekly schedule. I have integrated six additional questions specifically targeting the integration techniques from Section 3.13 (Trigonometric, Hyperbolic, and Euler irrational algebraic substitutions) across the week.

---

## 🗓️ Day 1

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Logarithmic Differentiation (Section 3.2e, Page 216): Used when variable components are locked inside both the base and the exponent, or when dealing with a massive product of fractional terms. Take a natural log first to convert multiplications into additions and exponents into coefficients.
- The Weierstrass Half-Angle Substitution (Section 3.13b, Page 293): Maps awkward rational combinations of $\sin x$ and $\cos x$ in a denominator into plain algebraic polynomial fractions.
    
    - _Recipe:_ Let $t = \tan(x/2)$. Substitute $\sin x = \frac{2t}{1+t^2}$, $\cos x = \frac{1-t^2}{1+t^2}$, and $dx = \frac{2}{1+t^2}dt$.
    
- Asymptotic Notations (Section 3.7f, Page 253): Used to find which terms dominate a landscape as values explode toward infinity, letting you safely truncate calculations.

## 📝 Quiz Questions

1. Find $\frac{dy}{dx}$ using logarithmic differentiation for:  
    $$y = x^{\sin x}$$
2. Convert this trigonometric integral into a plain rational algebraic function using the half-angle substitution $t = \tan(x/2)$ (do not evaluate the final algebraic integral):  
    $$\int \frac{1}{2 + \cos x} \, dx$$
3. Prove whether this statement is True or False as $x \to \infty$:  
    $$x^3 + 100x^2 \log x = O(x^3)$$
4. Evaluate using integration by parts:  
    $$\int x^2 \ln x \, dx$$
5. (NEW - Sec. 3.13b) Completely evaluate using the Weierstrass half-angle substitution:  
    $$\int \frac{1}{1 + \sin x + \cos x} \, dx$$

---

## 🗓️ Day 2

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Fermat’s Optimization Rule (Section 3.6b, Page 238): Interior local extrema occur where the tangent line flattens out entirely, meaning the instantaneous rate of change drops precisely to zero.
- Hyperbolic Functions Foundations (Section 3.5, Page 228): Governs catenary curves, deep-water wave mechanics, and special relativity. Remember that $\cosh^2 x - \sinh^2 x = 1$.
- Partial Fractions Strategy (Section 3.12, Page 282): Reverse-engineers a unified, complex fraction into a sum of smaller, elementary isolated components.

## 📝 Quiz Questions

1. Find the coordinates of the local minimum for the curve:  
    $$f(x) = 3\cosh x + 2\sinh x$$
2. Decompose the following expression into simpler partial fractions:  
    $$\frac{5x - 3}{(x^2 - 1)(x + 2)}$$
3. Prove the power rule for the rational fractional exponent $y = x^{3/4}$ by executing the inverse function derivative rule on its baseline form $y^4 = x^3$.
4. Check the convergence of this improper integral by evaluating its infinite boundary limit explicitly:  
    $$\int_1^\infty \frac{1}{x^2 + 1} \, dx$$

---

## 🗓️ Day 3

## 🧠 Conceptual Context, Core Recipes & Text Citations

- The Inverse Function Theorem (Section 3.2a, Page 206): Allows you to find the rate of change of an inverted variable mapping without having to compute the painful inverse function explicitly.
- Improper Integrals and Singularities (Section 3.15, Page 301): Allows you to find a finite volume, area, or energy value even if the geometry stretches infinitely across a horizon or spikes vertically into an endless chasm.
- Euler Substitutions for Irrationals (Section 3.13g, Page 295): Used to clear a radical square root of a quadratic expression ($\sqrt{ax^2+2bx+c}$) by setting the entire radical expression equal to a new linear variable construct, systematically eliminating the root.

## 📝 Quiz Questions

1. Evaluate by choosing an initial $u$-substitution:  
    $$\int \frac{x}{\sqrt{1 - x^4}} \, dx$$
2. Identify the point of infinite vertical discontinuity, rewrite the boundary using proper limit notation, and evaluate:  
    $$\int_0^1 \frac{1}{\sqrt{x}} \, dx$$
3. True or False? Prove your choice as $x \to 0$:  
    $$x^2 = o(x)$$
4. Show by directly differentiating the fundamental exponential definitions that:  
    $$\frac{d}{dx}(\tanh x) = \frac{1}{\cosh^2 x}$$
5. (NEW - Sec. 3.13g) Reduce the following irrational algebraic expression to a rational function form using a clean Euler algebraic substitution (do not evaluate the final integral):  
    $$\int \frac{1}{x + \sqrt{x^2 + x + 1}} \, dx$$

---

## 🗓️ Day 4

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Completing the Square (Section 3.12b, Page 284): Shifts an irreducible quadratic workspace to line it up directly with standard geometric arcs curves ($\arctan$).
- Integration by Parts (Section 3.11, Page 274): Acts as the product rule in reverse, shifting differentiation focus away from a difficult function onto its easier partner.
- Hyperbolic Rational Substitutions (Section 3.13c, Page 294): Uses hyperbolic transformations to map profiles structurally similar to circles (hyperbolas) into straightforward, manageable algebraic balances.

## 📝 Quiz Questions

1. Integrate using algebraic substitution and completing the square:  
    $$\int \frac{2x+3}{x^2 + 4x + 13} \, dx$$
2. Evaluate using logarithmic differentiation:  
    $$y = (\ln x)^x$$
3. Use the hyperbolic half-angle substitution $t = \tanh(x/2)$ to evaluate:  
    $$\int \frac{1}{\cosh x} \, dx$$
4. Find the derivative $\frac{dy}{dx}$ of the principal branch inverse hyperbolic function:  
    $$y = \text{arsinh}(x)$$
5. (NEW - Sec. 3.13c) Completely evaluate by substituting the exponential definitions or utilizing an identity-based hyperbolic mapping:  
    $$\int \frac{\cosh x}{1 + \cosh^2 x} \, dx$$

---

## 🗓️ Day 5

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Growth Rate Hierarchies (Section 3.7b, Page 249): Defines the boundaries of functional dominance, proving why exponential components outrun algebraic and logarithmic elements across extended horizons.
- Trigonometric Integrand Domination (Section 3.13b/h, Page 296): Employs classical reduction tactics or products of trigonometric identities to map high-degree exponential waveforms back down to linear scales.

## 📝 Quiz Questions

1. Find the constants $A, B$, and $C$ to split this rational fraction:  
    $$\frac{x^2 + 1}{x(x-1)^2}$$
2. Evaluate using integration by parts twice:  
    $$\int x^2 e^{3x} \, dx$$
3. Determine whether the following improper integral converges or diverges:  
    $$\int_2^\infty \frac{1}{x \ln x} \, dx$$
4. Find all stationary critical points ($f'(x) = 0$) for the function:  
    $$f(x) = x^2 e^{-x}$$
5. (NEW - Sec. 3.13h) Evaluate using products of trigonometric relationships or an explicit trigonometric mapping:  
    $$\int \sin^4 x \cos^3 x \, dx$$

---

## 🗓️ Day 6

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Convexity and Curvature Mechanics (Section 3.6a, Page 236): Uses the second derivative to find stress distribution changes and acceleration curves.
- Liouville's Principle (Section 3.14, Page 298): Distinguishes between elementary expressions and special mathematical functions (like elliptic fields) that can only be resolved via infinite expansions.
- Advanced Root Cancellations (Section 3.13d/e, Page 294): Uses inverse parameter mappings to eliminate bounded radical gaps like $\sqrt{1-x^2}$ or $\sqrt{x^2-1}$.

## 📝 Quiz Questions

1. Determine the exact intervals of $x$ where the following function is convex (curving upward):  
    $$f(x) = x^4 - 6x^2 + 2x$$
2. Classify the following non-elementary integral by stating whether it can be solved analytically using finite elementary combinations, and identify what specific category of integrals it belongs to:  
    $$\int \frac{1}{\sqrt{(1-x^2)(1-0.5x^2)}} \, dx$$
3. Evaluate using the chain rule and implicit differentiation to find $\frac{dy}{dx}$ if:  
    $$\arctan(y/x) = \ln\sqrt{x^2+y^2}$$
4. Determine whether the following growth statement holds True or False as $x \to \infty$:  
    $$e^x = o(x^{1000})$$
5. (NEW - Sec. 3.13d) Use the standard trigonometric parameter assignment ($x = \sin \theta$ or $x = \cos \theta$) to clear the structural root boundary and evaluate:  
    $$\int \frac{1}{x^2 \sqrt{1 - x^2}} \, dx$$

---

## 🗓️ Day 7

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Pathological Derivatives (Section 3.7 Appendix A.1e, Page 259): Proves that unique physical systems can maintain baseline geometric continuity while their internal rates of change fluctuate erratically.
- Cauchy’s Generalized MVT (Section 3.3c, Page 222): Connects two separate, moving parametric tracks back to a shared time-frequency scale.
- Geometric Quadratic Reductions (Section 3.13f, Page 295): Transforms complex positive hypocycloid shapes ($\sqrt{x^2+1}$) out of algebraic deadlocks using secant/tangent substitutions.

## 📝 Quiz Questions

1. Show that the following pathological function from the appendix is continuous at $x=0$ but has a first derivative that is entirely discontinuous there:  
    $$f(x) = \begin{cases} x^2 \sin(1/x) & x \neq 0 \\ 0 & x = 0 \end{cases}$$
2. Apply Cauchy’s Generalized MVT to the functions $f(x) = x^2$ and $g(x) = x^3$ on the interval $[1, 2]$ to explicitly find the matching interior value $\xi$.
3. Evaluate this standard improper integral across its continuous vertical asymptote:  
    $$\int_{-1}^1 \frac{1}{x^2} \, dx$$
4. Using your overall integration technique toolkit, resolve the general structural antiderivative for:  
    $$\int \sqrt{a^2 - x^2} \, dx$$
5. (NEW - Sec. 3.13f) Completely evaluate using the standard geometric tangent substitution ($x = a \tan \theta$) to clear the positive square root deadlock:  
    $$\int \frac{1}{(x^2 + a^2)^{3/2}} \, dx$$

---

Would you like me to output the complete master solution key right now so you can keep it close by all week, or should we run through these day by day?