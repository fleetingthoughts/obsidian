---
parent: "[[_Fleeting]]"
tags:
  - "#fleeting"
date_created: 2026-06-14
---
Here is the final, comprehensive version of your 7-day interleaved quiz. Each section reminder now includes a bite-sized, step-by-step example so you can visually verify the mechanics before diving into your daily quiz sets.

---

## 🗓️ Day 1

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Logarithmic Differentiation [Section 3.2e, Page 216]
    
    - Context: Used when variables are locked in both the base and exponent, or when dealing with a massive product of fractional terms.
    - Bite-sized Example: Differentiate $y = x^x$. Take logs: $\ln y = x \ln x$. Differentiate implicitly: $\frac{1}{y} y' = (1)\ln x + x(\frac{1}{x}) = \ln x + 1$. Multiply by $y$: $y' = x^x(\ln x + 1)$. [1, 2, 3]
    
- The Weierstrass Half-Angle Substitution [Section 3.13b, Page 293]
    
    - Context: Maps awkward rational combinations of $\sin x$ and $\cos x$ in a denominator into plain algebraic fractions.
    - Bite-sized Example: Convert $\int \frac{1}{\sin x} \, dx$. Let $t = \tan(x/2)$, so $\sin x = \frac{2t}{1+t^2}$ and $dx = \frac{2}{1+t^2}dt$. The integral becomes $\int \frac{1+t^2}{2t} \cdot \frac{2}{1+t^2} \, dt = \int \frac{1}{t} \, dt$.
    
- Asymptotic Notations [Section 3.7f, Page 253]
    
    - Context: Used to find which terms dominate a landscape as values explode toward infinity, letting you safely truncate calculations.
    - Bite-sized Example: Show $5x^2 + 3x = O(x^2)$ as $x \to \infty$. Divide by $x^2$: $\lim_{x\to\infty} \frac{5x^2+3x}{x^2} = \lim_{x\to\infty} (5 + \frac{3}{x}) = 5$. Since the ratio is bounded by a constant, the statement holds true.
    

## 📝 Quiz Questions

1. Find $\frac{dy}{dx}$ using logarithmic differentiation for:  
    $$y = x^{\sin x}$$
2. Convert this trigonometric integral into a plain rational algebraic function using the half-angle substitution $t = \tan(x/2)$ (do not evaluate the final algebraic integral):  
    $$\int \frac{1}{2 + \cos x} \, dx$$
3. Prove whether this statement is True or False as $x \to \infty$:  
    $$x^3 + 100x^2 \log x = O(x^3)$$
4. Evaluate using integration by parts:  
    $$\int x^2 \ln x \, dx$$
5. [Sec. 3.13b] Completely evaluate using the Weierstrass half-angle substitution:  
    $$\int \frac{1}{1 + \sin x + \cos x} \, dx$$ [4, 5, 6, 7, 8]

---

## 🗓️ Day 2

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Fermat’s Optimization Rule [Section 3.6b, Page 238]
    
    - Context: Interior local extrema occur where the tangent line flattens out entirely, meaning the instantaneous rate of change drops precisely to zero.
    - Bite-sized Example: Find the critical point of $f(x) = x^2 - 4x$. Set $f'(x) = 2x - 4 = 0$, which yields $x = 2$.
    
- Hyperbolic Functions Foundations [Section 3.5, Page 228]
    
    - Context: Governs catenary curves and deep-water wave mechanics.
    - Bite-sized Example: Prove $\frac{d}{dx}(\cosh x) = \sinh x$. Since $\cosh x = \frac{e^x+e^{-x}}{2}$, differentiating gives $\frac{e^x-e^{-x}}{2}$, which is exactly $\sinh x$. [9]
    
- Partial Fractions Strategy [Section 3.12, Page 282]
    
    - Context: Reverse-engineers a unified, complex fraction into a sum of smaller, elementary isolated components.
    - Bite-sized Example: Split $\frac{1}{x(x+1)}$. Set up $\frac{A}{x} + \frac{B}{x+1} = \frac{A(x+1)+Bx}{x(x+1)}$. Matching the numerators ($1 = (A+B)x + A$) gives $A=1$ and $A+B=0 \implies B=-1$. Thus, $\frac{1}{x} - \frac{1}{x+1}$.
    

## 📝 Quiz Questions

