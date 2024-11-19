---
layout: page
title: Practice Exam 3 Solutions
permalink: /exams/practice-exam3-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.
Assume both $$(s_n)$$ and $$(t_n)$$ are sequences of real numbers.

a) If $$f: [0,1]\rightarrow (0,2]$$ is surjective, then it cannot be continuous.

b) If $$f: \mathbb{R}\rightarrow \{x\in\mathbb{R}: x\neq 0\}$$ is surjective, then it cannot be continuous.

c) In Euclidean space $$\mathbb{R}^n$$, every Cauchy sequence converges.

d) A function $$f: [0,1]\rightarrow \mathbb{R}$$ must have an absolute maximum.

e) If $$f: \mathbb{R}\rightarrow\mathbb{R}$$ is a continuous function, then the image $$f((0,1)) = \{f(t): 0 < t < 1\}$$ must be open.

**Solution**:

* True (continuous image of compact is compact)
* True (continuous image of connected is connected)
* True (proved using Bolzano-Weierstrass)
* False (needs continuity)
* False (continuous image of open doesn't ahve to be open, think constant function)

## Problem 2

a) Let $$(S,d_S)$$ and $$(T,d_T)$$ be metric spaces and $$A\subseteq S$$.  If $$a\in S$$ is accumulation point of $$A$$ and $$f: A\rightarrow T$$ is a function, write the definition of $$\lim_{x\rightarrow a} f(x) = L$$.

b) Let $$f: \mathbb{R}^2\rightarrow\mathbb{R}$$ be the function defined by

$$f(x,y) = \left\lbrace\begin{array}{cc}
(x+y)\sin(1/x)\sin(1/y), &  (x,y)\neq (0,0)\\
0, & (x,y) = (0,0)
\end{array}\right.$$

Does the limit

$$\lim_{(x,y)\rightarrow (0,0)} f(x,y)$$

exist?  Carefully explain.

**Solution**:

a) This means that for all $$\epsilon > 0$$, there exists $$\delta > 0$$ such that for all $$x\in A$$

$$0 < d(x,a) < \delta\ \ \Rightarrow\ \ d(f(x),L) < \epsilon.$$

b) The limit exists and is equal to $$0$$.  To see this, let $$\epsilon > 0$$.
and choose $$\delta = \epsilon/2$$.

Then for

$$0 < d_{\mathbb{R}^2}((x,y),(0,0)) = \sqrt{x^2+y^2} < \delta$$

we have that

$$\lvert f(x,y)-0\rvert = \lvert (x + y)\sin(1/x)\sin(1/y)\rvert  \leq \lvert x + y\rvert$$

and since $$\lvert x\rvert \leq \sqrt{x^2+y^2}$$ and $$\lvert y\rvert \leq \sqrt{x^2+y^2}$$, we see

$$\lvert x + y \rvert \leq \lvert x \rvert + \lvert y\rvert \leq 2\sqrt{x^2+y^2} < 2\delta = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that the limit exists and is equal to $$0$$.

## Problem 3

* (a) Let $$(S,d_S)$$ and $$(T,d_T)$$ be metric spaces and $$f: S\rightarrow T$$.  Write down the definition of $$f$$ being continuous at a point $$a\in S$$.
* (b) Prove that the function $$f: \mathbb{R}\rightarrow\mathbb{R}$$ defined by

$$f(x) = \sqrt{x^2 + 1}$$

is continuous at the point $$x=0$$.

**Solution**:

a) This means that for all $$\epsilon > 0$$ there exists $$\delta > 0$$ such that

$$d(x,a) < \delta\ \ \Rightarrow\ \ d(f(x),f(a)) < \epsilon.$$

b) Let $$\epsilon >0$$.  Choose $$\delta = \sqrt{\epsilon}$$.  Then for $$\lvert x-0\rvert < \delta$$, we have

$$\lvert f(x)-f(0)\rvert = \lvert \sqrt{x^2 + 1}-1\rvert = \sqrt{x^2+1}-1 = \frac{x^2}{\sqrt{x^2+1}+1} < x^2 < \delta^2 = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that $$f$$ is continuous at $$x=0$$.


## Problem 4

* (a) State Rolle's Theorem
* (b) Prove Rolle's Theorem
* (c) State the Mean Value Theorem
* (d) Prove the Mean Value Theorem using Rolle's Theorem

**Solution**:

a) Rolle's Theorem:  Let $$f(x)$$ be a continuous function on $$[a,b]$$ which is differentiable at every point in $$(a,b)$$, and which satisfies $$f(a) =f(b)$$.
Then there exists a $$c\in (a,b)$$ with $$f'(c) = 0$$.

