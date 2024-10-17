---
layout: page
title: Homework 2 Solutions
permalink: /homework/hw2-soln
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

Note: in Apstol's notation, $$A\sim B$$ means $$\lvert A\rvert = \lvert B\rvert$$.

* 2.2,2.7,2.9,2.11,2.12,2.18

Additional problem: Let $$A$$ be an infinite set and suppose $$q$$ is an element that is not in $$A$$.  Prove that $$A$$ and $$A\cup\{q\}$$ have the same cardinality.


### Solutions

**Problem 2.2 Solution:**

* a) reflexive, transitive 
* b) transitive
* c) none
* d) symmetric
* e) symmetric, transitive
* f) reflexive, symetric, transitive

**Problem 2.7 Solution:**

* a) Let $$Y=f(X)$$.  We need to show that $$X\subseteq f^{-1}(Y)$$.  Let $$x\in X$$.  Then $$f(x)\in Y$$ and $$x\in S$$, so $$x\in f^{-1}(Y)$$.  Since $$x\in X$$ was arbitrary, this proves $$X\subseteq f^{-1}(Y)$$.
* b) Let $$X=f^{-1}(Y)$$.  We need to show that $$f(X)\subseteq Y$$.  Let $$y\in f(X)$$.  Then there exists $$x\in X$$ such that $$y = f(x)$$.  Moreover, since $$x\in X=f^{-1}(Y)$$ we know that $$x\in S$$ and $$f(x)\in Y$$.  Hence $$y=f(x)\in Y$$.  Since $$y\in f(X)$$ was arbitrary, this proves $$f(X)\subseteq Y.$$
* c)
Suppose that $$x\in f^{-1}(Y_1\cup Y_2)$$.
Then $$x\in S$$ and $$f(x)\in Y_1\cup Y_2$$.
Therefore $$f(x)\in Y_1$$ or $$f(x)\in Y_2$$.
Consequently, $$x\in f^{-1}(Y_1)$$ or $$x\in f^{-1}(Y_2)$$.
Hence $$x\in f^{-1}(Y_1)\cup f^{-1}(Y_2)$$.
Since $$x\in f^{-1}(Y_1\cup Y_2)$$ was arbitrary, this proves $$f^{-1}(Y_1\cup Y_2)\subseteq f^{-1}(Y_1)\cup f^{-1}(Y_2).$$

Conversely, suppose that $$x\in f^{-1}(Y_1)\cup f^{-1}(Y_2)$$.
Then $$x\in f^{-1}(Y_1)$$ or $$x\in f^{-1}(Y_2)$$.
Therefore $$x\in S$$ and $$f(x)\in Y_1$$ or $$f(x)\in Y_2$$.
It follows that $$f(x)\in Y_1\cup Y_2$$.
Therefore $$x\in f^{-1}(Y_1\cup Y_2)$$.
Since $$x\in f^{-1}(Y_1)\cup f^{-1}(Y_2)$$ was arbitrary, this proves $$f^{-1}(Y_1)\cup f^{-1}(Y_2)\subseteq f^{-1}(Y_1\cup Y_2)$$.
Putting this together with the result of the previous paragraph, we conclude $$f^{-1}(Y_1) = f^{-1}(Y_2)\subseteq f^{-1}(Y_1\cup Y_2)$$.

* d)
Suppose that $$x\in f^{-1}(Y_1\cap Y_2)$$.
Then $$x\in S$$ and $$f(x)\in Y_1\cap Y_2$$.
Therefore $$f(x)\in Y_1$$ and $$f(x)\in Y_2$$.
Consequently, $$x\in f^{-1}(Y_1)$$ and $$x\in f^{-1}(Y_2)$$.
Hence $$x\in f^{-1}(Y_1)\cap f^{-1}(Y_2)$$.
Since $$x\in f^{-1}(Y_1\cap Y_2)$$ was arbitrary, this proves $$f^{-1}(Y_1\cap Y_2)\subseteq f^{-1}(Y_1)\cap f^{-1}(Y_2).$$

Conversely, suppose that $$x\in f^{-1}(Y_1)\cap f^{-1}(Y_2)$$.
Then $$x\in f^{-1}(Y_1)$$ or $$x\in f^{-1}(Y_2)$$.
Therefore $$x\in S$$ and $$f(x)\in Y_1$$ and $$f(x)\in Y_2$$.
It follows that $$f(x)\in Y_1\cap Y_2$$.
Therefore $$x\in f^{-1}(Y_1\cap Y_2)$$.
Since $$x\in f^{-1}(Y_1)\cap f^{-1}(Y_2)$$ was arbitrary, this proves $$f^{-1}(Y_1)\cap f^{-1}(Y_2)\subseteq f^{-1}(Y_1\cap Y_2)$$.
Putting this together with the result of the previous paragraph, we conclude $$f^{-1}(Y_1) = f^{-1}(Y_2)\subseteq f^{-1}(Y_1\cap Y_2)$$.

