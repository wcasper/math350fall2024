---
layout: page
title: Practice Exam 1 Solutions
permalink: /exams/practice-exam1-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.
Assume both $$(s_n)$$ and $$(t_n)$$ are sequences of real numbers.

a) The set $$\{\mathbb{Z},\mathbb{R}\}$$ is uncountable.

b) The Well-Ordering Principle says that every set of integers has a minimum element.

c) Any set of real numbers which is bounded above has a maximum

d) The set $$\{(1,2),(2,1),(3,3)\}$$ is a relation from $$\mathbb{Z}$$ to $$\mathbb{R}$$

e) The number $$x = 0.123123123123\dots$$ is rational

**Solution:**

a) False!  It has only two elements!

b) False!  It needs to be *positive* integers!

c) False!  We have a supremum, but potentially no maximum...

d) True!  Any subset of $\mathbb{Z}\times\mathbb{R}$ is a relation

e) True!  As long as the decimal expansion is eventually repeating, it is rational.  Can you figure out what the fraction form is?

## Problem 2

a) Write down the five field axioms, the four order axioms, and the completeness axiom

b) State the definition of a supremum

c) Carefully state the Cauchy-Schwarz inequality.

**Solution:**

a) Make sure to know the other axioms, too!
 * commutativity:  $$x+y = y+x$$ and $$xy=yx$$
 * associativity:  $$(x+y) + z = x + (y+z)$$ and $$(xy)z = x(yz)$$
 * distributivity: $$$x(y + z) = xy + xz$$
 * addive inverses: given $$x,y\in F$$, there exists a unique $$z\in F$$ with $$x=y+z$$
 * multiplicative inverse: given $$x,y\in F$$ with $$y\neq 0$$, there exists a unique $$z\in F$$ with $$x = yz$$

b) What about infimum?  Minimum, maximum?  Know your stuff!

A supremum of a set $$A$$ is an element $$x$$ which is an upper bound of $$A$$, but with the property that if $$y < x$$ then $$y$$ is not an upper bound of $$A$$

c) Do we also know Minkowski's Inequality?  The Triangle Ineqeuality?

The Cauchy-Schwarz inequlity says that if $$x_1,\dots, x_n$$ and $$y_1,\dots, y_n$$ are real numbers then

$$\sum_{k=1}^n x_ky_k \leq \left(\sum_{k=1}^n x_k^2\right)^{1/2}\left(\sum_{k=1}^n y_k^2\right)^{1/2}.$$

## Problem 3

a) Give the definition of an upper bound

b) Is the set

$$\left\lbrace\frac{1}{x^2-3}: x\in\mathbb Q\right\rbrace$$

bounded above?  Carefully justify your answer.

**Solution:**

a) An element $$x$$ is an upper bound of a set $$A$$ if $$a\leq x$$ for all $$a\in A$$.

b) No.  To see this, suppose that it is bounded above by some number $$N$$.
Let $$N > 0$$ be an integer.  Then we may choose a rational number $$x$$ with 

$$\sqrt{3} < x < \sqrt{3 + 1/N}.$$ 

Then $$0 < x^2 - 3 < 1/N$$, so that $$N < \frac{1}{x^2-3}$$.
This is a contradiction.

## Problem 4

a) Write the definition of a relation $$\mathcal R$$ from a set $$A$$ to a set $$B$$

b) Write what it means for a relation $$\mathcal R$$ on a set $$A$$ to be reflexive.  What about symmetric?  Transitive?  An equivalence relation?

c) Give an example of a relation which is reflexive, but not symmetric or transitive.

**Solution:**

a) This is a subset of the Cartesian product $$A\times B$$.

b) 

 * Reflexive means $$x\mathcal R x$$ for all $$x\in A$$
 * Symmetric means $$x\mathcal R y$$ implies $$y\mathcal R x$$ for all $$x,y\in A$$
 * Transitive means $$x\mathcal R y$$ and $$y\mathcal R z$$ implies $$x\mathcal R z$$ for all $$x,y,z\in A$$
 * An equivalence relation is a relation which is reflexive, symmetric, and transitive.

c) One example is the relation $$\mathcal R$$ on $$\mathbb{R}$$ defined by

$$\mathcal R = \{(x,y): x=y\ \text{or}\ x=y^2\}.$$

Can you prove that it is reflexive but not symmetric or transitive?


## Problem 5

Consider the relation from $$\mathbb{Z}$$ to $$\mathbb{Z}_+$$ defined by

$$\mathcal R = \{(x+y,xy^2): x\in\mathbb{Z}_+,\ \ y\in\mathbb{Z}\},$$

a) Write what it means for a relation $$\mathcal R$$ from a set $$A$$ to a set $$B$$ to be a function

b) Is $$f(x)$$ a function?  Carefully explain.

**Solution:**

a) For every $$x$$ in the domain of $$\mathcal R$$ there exists a unique $$y$$ with $$x\mathcal R y$$

