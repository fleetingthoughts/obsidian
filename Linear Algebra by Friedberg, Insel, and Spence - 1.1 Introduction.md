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

These descriptions let us set up the following axioms to describe vectors $x$, $y$, $z$ with any scalars $a, b$ :
1) $x+y=y+x$  (commutativity of vector addition)
2) $(x+y)+z=x+(y+z)$ (associativity of vector addition)
3) There exists a vector 0 such that $x+0 = x$ 
4) For any vector, $x$, there exists a vector $y$ such that $x+y=0$
5) There exists the scalar 1 such that $1x=x$
6) $(ab)x=a(bx)$  (associativity of scalar multiplication)
7) $a(x+y) = ax+ay$  (left distributive property of scalar multiplication)
8) $(a+b)x = ax+bx$   (right distributive property of scalar multiplication)

Note that nowhere in this do we define multiplication between vectors

We now show to describe lines and planes in terms of vectors. To fully describe a line or point is to find an analytical way to determine whether any other candidate point is on the line or plane or to generate any new points on the line or plane. The line is defined by two points and the plane is defined by 3 so we will make use of the vectors $u, v,$ and if it is a plane, $w$ that have these given points as endpoints.

The book provides a geometric appeal to show that for a line defined by two points described by vectors $u, v$, the line is described by a vector that goes to $A$ then another vector that ends on $B$ (i.e. a vector that is parallel to $v-u$). Any point $x$ on the line is therefore:$$x = u+t(v-u) \text{\quad where t is a scalar}$$
The plane is done analogously: $$
$$