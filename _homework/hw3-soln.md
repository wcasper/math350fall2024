---
layout: page
title: Homework 3 Solutions
permalink: /homework/hw3-soln
---

### Directions
Solve the following problems and write up your solutions.  Your solutions should be provided in one of the following formats (in order of preference)
* typed up in $$\LaTeX$$ and submitted as a PDF on Canvas
* written legibly on blank paper, scanned into a PDF and then uploaded on Canvas
* written on ancient parchement with a quill and then flown to the instructor via owl post like in Harry Potter

If you go with the first strategy, you may wish to check out Overleaf which is a free and intuitive website for generating $$\LaTeX$$ documents online.
If you wish to use the second method and don't own a scanner at home, you can check out the numerous scanning apps available for smartphones.

You will be graded based on *completion* of all of the assigned problems, along with in-depth grading of *select* problems which will not be revealed until after the homework is graded.

**Remember:** Success in any math class is based on *practice*.  The assigned homework problems are the **bare minimum**.  You should strive to do as many problems as possible from the textbook.

### Problems

* 3.2, 3.9, 3.12 part e and f, 3.13, 3.17, 3.18

**Problem 3.2 Solution:**

* a) no accumulation points; closed;
* b) accumulation points $$[a,b]$$; neither;
* c) only accumulation point is $$0$$; neither;
* d) accumulation points $$\mathbb{R}$$; neither;
* e) only accumulation point is $$0$$; neither;
* f) accumulation points $$1$$ and $$-1$$; neither;
* g) accumulation points $$0$$ and $$1/n$$ for all $$n\in\mathbb{Z}_+$$; neither;
* h) accumulation points $$1$$ and $$-1$$; neither;

**Problem 3.9 Solution:**

Let $$A\subseteq\mathbb{R}^n$$ and let $$U=\text{int}(A)$$.
Suppose that $$x\in U$$.
Then $$x$$ is an interior point of $$A$$, so there exists $$r > 0$$ such that $$B(x;r)\subseteq A$$.
Now suppose $$x\in B(x;r)$$.
Then since $$B(x;r)$$ is open, there exists $$s>0$$ such that $$B(y;s)\subseteq B(x;r)$$.
In particular, this means $$B(y;s)\subseteq A$$, so that $$y$$ is an interior point of $$A$$.
Hence $$y\in U$$.
Since $$y\in B(x;r)$$ was arbitrary, this proves $$B(x;r)\subseteq U$$.
Therefore $$x$$ is an interior point of $$U$$.
Since $$x\in U$$ was arbitrary, this proves that $$U$$ is open.

**Problem 3.12 e and f Solution:**

e) To prove $$\overline{S}$$ is closed, we can show that its complement is open.
Suppose that $$x\in M\backslash \overline{S}$$.
Then $$x$$ is not an adherent point of $$S$$.
This means that there exists $$r>0$$ such that $$B(x;r)$$ contains no points in $$S$$.

Now suppose that $$y\in B(x;r)$$.
Then since $$B(x;r)$$ is open, there exists $$s>0$$ such that $$B(y;s)\subseteq B(x;r)$$.
This means that $$B(y;s)$$ contains no points in $$S$$.
Hence $$y$$ is not an adherent point of $$S$$, ie. $$y\in M\backslash \overline{S}$$.
Since $$y\in B(x;r)$$ was arbitrary, this proves $$B(x;r)\subseteq M\backslash\overline{S}$$.
This proves that $$x$$ is an interior point of $$M\backslash\overline{S}$$.
Since $$x\in M\backslash\overline{S}$$ was arbitrary, this proves every point in $$M\backslash\overline{S}$$ is an interior point.
Hence $$M\backslash\overline{S}$$ is open and $$\overline{S}$$ must be closed.