1. Find the coordinates of the local minimum for the curve:  
    $$f(x) = 3\cosh x + 2\sinh x$$
2. Decompose the following expression into simpler partial fractions:  
    $$\frac{5x - 3}{(x^2 - 1)(x + 2)}$$
3. Prove the power rule for the rational fractional exponent $y = x^{3/4}$ by executing the inverse function derivative rule on its baseline form $y^4 = x^3$.
4. Check the convergence of this improper integral by evaluating its infinite boundary limit explicitly:  
    $$\int_1^\infty \frac{1}{x^2 + 1} \, dx$$ [10]

---

## 🗓️ Day 3

## 🧠 Conceptual Context, Core Recipes & Text Citations

- The Inverse Function Theorem [Section 3.2a, Page 206]
    
    - Context: Allows you to find the rate of change of an inverted variable mapping without having to compute the painful inverse function explicitly.
    - Bite-sized Example: If $y = x^3 + x$, find $\frac{dx}{dy}$ at $x=1$. First, $\frac{dy}{dx} = 3x^2 + 1$. At $x=1$, $\frac{dy}{dx} = 4$. Therefore, $\frac{dx}{dy} = \frac{1}{4}$. [11]
    
- Improper Integrals and Singularities [Section 3.15, Page 301]
    
    - Context: Allows you to find a finite volume or area even if the geometry stretches infinitely across a horizon or spikes vertically into a chasm.
    - Bite-sized Example: Evaluate $\int_1^\infty \frac{1}{x^2}\,dx$. Rewrite as $\lim_{B\to\infty} \int_1^B x^{-2}\,dx = \lim_{B\to\infty} \left[ -\frac{1}{x} \right]_1^B = \lim_{B\to\infty} (-\frac{1}{B} + 1) = 1$.
    
- Euler Substitutions for Irrationals [Section 3.13g, Page 295]
    
    - Context: Used to clear a radical square root of a quadratic expression ($\sqrt{ax^2+2bx+c}$) by setting the entire radical expression equal to a new linear variable construct.
    - Bite-sized Example: For $\sqrt{x^2+1}$, set $\sqrt{x^2+1} = t - x$. Square both sides: $x^2 + 1 = t^2 - 2tx + x^2 \implies 1 = t^2 - 2tx$, which allows you to express $x = \frac{t^2-1}{2t}$ completely rationally without any roots.
    

## 📝 Quiz Questions

1. Evaluate by choosing an initial $u$-substitution:  
    $$\int \frac{x}{\sqrt{1 - x^4}} \, dx$$
2. Identify the point of infinite vertical discontinuity, rewrite the boundary using proper limit notation, and evaluate:  
    $$\int_0^1 \frac{1}{\sqrt{x}} \, dx$$
3. True or False? Prove your choice as $x \to 0$:  
    $$x^2 = o(x)$$
4. Show by directly differentiating the fundamental exponential definitions that:  
    $$\frac{d}{dx}(\tanh x) = \frac{1}{\cosh^2 x}$$
5. [Sec. 3.13g] Reduce the following irrational algebraic expression to a rational function form using a clean Euler algebraic substitution (do not evaluate the final integral):  
    $$\int \frac{1}{x + \sqrt{x^2 + x + 1}} \, dx$$

---

## 🗓️ Day 4

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Completing the Square [Section 3.12b, Page 284]
    
    - Context: Shifts an irreducible quadratic workspace to line it up directly with standard geometric arc curves ($\arctan$).
    - Bite-sized Example: Integrate $\int \frac{1}{x^2 + 2x + 5}\,dx$. Complete the square: $x^2 + 2x + 5 = (x+1)^2 + 4$. The integral becomes $\int \frac{1}{(x+1)^2 + 2^2}\,dx = \frac{1}{2}\arctan\left(\frac{x+1}{2}\right) + C$.
    
- Integration by Parts [Section 3.11, Page 274]
    
    - Context: Acts as the product rule in reverse, shifting differentiation focus away from a difficult function onto its easier partner.
    - Bite-sized Example: Evaluate $\int x e^x \, dx$. Let $u = x \implies du = dx$, and $dv = e^x dx \implies v = e^x$. The result is $uv - \int v\,du = xe^x - \int e^x\,dx = xe^x - e^x + C$. [12]
    