* e)
Suppose that $$x\in f^{-1}(T\backslash Y)$$.
Then $$x\in S$$ and $$f(x)\in T\backslash Y$$.
In particular, $$f(x)\notin Y$$ and therefore $$x\notin f^{-1}(Y)$$.
Hence $$x\in S\backslash f^{-1}(Y)$$.
Since $$x\in f^{-1}(T\backslash Y)$$ was arbitrary, this proves $$f^{-1}(T\backslash Y)\subseteq S\backslash f^{-1}(Y)$$.

Conversely, suppose that $$x\in S\backslash f^{-1}(Y).$$
Then $$x\in S$$ but $$x\notin f^{-1}(Y)$$.
Therefore $$f(x)\notin Y$$.
It follows that $$f(x)\in T\backslash Y$$, so that $$x\in f^{-1}(T\backslash Y)$$.
Since $$x\in S\backslash f^{-1}(Y)$$ was arbitrary, this proves $$S\backslash f^{-1}(Y)\subseteq f^{-1}(T\backslash Y)$$.
Putting this together with the results of the previous paragraph, we conclude $$S\backslash f^{-1}(Y)= f^{-1}(T\backslash Y)$$.

* f) To spice things up, we will do the proofs bidirectionally this time.  Let $$\{Y_i: i\in I\}$$ be a family of sets.

Then we have

$$\begin{align}
x\in f^{-1}\left(\bigcup_{i\in I} Y_i\right)
  & \Leftrightarrow x\in S,\ \text{and}\ f(x)\in \bigcup_{i\in I} Y_i\\
  & \Leftrightarrow x\in S,\ \text{and}\ f(x)\in Y_i,\ \text{for some $i\in I$}\\
  & \Leftrightarrow x\in S,\ \text{and}\ x\in f^{-1}(Y_i),\ \text{for some $i\in I$}\\
  & x\in \bigcup_{i\in I} f^{-1}(Y_i).
\end{align}$$

Since $$x$$ was arbitrary, this proves $$f^{-1}\left(\bigcup_{i\in I} Y_i\right) = \bigcup_{i\in I} f^{-1}(Y_i)$$.

Likewise,

$$\begin{align}
x\in f^{-1}\left(\bigcap_{i\in I} Y_i\right)
  & \Leftrightarrow x\in S,\ \text{and}\ f(x)\in \bigcap_{i\in I} Y_i\\
  & \Leftrightarrow x\in S,\ \text{and}\ f(x)\in Y_i,\ \text{for all $i\in I$}\\
  & \Leftrightarrow x\in S,\ \text{and}\ x\in f^{-1}(Y_i),\ \text{for all $i\in I$}\\
  & x\in \bigcap_{i\in I} f^{-1}(Y_i).
\end{align}$$

Since $$x$$ was arbitrary, this proves $$f^{-1}\left(\bigcap_{i\in I} Y_i\right) = \bigcap_{i\in I} f^{-1}(Y_i)$$.

**Problem 2.9 Solution:**

Let's do a fancypants round-robin type argument.

* a) implies b)
Assume $$f$$ is one to one on $$S$$, and let $$A,B\subseteq S$$.

If $$y\in f(A\cap B)$$, then $$y=f(x)$$ for some $$x\in A\cap B$$.
This means $$x\in A$$ and $$x\in B$$.
It follows that $$y\in f(A)$$ and $$y\in f(B)$$.
Hence $$y\in f(A)\cap f(B)$$.
Since $$y$$ is arbitrary, this proves $$f(A\cap B)\subseteq f(A)\cap f(B)$$.
[Note: this is basically problem 2.6 so far, and we haven't used injectivity].

Conversely, assume $$y\in f(A)\cap f(B)$$.
Then $$y=f(a)$$ for some $$a\in A$$ and $$y=f(b)$$ for some $$b\in B$$.
However, since $$f$$ is injective and $$f(a)=f(b)$$ we must have $$a=b$$.
In particular, $$a$$ belongs to both $$A$$ and $$B$$, ie. $$a\in A\cap B$$.
Hence $$y\in f(A\cap B)$$.
Since $$y$$ was arbitrary, this proves $$f(A)\cap f(B)=f(A\cap B)$$.

Since $$A$$ and $$B$$ were arbitrary subsets of $$S$$, this proves
$$f(A\cap B) = f(A)\cap f(B)$$ for all subsets $$A,B$$ of $$S$$

* b) implies c)
Assume $$f(A\cap B) = f(A)\cap f(B)$$ for all subsets $$A,B$$ of $$S$$.