f) Let $$\Lambda$ be the family consisting of all closed subsets of $$\mathbb{R}^n$$ containing $$S$$, and let $$X = \bigcap_{C\in \Lambda} C$$.
Then $$\overline{S}$$ is closed and contains $$S$$, so $$\overline{S}\in\Lambda$$.
Therefore $$X=\bigcap_{C\in\Lambda} C\subseteq\overline{S}$$.
Conversely, $$X=\bigcap_{C\in\Lambda} C$$ is the intersection of a bunch of closed sets, and is therefore closed.
In particular, $$X$$ contains all of its adherent points.
Every adherent point of $$X$$ is an adherent point of $$S$$, so it follows $$\overline S\subseteq\overline X = X$$.
Hence $$\overline S = X$$.

**Problem 3.13 Solution:**
Since $$S\cap T\subseteq \subseteq \overline S$$ and $$S\cap T\subseteq T\subseteq \overline T$$, we have $$S\cap T\subseteq \overline S\cap \overline T$$.
Therefore by 3.12f, we know $$\overline{S\cap T}\subseteq \overline S\cap\overline T$$.

Now if $$S$$ is open, then for any $$x\in S\cap\overline{T}$$, we have $$x\in S$$ and $$x\in\overline T$$.
We need to show that $$x$$ is an adherent point of $$S\cap T$$.
Let $$r > 0$$.
Then since $$x$$ is an interior point of $$S$$, there exists $$s > 0$$ such that $$B(x;s)\subseteq S$$.
Without loss of generality, we may assume $$s\leq r$$.
Moreover, since $$x$$ is an adherent point of $$T$$, the ball $$B(x;s)$$ contains an element of $$T$$.
Since $$B(x;s)\subseteq S$$, it follows that $$B(x;s)$$ contains an element of $$S\cap T$$.
Hence $$B(x;r)$$ contains an element of $$S\cap T$$, and since $$r > 0$$ is arbitrary, this proves that $$x$$ is an adherent point of $$S\cap T$$.
Hence $$x\in\overline{S\cap T}$$.
Since $$x\in S\cap\overline{T}$$ was arbitrary, this proves
$$S\cap\overline{T}\subseteq\overline{S\cap T}$$.

**Problem 3.17 Solution:**
Let $$A$$ be the set of isolated points of $$S$$.
Then for all $$a\in A$$, there exists $$r_a >0$$ with $$B(a;r_a)\cap S = \{a\}$$.
The set $$\{B(a;r_a): a\in A\}$$ is an open cover of $$A$$.
If we throw out any sets in this cover, we no longer cover $$A$$.
If $$A$$ is uncountable, this would contradict Lindelof's Theorem.
Therefore $$A$$ is countable.

**Problem 3.18 Solution:**

Let $$(x,y)\in\mathbb{R}^2$$ with $$x,y > 0$$.
Then by the density of the rationals, for all $$\epsilon > 0$$, we can choose $$(a,b)$$ with $$a,b\in\mathbb{Q}$$ and

$$x < a < x+\epsilon,\quad\text{and}\quad y < b < y+\epsilon.$$

Choose $$\epsilon = \min(x,y)/2$$.
Then for the rational number $$r=\max(a,b)$$, the triangle inequality says

$$\begin{align}
\sqrt{(x-r)^2+(y-r)^2}
  & \leq \sqrt{(x-a)^2+(y-b)^2} + \sqrt{(a-r)^2+(b-r)^2}\\
  & =  \sqrt{(x-a)^2+(y-b)^2} + \max(a,b)-\min(a,b)\\
  & \leq |x-a|+|y-b| + \max(a,b)-\min(a,b)\\
  & < \min(x,y) + \max(a,b)-\min(a,b)\\
  & < \max(a,b) = r.
\end{align}$$
Therefore $$(x,y)\in B((r,r);r)$$.
Since the point we picked was arbitrary, this proves

$$\bigcup_{r\in\mathbb Q_+} B((r,r),r) = \{(x,y)\in\mathbb{R}^2: x>0,\ y>0\}.$$