- Hyperbolic Rational Substitutions [Section 3.13c, Page 294]
    
    - Context: Uses hyperbolic transformations to map profiles structurally similar to hyperbolas into straightforward, manageable algebraic balances.
    - Bite-sized Example: Solve $\int \sqrt{1 + \sinh^2 x} \cdot \cosh x \, dx$. Because $1 + \sinh^2 x = \cosh^2 x$, the radical collapses into $\int \cosh^2 x \, dx$, which splits into standard elementary exponentials easily.
    

## 📝 Quiz Questions

1. Integrate using algebraic substitution and completing the square:  
    $$\int \frac{2x+3}{x^2 + 4x + 13} \, dx$$
2. Evaluate using logarithmic differentiation:  
    $$y = (\ln x)^x$$
3. Use the hyperbolic half-angle substitution $t = \tanh(x/2)$ to evaluate:  
    $$\int \frac{1}{\cosh x} \, dx$$
4. Find the derivative $\frac{dy}{dx}$ of the principal branch inverse hyperbolic function:  
    $$y = \text{arsinh}(x)$$
5. [Sec. 3.13c] Completely evaluate by substituting the exponential definitions or utilizing an identity-based hyperbolic mapping:  
    $$\int \frac{\cosh x}{1 + \cosh^2 x} \, dx$$ [13]

---

## 🗓️ Day 5

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Growth Rate Hierarchies [Section 3.7b, Page 249]
    
    - Context: Defines the boundaries of functional dominance, proving why exponential components outrun algebraic and logarithmic elements across extended horizons.
    - Bite-sized Example: Evaluate $\lim_{x\to\infty} \frac{e^x}{x^{100}}$. By applying L'Hôpital's rule repeatedly (or utilizing the growth hierarchy theorem directly), the exponential numerator completely dominates the polynomial denominator, driving the limit to $\infty$.
    
- Trigonometric Integrand Domination [Section 3.13b/h, Page 296]
    
    - Context: Employs classical reduction tactics or products of trigonometric identities to map high-degree exponential waveforms back down to linear scales.
    - Bite-sized Example: Evaluate $\int \sin^3 x \, dx$. Separate one sine term: $\int (1 - \cos^2 x)\sin x \, dx$. Let $u = \cos x \implies du = -\sin x \, dx$, transforming it into $-\int (1-u^2)\,du$.
    

## 📝 Quiz Questions

1. Find the constants $A, B$, and $C$ to split this rational fraction:  
    $$\frac{x^2 + 1}{x(x-1)^2}$$
2. Evaluate using integration by parts twice:  
    $$\int x^2 e^{3x} \, dx$$
3. Determine whether the following improper integral converges or diverges:  
    $$\int_2^\infty \frac{1}{x \ln x} \, dx$$