b) No, since if we take $$x=2$$ and $$y=-2$$ we get the point $$(0,8)$$, but if we take $$x=1$$ and $$y=-1$$ we get the poinit $$(0,1)$$.
Therefore $$0\mathcal R8$$ and $$0\mathcal R1$$.

## Problem 6

For any subset $$A\subseteq\mathbb{R}$$, define $$-A = \{-x: x\in A\}.$$

a) Suppose that $$A$$ is bounded above.  Define the supremum of $$A$$.

b) Suppose that $$A$$ is bounded both above and below.  Prove that $$\sup(-A) = -\inf(A)$$ and $$\inf(-A)=-\sup(A)$$.

**Solution:**

a) It is an upper bound of $$A$$ with the property that any smaller number is not an upper bound.

b) Let $$M=\sup(A)$$.  Then $$M$$ is an upper bound of $$A$$.  Therefore

$$x \leq M\quad \text{for all}\ x\in A.$$

It follows that

$$-M\leq -x \quad \text{for all}\ x\in A,$$

and therefore

$$-M\leq y \quad \text{for all}\ y\in -A.$$

Therefore $$-M$$ is a lower bound of $$-A$$.

If $$a > -M$$, then $$-a < M$$ and therefore $$-a$$ is not an upper bound of $$A$$.
It follows that there exists $$x\in A$$ with $$x > -a$$.
Therefore $$y=-x\in -A$$ satisfies $$y < a$$.
Thus $$a$$ is not a lower bound.
This shows that $$-M$$ is the greatest lower bound, ie. the infimum of $$A$$.
The other half of the problem is proved similarly.


## Problem 7

Consider the set

$$\left\lbrace\frac{2n^2+3}{n^2+2n}: n\in\mathbb{Z}_+\right\rbrace$$

a) Explain why the set has a supremum

b) Find the supremum of the set

c) Carefully prove that the supremum you found is the supremum of the set

**Solution:**

a) First of all

$$\frac{2n^2+3}{n^2+2n} = \frac{2+3/n^2}{1+2/n} \leq \frac{2+3/n^2}{1+2/n} \leq \frac{2+3/n^2}{1} \leq 5.$$

Thereefore the set is bounded above by $$5$$.
By the Completeness Axiom it must have a supremum.

b) The first element of the set is $$5/3$$.  The second is $$11/8$$.  The third is $$21/15$$. Then as $$n$$ gets larger, the elements of the set increase toward $$2$$.  This makes us suspect that the answer might be $$2$$.  Let's prove it.

First of all

$$\frac{2n^2+3}{n^2+2n} = 2 - \frac{4n-3}{n^2+2n} < 2$$

for all $$n\in\mathbb{Z}_+$$.  Therefore $$2$$ is an upper bound for the set.

Moreover, 

$$\frac{4n-3}{n^2+2n} < \frac{4(n-1)}{n(n+2)} < \frac{4}{(n-1)(n+2)} = \frac{4}{n+2}.$$

This means that

$$ \frac{2n^2+3}{n^2+2n} \geq 2 - \frac{4}{n+2}.$$

Now suppose that $$a < 2$$.  Then for $$n$$ an integer greater than $$4/(2-a) - 2$$ we have

$$n+2 > 4/(2-a)$$

and therefore

$$2-a > 4/(n+2)$$

and thus

$$ \frac{2n^2+3}{n^2+2n} \geq 2 - \frac{4}{n+2} > 2 - (2-a) = a.$$

Thus $$a$$ is not an upper bund and this proves $$2$$ is the greatest upper bound.

## Problem 8

Consider the family of sets $$\{A_i: i\in I\}$$
with index set $$I=\mathbb{Z}_+$$ and with $$A_i = (-1/i,1/i)$$.

(a) Determine the value of $$\bigcup_{i\in I} A_i$$

(b) Carefully prove your answer in part (a)

(c) Determine the value of $$\bigcap_{i\in I} A_i$$

(d) Carefully prove your answer in part (d)


**Solution:**

a) The answer is $$(-1,1)$$.

b) Clearly $$(-1,1) = A_1\subseteq\bigcup_{i\in I} A_i$$, so we need only show the other containment.
Suppose that $$x\in \bigcup_{i\in I}A_i$$.  Then $$x\in A_n$$ for some $$n$$.  Therefore $$x\in (-1/n, 1/n)$$, and consequently $$x\in (-1,1)$$.  Since $$x$$ was arbitrary, this proves our equality.

c) The answer is $$\{0\}$$

d) Clearly $$0\in A_i$$ for all $$i$$, so $$\{0\}\subseteq\bigcap_{i\in I} A_i$$.

For the coverse, suppose that $$x\in\mathbb{R}\neq 0$$.  Then by the Archimedian principle, there exists an integer $$n$$ with $$n > \lvert x r\vert.$$ It follows that $$x\notin (-1/n, 1/n)$$.  Therefore $$x\notin A_n$$ and thus $$x\notin \bigcap_{i\in I} A_i$$.



