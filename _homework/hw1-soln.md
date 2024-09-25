---
layout: page
title: Homework 1 Solutions
permalink: /homework/hw1-soln
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

* 1.6, 1.11, 1.20, 1.21, 1.23, 1.25

### Solution to 1.6

Let $$A$$ be a set of positive integers and consider $$-A = \{-a: a\in A\}.$$

The set $$-A$$ is bounded above by $$0$$.
Since $$-A$$ is also a set of integers, a result we proved in class tells us that $$-A$$ has a maximum $$k$$.
This means $$k\in -A$$ and $$k\geq x$$ for all $$x\in -A$$.
It follows that $$-k\in A$$ and $$k\geq -a$$ for all $$a\in A$$.
Thus $$-k\in A$$ and $$-k\leq -a$$ for all $$a\in A$$.
Hence $$-k$$ is a minimum element of $$A$$.
In particular $$A$$ has a minimum element.

### Solution to 1.11

First, suppose that $$x$$ is rational.
Then the number $$y = x/\sqrt{2}$$ lies between $$0$$ and $$x$$.
Moreover, if $$y$$ were rational, then $$\sqrt{2} = x/y$$ would also be rational, which we know it is not!
Therefore $$y$$ is an irrational number between $$0$$ and $$x$$.

Next, suppose instead that $$x$$ is irrational.
Then the number $$y = x/2$$ lies between $$0$$ and $$x$$.
Moreover, if $$y$$ were rational, then $$x = 2y$$ would also be rational, which we know it is not!
Therefore $$y$$ is an irrational number between $$0$$ and $$x$$.

In either case, we have an irrational number between $$0$$ and $$x$$.

### Solution to 1.20

Since $$T$$ is nonempty, we may choose a $$t_0\in T$$.
Then $$s\leq t_0$$ for all $$s\in S$$, and therefore $$S$$ is bounded above by $$t_0$$.
Thus by the completeness axiom, $$S$$ has a supremum $$\sup(S)$$.

If $$t_0 < \sup(S)$$, then by definition it cannot be an uppere bound of $$S$$.  Hence $$\sup(S)\leq t_0$$.
Furthermore, since $$\sup(T)$$ is an upper bound of $$T$$, we know $$t_0\leq \sup(T)$$.

