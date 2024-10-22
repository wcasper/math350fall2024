---
layout: page
title: Homework 4 Solutions
permalink: /homework/hw4-soln
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

* 3.30, 3.39, 3.45, 4.7

**Solution to Problem 3.30:**

Let $$A\subseteq M$$ be a finite collection of points.
To prove $$A$$ is closed, we will show that its complement is open.

Let $$x\in M\backslash A$$.
Then the set

$$D = \{d(x,a): a\in A\}$$

is a finite set of positive numbers, and therefore must have a minimum value $$r=\min D$$.
Since the minimum is also a member of $$D$$ and all the elements of $$D$$ are positive, we also know $$r>0$$.
The ball

$$B_M(x;r) = \{y\in M: d(x,y) < r\}$$

cannot contain any points in $$A$$, so $$B_M(x;r)\subseteq M\backslash A$$.
This proves that $$x$$ is an interior point of $$B_M(x;r)\subseteq M\backslash A$$.
Since it was arbitrary, every point in $$B_M(x;r)\subseteq M\backslash A$$ is an interior point, making the set open.
Hence $$A$$ itself is closed.


**Solution to Problem 3.39:**

Suppose $$S$$ is closed and $$T$$ is compact, and let $$\{U_i: i\in I\}$$ be an open cover of $$S\cap T$$.
Then the set $$V = M \backslash S$$ is open and $$\{U_i: i\in I\}\cup\{V\}$$ is an open cover of $$T$$.
Since $$T$$ is compact, it must have a finite subcover, which without loss of generality will be of the form

$$\{U_{i_1}, U_{i_2},\dots, U_{i_r},V\}.$$

This is an open cover of $$T$$, and therefore also covers $$S\cap T$$.
Moreover, $$V$$ does not contain any points of $$S$$, so it contains no points of $$S\cap T$$.
Therefore if we want to cover $$S\cap T$$ only, we can throw it out leaving us with

$$\{U_{i_1}, U_{i_2},\dots, U_{i_r}\}$$

as an open cover of $$S\cap T$$.  This is also a subcover of $$\{U_i: i\in I\}$$!  In this way, we have shown every open cover of $$S\cap T$$ has a finite subcover, meaning that $$S\cap T$$ must be compact.


**Solution to Problem 3.45:**
Every interior point of a set is also an element of that set, meaning that $$\text{int}(X)\subseteq X$$ for any set $$X\subseteq M$$.
In particular, for $$X=\text{int}(A)$$ we know $$\text{int}(\text{int}(A))\subseteq \text{int}(A)$$.
The interesting part is proving the converse.

Suppose that $$x\in\text{int}(A)$$.
Then $$x$$ is an interior point of $$A$$.
Therefore there exists $$r>0$$ such that $$B_M(x;r)\subseteq A$$.
Now since open balls in a metric space are open sets, for any $$y\in B_M(x;r)$$, there exists $$s>0$$ such that $$B_M(y;s)\subseteq B_M(x;r)$$.
However, this implies that $$B_M(y;s)\subseteq A$$, meaning that $$y$$ is an interior point of $$A$$.
Since $$y\in B_M(x;r)$$ was arbitrary, this proves that every element of $$B_M(x;r)$$ is an interior point of $$A$$, ie. $$B_M(x;r)\subseteq\text{int}(A)$$.
This proves that $$x$$ is an interior point of $$\text{int}(A)$$, ie. $$x\in \text{int}(\text{int}(A))$$.
Since $$x\in\int(A)$$ was arbitrary, this proves $$\text{int}(A)\subseteq \text{int}(\text{int}(A)).$$

**Solution to Problem 3.47:**
By the triangle inequality applied twice, we have

$$d(x_n,y_n)\leq d(x_n,x) + d(x,y_n)\leq d(x_n,x) + d(x,y) + d(y,y_n).$$

This tells us $$d(x_n,y_n)-d(x,y)\leq d(x_n,x) + d(y,y_n).$$

Likewise, the triangle inequality applied twice tells us

$$d(x,y)\leq d(x,x_n) + d(x_n,y)\leq d(x,x_n) + d(x_n,y_n) + d(y_n,y).$$

Remembering symmetry, this tells us $$d(x,y)-d(x_n,y_n)\leq d(x_n,x) + d(y,y_n).$$

Putting these two results together, we get that for all $$n\in\mathbb{Z}_+$$

$$|d(x,y)-d(x_n,y_n)|\leq d(x_n,x) + d(y,y_n).$$

Let $$\epsilon > 0$$.
Then we can choose $$N_1\in\mathbb{Z}_+$$ such that $$n\geq N_1$$ implies $$d(x_n,x) < \epsilon /2$$.
Likewise, we can choose $$N_2\in\mathbb{Z}_+$$ such that $$n\geq N_1$$ implies $$d(y_n,y) < \epsilon /2$$.
Therefore, if we take $$N = \max(N_1,N_2)$$, then for all $$n\geq N$$ we have

$$|d(x,y)-d(x_n,y_n)|\leq d(x_n,x) + d(y,y_n) < \epsilon/2 + \epsilon/2 = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that

$$\lim_{n\rightarrow\infty} d(x_n,y_n) = d(x,y).$$

