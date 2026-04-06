---
tags:
  - math
  - real_analysis
  - richard_courant
date_created: 2026-04-05
parent: "[[Introduction to Calculus and Analysis I]]"
---
The only theorem of this chapter is the chain rule which lets us compute the derivative of a composition of functions which requires both composite functions to be differentiable on the domain of interest.

A naive proof of the derivative of the function $f(x)=g(\phi(x))$ follows can follow from a "strategic multiplication of 1":$$f'(x)=\lim_{ h \to 0 } \frac{g(\phi(x+h))-g(\phi(x))}{h}=\lim_{ h \to 0 } \frac{g(\phi(x+h))-g(\phi(x))}{\phi(x+h)-\phi(x)}\frac{\phi(x+h)-\phi(x)}{h}$$
The issue with the proof here is that it is in general undefined at points where $\phi'(x)=0$, but we can prove the chain rule still holds for $g'(x)=0$ by defining a helper function $\epsilon$ and $\eta$  that follows from the mean value theorem of differential calculus: $$\epsilon=\frac{g(x+h)-g(x)}{h}-g'(x)\text{\quad and also\quad} \eta=\frac{\phi(x+h)-\phi(x)}{h}-\phi'(x)$$
We can then replace our "naive proof" by substituting with the identity:$$g(\phi(x+h))-g(\phi(x))=[g'(\phi(x))+\epsilon]h \text{\quad and also\quad} \phi(x+h)-\phi(x)=[\phi'(x)+\eta]h$$
For both $\epsilon$ and $\eta$ must go to 0 as $h$ goes to 0 and so we define them to be 0. If we do not define them at 0, then the functions $g$ and $\phi$ are no longer continuous and we have a contradiction. The trick here is that we are replacing the "naive proof" with an algebraic identity that is identical with the derivative $f'(x)$ except at the one point where it was undefined for $\phi'(x)=0$. [Functions that are identical except at one point will have the same limit at that one point](Theorem%20for%20why%20we%20can%20algebraically%20manipulate%20a%20function%20to%20determine%20its%20limit.md) so we have replaced our "naive proof" with a function that is computable at $\phi'(x)=0$ 

One conceptual application of the chain rule is the ***generalized mean value theorem of differential calculus.*** Given two functions $G(x)$ and $F(x)$ that are 
- Continuous on a closed interval $[a,b]$ 
- Differentiable on the $(a,b)$
- Assume $G'(x)>0$ so it is monotone. 
Then we have the following difference quotient: $$\frac{F(b)-F(a)}{G(b)-G(a)}=\frac{F'(\xi)(b-a)}{G(\eta)(b-a)}=\frac{F'(\xi)}{G'(\xi)}$$
The second equality is simply the mean value theorem of differentiable calculus, but the progress made with the generalized mean value theorem is to show the difference quotient can be evaluated by the derivative at the same intermediate point $x=\xi$. The proof is a simple substitution that takes advantage of the assumed monotonicity of $G(x)$:
- Because $y= G(x)$ is monotonic, there exists $G^{-1}(y)=x$ that is defined on the interval $[G(a),G(b)]=[\alpha,\beta]$
- Substitute $F(b)-F(a)$ by $F(G^{-1}(\alpha))-F(G^{-1}(\beta))$ and apply the chain rule.
# Theorems
***Chain Rule.*** The function $f(x)=g[\phi(x)]$ is differentiable if both $g(x)$ and $\phi(x)$ are differentiable on the domain of differentiation and the derivative is given by: $$f'(x)=g'(x)\phi'(x)$$