b) Proof: By the Extreme Value Theorem, $$f$$ has a global max and a global min at some points in $$[a,b]$$.
If these occur at the endpoints of the interval, then by the assumption $$f(a)=f(b)$$ the absolute max of $$f$$ must be the same as the absolute min, forcing $$f$$ to be a constant function.  It follows that $$f'(c) = 0$$ for any $$c\in (a,b)$$ that you want.

Otherwise, the global max or global min occurs at some point $$c$$ in $$(a,b)$$.  This is also a local max or local min, so it must be a critical point.
Since $$f$$ is differentiable at $$c$$, it follows that $$f'(c) = 0$$.

c) The Mean Value Theorem: Let $$f(x)$$ be a continuous function on $$[a,b]$$ which is differentiable at every point in $$(a,b)$$.
Then there exists a $$c\in (a,b)$$ with

$$f'(c) = \frac{f(b)-f(a)}{b-a}.$$

d) Proof: We apply Rolle's Theorem to the function

$$g(x) = f(x) - \frac{f(b)-f(a)}{b-a}(x-a) - f(a).$$

This function satisfies $$g(b) = 0$$ and $$g(a) = 0$$, is continuous on $$[a,b]$$, and is differentiable on $$(a,b)$$.
Therefore by Rolle's Theorem, there's a point $$c\in (a,b)$$ with $$g'(c) =0$$ ie. 

$$0 = g'(c) = f'(c) - \frac{f(b)-f(a)}{b-a}.$$

Hence

$$f'(c) = \frac{f(b)-f(a)}{b-a}.$$

## Problem 5

* (a) Let $$f$$ and $$\alpha$$ be a real-valued function on an interval $$[a,b]$$.  Write down the definition of the Riemann integral of $$f$$ on $$[a,b]$$ with respect to $$\alpha$$.
* (b) Give an example of an $$f$$ and $$\alpha$$ where $$\int_a^b f d\alpha$$ does not exist
* (c) Prove directly from the definition that $$\int_a^b 1 d\alpha = \alpha(b)-\alpha(a)$$.

**Solution**:

a) The Riemann integral of $$f$$ with respect to $$\alpha$$ is a real number $$A=\int_a^b fd\alpha$$ with the property that for all $$\epsilon > 0$$ there exists a partition $$P_\epsilon$$ of $$[a,b]$$ such that for any refinement $$P$$ of $$P_\epsilon$$

$$\lvert S(P,f,\alpha,\{t_k\}) - A\rvert < \epsilon$$

for all choices of sample points $$\{t_k\}$$ of $$P$$.
Here $$S(P,f,\alpha,\{t_k\})$$ is the Riemann-Stieltjes sum

$$S(P,f,\alpha,\{t_k\}) = \sum_{k=1}^n f(t_k) \Delta\alpha_k(P)$$

b) For example $$f(x) = 1/x$$ and $$\alpha(x) = x$$ on $$[0,1]$$.

c) Define $$f(x) = 1$$.  Let $$\epsilon>0$$ and choose the partition $$P_\epsilon = \{a,b\}$$.
Then for any refinement $$P = \{x_0=a,x_1,\dots, x_n=b\}$$ of $$P_\epsilon$$, we have that

$$S(P,f,\alpha,\{t_k\}) = \sum_{k=1}^n f(t_k) \Delta \alpha_k(P) = \sum_{k=1}^n 1\cdot (\alpha(x_k)-\alpha(x_{k-1})).$$

The latter sum telescoping and adds to $$\alpha(x_n)-\alpha(x_0) = \alpha(b)-\alpha(a)$$.
Therefore 

$$S(P,f,\alpha,\{t_k\})  = \alpha(b)-\alpha(a)$$

It follows that

$$\lvert S(P,f,\alpha,\{t_k\})-(\alpha(b)-\alpha(a))\rvert = 0 < \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that $$\int_a^b 1 d\alpha = \alpha(b)-\alpha(a)$$.

## Problem 6

* (a) Let $$f$$ be a real-valued function on $$(a,b)$$.  Write down what it means for $$f$$ to be differentiable at $$c\in (a,b)$$.
* (b) Write down the Quotient Rule for derivatives.  Make sure to carefully state the required assumptions!
* (c) Prove the quotient rule for derivatives.  You may use the Helper Theorem!

**Solution**:

a) We say $$f$$ is differentiable at $$c$$ if the limit $$\lim_{x\rightarrow a} \frac{f(x)-f(a)}{x-a}$$ exists