Let $$A\subseteq S$$.
From Problem 2.7, we know $$A\subseteq f^{-1}(f(A))$$.
If this is not an equality, then there exists $$x\in f^{-1}(f(A))$$ with $$x\notin A$$.
This means that $$x\in S$$ and $$f(x)\in f(A)$$ buth $$x\notin A$$.
Let $$B = \{x\}$$.
Then $$f(B) = \{f(x)\}$$ and $$f(A)\cap f(B) = \{f(x)\}.$$
However, $$A\cap B = \varnothing$$, so $$f(A\cap B) = f(\varnothing) = \varnothing$$.
Since we know $$f(A\cap B) = f(A)\cap f(B)$$, this is a contradiction!
Therefore we must have equality, ie. $$A = f^{-1}(f(A))$$.

Since $$A\subseteq S$$ was arbitrary, this proves  $$f^{-1}(f(A))=A$$ for all $$A\subseteq S$$.

* c) implies d)
Assume $$f^{-1}(f(A))=A$$ for all $$A\subseteq S$$.

Let $$A$$ and $$B$$ be disjoint subsets of $$S$$.  If $$f(A)$$ and $$f(B)$$ are not disjoint, then there exists $$y\in f(A)\cap f(B)$$.
This means that $$y\in f(A)$$ and $$y\in f(B)$$.
Therefore there exists $$a\in A$$ with $$y=f(a)$$ and $$b\in B$$ with $$y=f(b)$$.
Since $$A$$ and $$B$$ are disjoint, we know $$b\notin A$$.
However, $$f(b) = f(a)\in f(A)$$, and therefore $$b\in f^{-1}(f(A))$$.
This contradicts the fact that $$f^{-1}(f(A))=A$$.
We conclude that $$f(A)$$ and $$f(B)$$ must be disjoint.
Since $$A$$ and $$B$$ were arbitrary disjoint subsets of $$S$$, this proves that for all disjoint subsets $$A$$ and $$B$$ of $$S$$, the images $$f(A)$$ and $$f(B)$$ must be disjoint.

* d) implies a)
Assume that for all disjoint subsets $$A$$ and $$B$$ of $$S$$, the images $$f(A)$$ and $$f(B)$$ must be disjoint.

Suppose that $$a,b\in S$$ with $$a\neq b$$.
Then the sets $$A$$ and $$B$$ defined by $$A = \{a\}$$ and $$B = \{b\}$$ are disjoint.
Therefore $$f(A) = \{f(a)\}$$ and $$f(B) = \{f(b)\}$$ are disjoint.
In particular, we see $$f(a)\neq f(b)$$.
Thus if $$a,b\in S$$ with $$f(a)=f(b)$$, we must have $$a=b$$.
This proves $$f$$ is injective.


**Problem 2.11 Solution:**

We proceed by induction on $$m$$.

Base case: Suppose that $$m=1$$.  Then if

$$\{1\} \sim \{1,2,\dots,n\}$$

then there exists a bijection $$f: \{1\} \sim \{1,2,\dots,n\}$$
If $$n>1$$, both $$1$$ and $$2$$ are elements of the codomain.  Thus surjectivity implies there exists $$x_1\in \{1\}$$ such that $$f(x) = 1$$ and there exists $$x_2\in \{1\}$$ such that $$f(x) = 2$$.
However, this would mean $$f(1) = 1$$ and $$f(2) = 1$$, which would contradict $$f$$ being a function!
Thus $$n=1$$.

Inductive assumption:  Suppose that for an integer $$m\geq 1$$, if $$\{1,2,\dots,m\} \sim \{1,2,\dots,n\}$$ then $$m=n$$.

Inductive step:  Suppose that $$\{1,2,\dots, m+1\}\sim \{1,2,\dots,n\}$$.  Then there exists a bijection $$f:\{1,2,\dots, m+1\}\rightarrow \{1,2,\dots,n\}$$.
Let $$k=f(m+1)$$ and consider the bijection $$\sigma: \{1,2,\dots, n\}\rightarrow\{1,2,\dots, n\}$$ defined by the permutation

