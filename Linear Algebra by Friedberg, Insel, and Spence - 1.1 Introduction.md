---
tags:
  - "#math"
  - arnold_friedberg
  - linear_algebra
date_created: 2026-02-16
parent: "[[Linear Algebra - Friedberg, Insel, and Spence]]"
---
The chapter begins with an experimental motivation to look at mathematical objects that describe physical quantities (e.g. force and velocity) that care about two quantities: magnitude and direction. These mathematical objects are vectors. Note that starting position is not considered.

These experimental motivation go on further to describe geometrically vectors can be added following a parallelogram law: 
![](Pasted%20image%2020260216195903.png)
This geometric view looks at vector addition as a tail-to-head construction where one vector originates from the endpoint of another vector that starts from the origin.

Another view is to describe this geometry "analytically" by the endpoint of each vector originating from the origin. We can fully describe a vector's magnitude and direction by this endpoint, say $(x_1,y_2)$ and so given two vectors described this way by their endpoints $(x_1,x_2)$ and $(y_1,y_2)$, then the sum of the vectors is simply $$(x_{1}+y_{1},x_{2}+y_{2})$$
We are further experimentally motivated to describe parallel vectors by the fact if they only differ in magnitude but go in the same direction so that their ratio is simply a scalar.

These descriptions let us set up the following axioms to describe vectors $x$, $y$, $z$:
1) $x+y=y+x$  (commutativity)
2) $(x+y)+z = x +(y+z)$ (associativity)
3) There exists a vector $0$ such that $x+0 = x$ for any $x$
4) For each vector $x$ there exists a vector $y$ such that $x+y=0$
5) $1x=x$
6) $(ab)x=a(bx)$
7) $a(x+y) =ax+ay$ for $a\in \mathbb{R}$ (right distributive)
8) $(a+b)x = ax+bx$

The author then provides the algorithms to describe lines and planes. A line is defined by 2 points and a plane is defined by 3. To be able to describe a line or plane is to be able to mathematically express any point on that line or plane.

Given two points $(u_{1},u_{2},u_{3})$ and $(v_{1},v_{2},v_{3})$, we can describe the line that contains these two points by the vectors with those end points. Any point on the line will be a vector that goes to either of those points and then go towards the other point. The line is then determined by vector addition. The equation that describes any point $x=(x_{1},x_{2},x_{3})$ is therefore:
$$x=u+t(v-u)\text{\quad for \quad}t\in \mathbb{R}$$
![](Pasted%20image%2020260217005640.png)

Now for a plane, we're described by 3 points, so along with points described by vectors $u$ and $v$ we have a vector $a$ that describes a third point. The equation that describes any point $x=(x_{1},x_{2},x_{3})$ on the plane is:
$$x = a+s(u-a)+t(v-a) \text{\quad for \quad} s,t \in \mathbb{R}$$

![](Pasted%20image%2020260217010326.png)