4. Find all stationary critical points ($f'(x) = 0$) for the function:  
    $$f(x) = x^2 e^{-x}$$
5. [Sec. 3.13h] Evaluate using products of trigonometric relationships or an explicit trigonometric mapping:  
    $$\int \sin^4 x \cos^3 x \, dx$$

---

## 🗓️ Day 6

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Convexity and Curvature Mechanics [Section 3.6a, Page 236]
    
    - Context: Uses the second derivative to find stress distribution changes and acceleration curves.
    - Bite-sized Example: Determine if $f(x) = x^3$ is convex or concave at $x = 1$. Find $f'(x) = 3x^2$ and $f''(x) = 6x$. At $x = 1$, $f''(1) = 6 > 0$, so the curve is convex (upward bending) at that point. [14]
    
- Liouville's Principle [Section 3.14, Page 298]
    
    - Context: Distinguishes between elementary expressions and special functions (like elliptic fields) that can only be resolved via infinite expansions.
    - Bite-sized Example: Identifying why $\int \frac{e^x}{x} \, dx$ or $\int \sin(x^2) \, dx$ cannot be simplified to normal, closed-form algebraic expressions. You must state they are non-elementary.
    
- Advanced Root Cancellations [Section 3.13d/e, Page 294]
    
    - Context: Uses inverse parameter trigonometric mappings to eliminate bounded radical gaps like $\sqrt{1-x^2}$ or $\sqrt{x^2-1}$.
    - Bite-sized Example: Simplify $\int \sqrt{1-x^2}\,dx$. Substitute $x = \sin\theta \implies dx = \cos\theta\,d\theta$. The radical becomes $\sqrt{1-\sin^2\theta} = \cos\theta$, reducing the problem cleanly to $\int \cos^2\theta\,d\theta$.
    

## 📝 Quiz Questions

1. Determine the exact intervals of $x$ where the following function is convex (curving upward):  
    $$f(x) = x^4 - 6x^2 + 2x$$
2. Classify the following non-elementary integral by stating whether it can be solved analytically using finite elementary combinations, and identify what specific category of integrals it belongs to:  
    $$\int \frac{1}{\sqrt{(1-x^2)(1-0.5x^2)}} \, dx$$
3. Evaluate using the chain rule and implicit differentiation to find $\frac{dy}{dx}$ if:  
    $$\arctan(y/x) = \ln\sqrt{x^2+y^2}$$
4. Determine whether the following growth statement holds True or False as $x \to \infty$:  
    $$e^x = o(x^{1000})$$
5. [Sec. 3.13d] Use the standard trigonometric parameter assignment ($x = \sin \theta$ or $x = \cos \theta$) to clear the structural root boundary and evaluate:  
    $$\int \frac{1}{x^2 \sqrt{1 - x^2}} \, dx$$ [15, 16, 17]

---

## 🗓️ Day 7

## 🧠 Conceptual Context, Core Recipes & Text Citations

- Pathological Derivatives [Section 3.7 Appendix A.1e, Page 259]
    
    - Context: Proves that unique mathematical curves can stay structurally continuous on a graph while their slope properties ripple into absolute chaos at a single point.
    - Bite-sized Example: For $f(x) = x \sin(1/x)$, as $x \to 0$, the function bounds squeeze to $0$ via the Sandwich Theorem (continuous). However, computing the derivative slope at $0$ yields $\lim_{h\to0} \frac{h\sin(1/h) - 0}{h} = \lim_{h\to0} \sin(1/h)$, which oscillates endlessly and fails to exist.
    
- Cauchy’s Generalized MVT [Section 3.3c, Page 222]
    
    - Context: Connects two separate, moving parametric tracks back to a shared scale, serving as the logical bedrock for L'Hôpital's proof.
    - Bite-sized Example: For $f(x)=x^2$ and $g(x)=x$ on $[0,1]$, Cauchy's theorem asserts there is a point $\xi$ where $\frac{f(1)-f(0)}{g(1)-g(0)} = \frac{f'(\xi)}{g'(\xi)} \implies \frac{1-0}{1-0} = \frac{2\xi}{1} \implies \xi = \frac{1}{2}$.
    
- Geometric Quadratic Reductions [Section 3.13f, Page 295]
    
    - Context: Transforms complex positive hypocycloid shapes ($\sqrt{x^2+1}$) out of algebraic deadlocks using secant/tangent substitutions.
    - Bite-sized Example: For $\int \frac{1}{\sqrt{x^2+1}}\,dx$, substitute $x = \tan\theta \implies dx = \sec^2\theta\,d\theta$. The radical simplifies to $\sqrt{\tan^2\theta+1} = \sec\theta$, reducing the integrand to $\int \frac{\sec^2\theta}{\sec\theta}\,d\theta = \int \sec\theta\,d\theta$. [18]
    

## 📝 Quiz Questions

1. Show that the following pathological function from the appendix is continuous at $x=0$ but has a first derivative that is entirely discontinuous there:  
    $$f(x) = \begin{cases} x^2 \sin(1/x) & x \neq 0 \\ 0 & x = 0 \end{cases}$$
2. Apply Cauchy’s Generalized MVT to the functions $f(x) = x^2$ and $g(x) = x^3$ on the interval $[1, 2]$ to explicitly find the matching interior value $\xi$.
3. Evaluate this standard improper integral across its continuous vertical asymptote:  
    $$\int_{-1}^1 \frac{1}{x^2} \, dx$$
4. Using your overall integration technique toolkit, resolve the general structural antiderivative for:  
    $$\int \sqrt{a^2 - x^2} \, dx$$
5. [Sec. 3.13f] Completely evaluate using the standard geometric tangent substitution ($x = a \tan \theta$) to clear the positive square root deadlock:  
    $$\int \frac{1}{(x^2 + a^2)^{3/2}} \, dx$$