Hence (you're welcome Jose):

$$\sup(S)\leq t_0 \leq \sup(T).$$

In particular $$\sup(S)\leq\sup(T)$$.

### Solution to 1.21

First of all, we know that $$a$$ is an upper bound of $$A$$, so that $$x\leq a$$ for all $$x\in A$$.
Likewise $$y\leq b$$ for all $$y\in B$$.
Consequently $$xy\leq ab$$ for all $$x\in A$$ and $$y\in B$$.

If $$z\in C$$, then $$z = xy$$ for some $$x\in A$$ and $$y\in B$$.
It follows from the previous paragraph that $$z\leq ab$$, and therefore $$ab$$ is an upper bound of $$C$$.
Thus by the completeness axiom, $$C$$ has a supremum.
Let $$c = \sup(C)$$.
Since the supremum of $$C$$ is the least upper bound, we know $$c\leq ab$$.

Next, note that for all $$x\in A$$ and $$y\in B$$ we have $$xy\leq c$$.
Therefore $$x\leq (c/y)$$, so that $$(c/y)$$ is an upper bound of $$A$$ for all $$y\in B$$.
Since the supremum of $$A$$ is the least upper bound of $$A$$, it follows $$a\leq (c/y)$$.
Thus $$y\leq (c/a)$$ for all $$y\in B$$, making $$c/a$$ an upper bound of $$B$$.
Since the supremum of $$B$$ is the least upper bound of $$B$$, it follows $$b\leq (c/a)$$.
Whence $$ab\leq c$$.

Putting the results of the previous two paragraphs together, we get $$c=ab$$.

### Solution to 1.23

We have to foil the crap out of it...

$$\begin{align}
\left(\sum_{k=1}^n a_kb_k\right)^2
  & = \sum_{j,k=1}^n a_jb_ja_kb_k\\
  & = \sum_{1\leq j < k\leq n} a_jb_ja_kb_k + \sum_{1\leq k < j\leq n} a_jb_ja_kb_k + \sum_{k=1}^n a_k^2b_k^2\\
  & = 2\sum_{1\leq j < k\leq n} a_jb_ja_kb_k + \sum_{k=1}^n a_k^2b_k^2\\
  & = \sum_{1\leq j < k\leq n} 2a_jb_ja_kb_k + \sum_{k=1}^n a_k^2b_k^2
\end{align}$$

$$\begin{align}
\left(\sum_{k=1}^n a_k^2\right)\left(\sum_{k=1}^n b_k^2\right)
  & = \sum_{j,k=1}^n a_j^2b_k^2\\
  & = \sum_{1\leq j < k \leq n} a_j^2b_k^2 + \sum_{1\leq k < j \leq n} a_j^2b_k^2 + \sum_{k=1}^n a_j^2b_k^2\\
  & = \sum_{1\leq j < k \leq n} a_j^2b_k^2 + \sum_{1\leq j < k \leq n} a_k^2b_j^2 + \sum_{k=1}^n a_j^2b_k^2\\
  & = \sum_{1\leq j < k \leq n} (a_j^2b_k^2 +  a_k^2b_j^2) + \sum_{k=1}^n a_j^2b_k^2
\end{align}$$

Therefore

$$\begin{align}
\left(\sum_{k=1}^n a_kb_k\right)^2 
  & - \left(\sum_{k=1}^n a_k^2\right)\left(\sum_{k=1}^n b_k^2\right)\\
  & = \sum_{1\leq j < k \leq n} (-a_j^2b_k^2 -  a_k^2b_j^2 + 2a_jb_ja_kb_k)\\
  & = -\sum_{1\leq j < k \leq n} (a_j^2b_k^2 +  a_k^2b_j^2 - 2a_jb_ja_kb_k)\\
  & = -\sum_{1\leq j < k \leq n} (a_kb_j-a_jb_k)^2
\end{align}$$

### Solution to 1.25

First of all, by the Triangle Inequality:

$$\begin{align}
\sum_{k=1}^n (a_k + b_k)^2 
  &= \sum_{k=1}^n \lvert a_k + b_k \rvert^2\\
  &= \sum_{k=1}^n \lvert a_k + b_k \rvert\ \lvert a_k + b_k \rvert\\
  &\leq \sum_{k=1}^n (\lvert a_k\rvert + \lvert b_k \rvert)\lvert a_k + b_k \rvert\\
  &= \sum_{k=1}^n \lvert a_k\rvert\ \lvert a_k + b_k \rvert\\
  &+ \sum_{k=1}^n \lvert b_k\rvert\ \lvert a_k + b_k \rvert
\end{align}$$

Then by the Cauchy-Schwarz Inequality:

$$\begin{align}
\sum_{k=1}^n (a_k + b_k)^2 
  &\leq \left(\sum_{k=1}^n a_k^2\right)^{1/2}\left(\sum_{k=1}^n (a_k+b_k)^2\right)^{1/2}\\
  &+    \left(\sum_{k=1}^n b_k^2\right)^{1/2}\left(\sum_{k=1}^n (a_k+b_k)^2\right)^{1/2}
\end{align}$$

Now dividing both sides of the inequality by $$\left(\sum_{k=1}^n (a_k+b_k)^2\right)^{1/2}$$, we get

$$\left(\sum_{k=1}^n (a_k + b_k)^2 \right)^{1/2} \leq \left(\sum_{k=1}^n a_k^2\right)^{1/2} + \left(\sum_{k=1}^n b_k^2\right)^{1/2}$$

