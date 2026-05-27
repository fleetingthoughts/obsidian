---
tags:
  - math
  - real_analysis
  - richard_courant
date_created: 2026-04-05
parent: "[[Introduction to Calculus and Analysis I]]"
---
We derive the chain rule technique to solve the derivative of a composition of functions. The theorem is used to complete our understanding of power functions when it comes to powers of irrational numbers and facilitate their computation. We also use the chain rule to deduce Cauchy's Mean value theorem also known as the Generalized mean value theorem:
1) Naive derivation of the chain rule that presumes the derivative of the inner composite function cannot be 0
2) Another definition using the definitions of derivatives that shows the same formula as 1) follows even if the inner composite function is 0.
	1) Uses Weierstrass' definition of a derivative to construct helper functions
	2) Reformulate the standard quotient for a derivative using Weierstrass' definition
	3) Evaluate the limit
3) The chain rule solves the computation problem with our analytic continuation of the power function by defining it in terms of the exponential function, which turned it into a compositional funciton.

# The two proofs of the chain rule. A Naive proof and a refined proof that shows the same formula applies to more situations
A naive proof of the derivative of the function $f(x)=g(\phi(x))$ can follow from a "strategic multiplication of 1":$$f'(x)=\lim_{ h \to 0 } \frac{g(\phi(x+h))-g(\phi(x))}{h}=\lim_{ h \to 0 } \frac{g(\phi(x+h))-g(\phi(x))}{\phi(x+h)-\phi(x)}\frac{\phi(x+h)-\phi(x)}{h}$$
The issue with the proof here is that it is in general undefined at points where $\phi'(x)=0$, but we can prove the chain rule still holds for $g'(x)=0$ by defining a helper function $\epsilon$ and $\eta$  that follows from the direct definition of the limit which happens to be Weierstrass' definition of a derivative: $$\epsilon=\frac{g(x+h)-g(x)}{h}-g'(x)\text{\quad and also\quad} \eta=\frac{\phi(x+h)-\phi(x)}{h}-\phi'(x)$$
We can then replace our "naive proof" by substituting with the identity:$$g(\phi(x+h))-g(\phi(x))=[g'(\phi(x))+\epsilon]h \text{\quad and also\quad} \phi(x+h)-\phi(x)=[\phi'(x)+\eta]h$$
For both $\epsilon$ and $\eta$ must go to 0 as $h$ goes to 0 and so we define them to be 0. If we do not define them at 0, then the functions $g$ and $\phi$ are no longer continuous and we have a contradiction. The trick here is that we are replacing the "naive proof" with an algebraic identity that is identical with the derivative $f'(x)$ except at the one point where it was undefined for $\phi'(x)=0$. [Functions that are identical except at one point will have the same limit at that one point](Theorem%20for%20why%20we%20can%20algebraically%20manipulate%20a%20function%20to%20determine%20its%20limit.md) so we have replaced our "naive proof" with a function that is computable at $\phi'(x)=0$ 

# Complete our analytical definition of the power function and use chain rule to easily compute the derivative of power functions.
One of the powers of calculus is it allows us to reformulate our naive conception of functions to a more general function that extends the domain of the function called analytic continuation. We use calculus to complete the analytic continuation of the power function to irrational exponents

A naive conception of the power function $x^{\alpha}$ was to view it as a number $x$ multiplied $\alpha$ times and $x^{1/\alpha}$ is the inverse operation. This formulation holds well for rational exponents but lacks meaning for irrational numbers. We can define power functions to irrational exponents by an infinite sequence of irrational numbers but this is cumbersome for computation and proofs as you have to show the limit exists and is unique for all possible sequences. 

In [chapter 2.7](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%202.7%20The%20Integral%20of%20an%20Arbitrary%20Power%20of%20x.md), we defined the power function in terms of the exponential which is the inverse of the logarithm defined as an integral. This definition satisfies all the usual properties we want in a power function and it also instantly proves the uniqueness and existence as it is defined in terms of an integral that is continuous and monotonic.

The problem with the analytic continuation of the power function with this new definition is that it is now a composite function and we had no means of computing the derivative, but we can with the chain rule. Application of the chain rule to powers with rational exponents also shows our definition is consistent with the results we derived in [chapter 2.2](Introduction%20to%20Calculus%20I%20by%20Fritz%20and%20Courant%20-%202.2%20Elementary%20Examples%20of%20Integration.md) to ensure we didn't create a monster.

# Cauchy's Mean Value Theorem
One conceptual application of the chain rule is the ***generalized mean value theorem of differential calculus.*** Given two functions $G(x)$ and $F(x)$ that are 
- Continuous on a closed interval $[a,b]$ 
- Differentiable on the $(a,b)$
- Assume $G'(x)>0$ so it is monotone. 
Then we have the following difference quotient: $$\frac{F(b)-F(a)}{G(b)-G(a)}=\frac{F'(\xi)(b-a)}{G(\eta)(b-a)}=\frac{F'(\xi)}{G'(\xi)}$$
The second equality is simply the mean value theorem of differentiable calculus, but the progress made with the generalized mean value theorem is to show the difference quotient can be evaluated by the derivative at the same intermediate point $x=\xi$. The proof is a simple substitution that takes advantage of the assumed monotonicity of $G(x)$:
- Because $y= G(x)$ is monotonic, there exists $G^{-1}(y)=x$ that is defined on the interval $[G(a),G(b)]=[\alpha,\beta]$
- Substitute $F(b)-F(a)$ by $F(G^{-1}(\alpha))-F(G^{-1}(\beta))$ and apply the chain rule.

# Summary of computational results
- ***Formulation of the derivative using Weierstrass' definition.*** It is useful to consider alternatives to the standard definition of a derivative as a difference quotient. If we consider the standard to be our definition, then Weierstrass' definition of a derivative is a "theorem" that provides an equivalent formulation of the derivative that is useful. <u>The Weierstrass definition of the derivative is useful to see the derivative in terms of an error</u>

# Theorems
***Chain Rule.*** The function $f(x)=g[\phi(x)]$ is differentiable if both $g(x)$ and $\phi(x)$ are differentiable on the domain of differentiation and the derivative is given by: $$f'(x)=g'(x)\phi'(x)$$