b) The Quotient Rule says that if $$f$$ and $$g$$ are differentiable at $$x=a$$ and $$g(a)\neq 0$$, then $$h=f/g$$ satisfies

$$h'(a) = \frac{f'(a)g(a)-f(a)g'(a)}{g(a)^2}.$$

c) By the Helper Theorem, there exist functions $$f^*$$ and $$g^*$$ which are continuous on $$(a,b)$$, and which satisfy

$$f(x)-f(a) = (x-a)f^*(x),\ \ g(x)-g(a) = (x-a)g^*(x)$$

and moreover $$f^*(a) = f'(a)$$ and $$g^*(a) = g'(a)$$.  Therefore

$$\begin{align}
h(x)-h(a)
  & = \frac{f(x)}{g(x)}-\frac{f(a)}{g(a)}}\\
  & = \frac{f(x)g(a)-f(a)g(x)}{g(x)g(a)}\\
  & = \frac{f(x)g(a)-f(x)g(x)+f(x)g(x)-f(a)g(x)}{g(x)g(a)}\\
  & = \frac{-f(x)(g(x)-g(a))+(f(x)-f(a))g(x)}{g(x)g(a)}\\
  & = (x-a)\frac{-f(x)g^*(x)+f^*(x)g(x)}{g(x)g(a)}.
\end{align}$$

The function

$$h^*(x) = \frac{-f(x)g^*(x)+f^*(x)g(x)}{g(x)g(a)}$$

Since $$f$$ and $$g$$ are differentiable at $$x=a$$, they are both continuous at $$x=a$$.
The functions $$f^*$$ and $$g^*$$ are continuous at $$x=a$$, and sums and products of continuous functions are continuous.
Therefore the numerator and denominator of $$h^*$$ are continuous.
The denominator is nonzero at $$x=a$$, so $$h^*$$ itself is continuous at $$x=a$$.
Thus by the Helper Theorem, $$h(x)$$ is differentiable at $$x=a$$ and

$$h'(a) = h^*(a) = \frac{-f(a)g^*(a)+f^*(a)g(a)}{g(a)g(a)} = \frac{-f(a)g'(a)+f'(a)g(a)}{g(a)^2}.$$

## Problem 7

Let $$S=\mathbb{R}$$ and $$d_S: S\times S\rightarrow S$$ be the discrete metric on $$S$$, and let $$T=\mathbb{R}$$ with $$d_T: T\times T\rightarrow T$$ the Euclidean metric.

* (a) Prove that every subset of $$S$$ is open.
* (b) Prove that *any* function $$f: S\rightarrow T$$ is continuous.

**Solution**:

a) Let $$A\subseteq S$$ be any subset.  Then for $$a\in A$$, the ball $$B_S(a,1) = \{a\}\subseteq A$$, making $$a$$ an interior point of $$A$$.  It follows that every point in $$A$$ an interior point of $$A$$, making $$A$$ an open set.  Thus every subset is open.

b) A function is continuous if and only if the preimage of every open set is open.  Let $$U\subseteq T$$ be open.  Then since every subset of $$S$$ is open, the preimage $$f^{-1}(U)\subsetq S$$ is open.  Hence $$f$$ is continuous.

## Problem 8

Let $$S=\mathbb{R}$$ and $$d_S: S\times S\rightarrow S$$ be the discrete metric on $$S$$, and let $$T=\mathbb{R}$$ with $$d_T: T\times T\rightarrow T$$ the Euclidean metric.

* (a) Write down the definition of a set being connected.
* (b) Prove that the only connected subsets of $$S$$ are singleton sets.
* (c) Prove that a function $$g: T\rightarrow S$$ will be continuous if and only if it is constant.

a) A metric space $$(S,d_S)$$ is connected if it is not disconnected, ie. if it cannot be written as the union of two nonempty, disjoint, open sets.  A subset of a metric space is connected if the associated subspace is a connected metric space.

b) Suppose that $$A\subseteq S$$.  If $$A$$ has more than one point, then for $$a\in A$$ the sets $$U=\{a\}$$ and $$V = A\backslash U$$ are nonempty, disjoint, and their union is $$A$$.  Moreover, both $$U$$ and $$V$$ are open in the subspace $$A$$ of $$S$$ (since every set is open).  Thus $$A$$ is disconnected.  It follows that the connected sets are singletons.

c) The continuous image of a connected set is connected.  We proved in class that the real line with the Euclidean metric is connected.  Thus $$g(T)$$ is connected, and from part (b), it follows that it is a singleton set, ie. $$g(T) = \{a\}$$ for some $$a\in S$$.  Hence $$g(x) = a$$ for all $$x$$, meaning $$g$$ is constant.




