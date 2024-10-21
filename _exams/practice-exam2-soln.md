---
layout: page
title: Practice Exam 2
permalink: /exams/practice-exam2
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.
Assume both $$(s_n)$$ and $$(t_n)$$ are sequences of real numbers.

a) In a metric space $$M$$ with the discrete metric, every subset is both open and closed

b) The union of any family of closed sets is closed

c) Every open subset of $$\mathbb{R}$$ with the Euclidean metric is a countable union of disjoint open intervals

d) A convergent sequence must be bounded

e) Every accumulation point is also an adherent point

**Solution:**

True, False, True, True, True

## Problem 2

a) Write down the definition of $$\{x_n\}$$ being a Cauchy sequence and the definition of $$\{x_n\}$$ converging to $$L$$.

b) State the definition of an open cover of a set

c) Carefully state the Heine-Borel Theorem and Lindelof's Theorem.

**Solution:**

a) A sequence is Cauchy if for all $$\epsilon > 0$$ there exists $$N$$ such that $$m,n\geq N$$ implies $$d(x_m,x_n) < \epsilon$$.
A sequence converges to $$L$$ if for all $$\epsilon > 0$$ there exists $$N$$ such that $$n\geq N$$ implies $$d(x_m,L) < \epsilon$$.


b) An open cover of a set $$A$$ is a family of sets $$\{U_i: i\in I\}$$ which are all open and with the property that $$A\subseteq \bigcup_{i\in I} U_i$$

c)
The Heine-Borel Theorem says that a subset of $$\mathbb{R}^n$$ (with the Euclidean metric) is compact if and only if it is closed and bounded.
Lindelof's Theorem says that for any subset $$A$$ of $$\mathbb{R}^n$$ (with the Euclidean metric), every open cover of $$A$$ has a countable subcover.

## Problem 3

a) Write down the definition of a metric space.

b) Carefully prove that in a metric space $$(M,d)$$, the open ball 

$$B_M(x,r) = \{y\in M: d(x,y) < r\}$$

is an open set.

**Solution:**

a) A metric space is a pair $$(M,d)$$ consisting of a set $$M$$ and a function $$d: M\times M\rightarrow \mathbb{R}$$ with the following four properties
* $$d(x,y) = 0$$ if and only if $$x=y$$ for all $$x,y\in M$$
* (positivity) $$d(x,y)\geq 0$$ for all $$x,y\in M$$
* (symmetry) $$d(x,y) = d(y,x)$$ for all $$x,y\in M$$
* (triangle inequality) $$d(x,y)\leq d(x,z) + d(z,y)$$ for all $$x,y,z\in M$$

b) Suppose that $$y\in B_M(x,r)$$.  Then $$d(x,y) < r$$, so $$s := r-d(x,y) > 0$$.
If $$z\in B_M(y,s)$$, then the triangle inequality says

$$d(x,z)\leq d(x,y) + d(y,z) < d(x,y) + s = r.$$

Therefore $$d(x,z) < r$$, implying that $$z\in B_M(x,r)$$.  Since $$z\in B_M(y,s)$$ was arbitrary, this proves $$B_M(y,s)\subseteq B_M(x,r)$$.
This means that $$y$$ is an interior point of $$B_M(x,r)$$. 
Since $$y\in B_M(x,r)$$ was arbitrary, this shows every element of $$B_M(x,r)$$ is an interior point.
Hence $$B_M(x,r)$$ is an open set.

## Problem 4

In this problem, let $$M=\mathbb{R}$$ with the Euclidean metric

a) Write down the definition of an adherent point and an accumulation point of a set $$S\subseteq M$$

b) Prove that $$0$$ is an accumulation point of the set

$$S = \{x\in M: 0 < x < 1,\ \ \text{$x$ is irrational}\}.$$

**Solution:**

a)
A point $$a\in M$$ is an adherent point of $$S$$ if for all $$r>0$$ the ball $$B_M(a,r)$$ contains at least one element of $$S$$.
A point $$a\in M$$ is an accumulation point of $$S$$ if for all $$r>0$$ the ball $$B_M(a,r)$$ contains at least one element of $$S$$ which is different from $$a$$.

b)
Let $$r>0$$.
We proved in the homework, that there exists an irrational point between $$0$$ and $$\min(r,1)$$.
Therefore $$B_M(0,r) = (-r,r)$$ contains an element of $$S$$.
Since $0\notin S$$, this point is also different from $$0$$.
Hence $$0$$ is an accumulation point of $$S$$.

## Problem 5

a) Define the closure $$\overline{S}$$ of a subset $$S$$ of a metric space $$(M,d)$$

b) Prove that $$\overline{S}$$ is closed in $$M$$

**Solution:**

a) The closure is the set of all adherent points of $$S$$

b) To prove $$\overline{S}$$ is closed, we can show that its complement is open.
Suppose that $$x\in M\backslash \overline{S}$$.
Then $$x$$ is not an adherent point of $$S$$.
This means that there exists $$r>0$$ such that $$B_M(x;r)$$ contains no points in $$S$$.

Now suppose that $$y\in B_M(x;r)$$.
Then since $$B_m(x;r)$$ is open, there exists $$s>0$$ such that $$B_M(y;s)\subseteq B_M(x;r)$$.
This means that $$B_M(y;s)$$ contains no points in $$S$$.
Hence $$y$$ is not an adherent point of $$S$$, ie. $$y\in M\backslash \overline{S}$$.
Since $$y\in B_M(x;r)$$ was arbitrary, this proves $$B_M(x;r)\subseteq M\backslash\overline{S}$$.
This proves that $$x$$ is an interior point of $$M\backslash\overline{S}$$.
Since $$x\in M\backslash\overline{S}$$ was arbitrary, this proves every point in $$M\backslash\overline{S}$$ is an interior point.
Hence $$M\backslash\overline{S}$$ is open and $$\overline{S}$$ must be closed.