$$\sigma(x) = \left\lbrace
n & x=k\\
k & x=n\\
x & \text{otherwise}
\right.$$

The composition of bijections is a bijection, so $$g = \sigma\circ f: \{1,2,\dots, m+1\}\rightarrow \{1,2,\dots,n\}$$ is a bijection.
Moreover, $$g(m+1) = \sigma(f(m+1))=\sigma(k)=n$$, so the restriction of $$g$$ to $$\{1,2,\dots,m\}$$ defines a bijection
$$\{1,2,\dots,m\}\rightarrow\{1,2,\dots,n-1\}$$.
Hence $$\{1,2,\dots,m\}\sim\{1,2,\dots,n-1\}$$, and by our inductive assumption $$m=n-1$$.
Therefore $$n=m+1$$.

Thus by the Principle of Induction, $$\{1,2,\dots,m\}\sim\{1,2,\dots,n\}$$ implies $$m=n$$ for all $$m$$ and $$n$$.

**Problem 2.12 Solution:**

Suppose that $$S$$ is an infinite set.
Choose $$a_1\in S$$, $$a_2\in S \backslash \{a_1\}$$, $$a_3\in S\backslash \{a_1,a_2\}$$ and in general

$$a_n\in S\backslash \{a_1,a_2,\dots,a_{n-1}\},\quad n\geq 4.$$

Note this is possible since $$S$$ is infinite, so that the set we are selecting from is nonempty every time.
The set $$A = \{a_k: k\in \mathbb{Z}_+\}$$ is a subset of $$S$$.
Moreover, the function

$$f: \mathbb{Z}_+\rightarrow A,\quad f(k) = a_k$$

is a bijection.  Thus $$A$$ has the same cardinality as $$\mathbb Z_+$$, making it countably infinite.

**Problem 2.18 Solution:**

We use a version of Cantor diagonalization.

Suppose that $$S$$ was countable.
Then there would be a bijection

$$f: \mathbb Z_+ \rightarrow S.$$

Now let

$$\begin{align}
f(1) &= (b_{11},b_{12},b_{13},b_{14},\dots)\\
f(2) &= (b_{21},b_{22},b_{23},b_{24},\dots)\\
f(3) &= (b_{31},b_{32},b_{33},b_{34},\dots)\\
\vdots
\end{align}$$

and consider the binary sequence $$(q_1,q_2,q_3,\dots)$$ defined by $$q_k = 1-b_{kk}$$ for all $$k\in\mathbb Z_+$$.

Since $$f$$ is surjective, we must have $$f(n) = (q_1,q_2,q_3,\dots)$$ for some $$n\in\mathbb{Z}_+$$.
This implies

$$(b_{n1},b_{n2},b_{n3},b_{n4},\dots) = (q_1,q_2,q_3,q_4,\dots)$$

and by looking at the $$n$$'th term in both sequences, we see

$$b_{nn} = q_n = 1-b_{nn}.$$ 

This says $$2b_{nn} = 1$$, making $$b_{nn} = 1/2$$, which is impossible for a binary sequence!
We conclude that $$S$$ cannot be countable.

**Additional problem solution:**
Suppose that $$A$$ is an infinite set.
Choose $$a_1\in A$$, $$a_2\in A \backslash \{a_1\}$$, $$a_3\in A\backslash \{a_1,a_2\}$$ and in general

$$a_n\in A\backslash \{a_1,a_2,\dots,a_{n-1}\},\quad n\geq 4.$$

Note this is possible since $$A$$ is infinite, so that the set we are selecting from is nonempty every time.
Now consider the functions

$$f: A\rightarrow A\cup\{q\},\quad\text{and}\quad g: A\cup\{q\}\rightarrow A$$

defined by

$$f(x) = \left\lbrace\begin{array}{cc}
a_{n-1} & x=a_n\ \text{for some integer $n\geq 2$}\\
q     & x=a_1\\
x       & \text{otherwise}
\end{array}\right.$$

$$g(y) = \left\lbrace\begin{array}{cc}
a_{n+1} & y=a_n\ \text{for some integer $n\geq 1$}\\
a_1     & y=q\\
y       & \text{otherwise}
\end{array}\right.$$

These two functions are inverses, ie.

$$f(g(y)) = y\ \forall y\in A\cup\{q\},\quad\text{and}\quad g(f(x)) = x\ \forall\ x\in A.$$ 

The only functions with inverses are bijections, so $$f$$ is a bijection.
This proves $$A$$ and $$A\cup\{q\}$$ have the same cardinality.