## Problem 6

a) Write down the definition of a subset $$S\subseteq M$$ of a metric space $$(M,d)$$ being compact

b) Let $$M=\mathbb{R}$$ with the Euclidean metric.  Prove that the half-open interval $(0,1]$ is not compact directly from the definitions, ie. without using the Heine-Borel Theorem.

**Solution:**

a) A subset $$S$$ is compact if every open cover of $$S$$ has a finite subcover.

b) Consider the family of sets defined by $$\{U_i: i\in I\}$$ where the index set $$I=\mathbb{Z}_+$$ and $$U_i = (1/i,2)$$ for all $$i$$.
These are open intervals, so this is a family of open sets.
Moreover, if $$x\in (0,1]$$, then there exists $$n\in\mathbb{Z}_+$$ with $$n>1/x \geq 1$$, so that $$1/n < x\leq 1$$.  This makes $$x\in (1/n,2)= U_n$$ and therefore $$x\in \bigcup_{i\in I} U_i$$.
Since $$x\in(0,1]$$ was arbitrary, we conclude $$(0,1]\subseteq\bigcup_{i\in I} U_i$$.
Hence $$\{U_i: i\in I\}$$ is an open cover of $$(0,1]$$.

Now if $$J\subseteq I$$ is a finite set, then we can write $$J = \{j_1,j_2,\dots, j_n\}$$ for some positive integers $$j_1,j_2,\dots,j_n$$ with

$$j_1 < j_2 < \dots < j_n.$$

The elements in the cover are nested, so

$$U_{j_1}\cup U_{j_2}\cup\dots\cup U_{j_n} = U_{j_n} = (1/j_n,2],$$

which does not cover $$(0,1]$$.
Thus the open cover $$\{U_i: i\in I\}$$ of $$(0,1]$$ has no finite subcover.

## Problem 7

Let $$M=\mathbb{R}$$ with the Euclidean metric and consider the subspace

$$S = \{0\}\cup \{\frac{1}{n}: n\in\mathbb{Z}_+\}.$$

a) Show that if $$x\in S$$ is nonzero, then the singleton set $$\{x\}$$ is open in the subspace $$S$$.

b) Show that the singleton set $$\{0\}$$ is not open in $$S$$

BONUS PRACTICE: is $$S$$ a compact metric space?  Why or why not?

**Solution:**

a) Suppose $$x\in S$$ is greater than zero.  Then $$x=1/n$$ for some positive integer $$n$$.  If we let $$r = 1/n - 1/(n+1) = \frac{1}{n(n+1)}$$ then

$$B_S(x;r) = B_M(x;r)\cap S = (x-r,x+r)\cap S = (1/(n+1),1/n + 1/(n(n+1)))\cap S = \{1/n\} = \{x\}.$$

Therefore $$\{x\}$$ is open in $$S$$, since it is equal to an open ball in the subspace.

b) Suppose that $$r>0$$.  Then there exists $$n\in\mathbb{Z}_+$$ with $$n > 1/r$$.  Therefore $$1/n < r$$ and the ball

$$B_S(0;r) = (-r,r)\cap S$$

contains $$1/n$$.  Thus no ball in $$S$$ around $$0$$ is contained in $$\{0\}$, so $$0$$ is not an interior point of $$\{0\}$$.  This means $$\{0\}$$ is not open.

## Problem 8

Suppose that $$\{x_n\}$$ is a monotone decreasing sequence of real numbers which is bounded below.

a) Show that using the Euclidean metric, $$\{x_n\}$$ will converge (without using the Monotone Convergence Theorem!)

b) Give an example showing that under the discrete metric, $$\{x_n\}$$ actually might not converge

**Solution:**

a) As a consequence of the Completeness Axiom and results from the homework, any set of real numbers which is bounded below has an infimum.
Let $$X$$ be the set of all values of $$X$$ and let $$L = \inf(X)$$.  We will show that $$\lim x_n = L$$.

Let $$\epsilon > 0$$.
Then since $$L$$ is the greatest lower bound, $$L+\epsilon$$ is not a lower bound of $$X$$.
Therefore there exists $$x\in X$$ with $$x < L+\epsilon$$.
Furthermore, there exists $$N\in\mathbb{Z}_+$$ with $$x = x_N$$.
Then since $$x_n$$ is monotone decreasing, for all $$n\geq N$$ we have

$$d(x_n,L) = |x_n-L| = x_n - L < x_N - L < \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves $$\{x_n\}$$ converges to $$L$$.

b) The statement is not true for the discrete metric. For example, the sequence defined by $$x_n = 1/n$$ is monotone decreasing and bounded below by $$0$$.
However, it does not converge.  To see this, suppose that it did converge to some real number $$L$$.
Then if we take $$\epsilon = 1$$, there should exists $$N\in\mathbb{Z}_+$$ with $$d(x_n,L) < 1$$ for all $$n\geq N$$.
For the discrete metric $$d(x,y) < 1$$ if and only if $$x=y$$, so this would require $$x_n=L$$ for all $$n\geq N$$.
In other words, our sequence would have to be eventually constant and equal to the value $$L$$, but the value of our sequence continues to change.
This is a contradiction.


