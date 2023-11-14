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

* (a) If $$R>0$$ then the radius of convergence of $$\sum_{k=0}^\infty \frac{x^k}{R^k}$$ is $$R$$

TRUE

* (b) There exists a function $$f(x)$$ which is discontinuous at every rational number and continuous at every irrational number

TRUE

* (c) If $$f(x)$$ is continuous on an interval, then $$f(x)$$ must be uniformly continuous on that interval

FALSE

* (d) The function $$f(x) = 1/x$$ is continuous everywhere in its domain

TRUE

* (e) If $$\lim_{x\rightarrow a+} f(x)$$ and $$\lim_{x\rightarrow a-}f(x)$$ exist, then $$\lim_{x\rightarrow a}f(x)$$ exists

FALSE

## Problem 2

Give an example of each of the following, or explain why it doesn't exist.

* (a) A function which is uniformly continuous on $$\mathbb{R}$$

The constant function $$f(x) = 1$$

* (b) A function which is continuous on $$(0,1)$$ but not uniformly continuous on $$(0,1)$$

The function $$f(x) = 1/x$$.

* (c) A power series whose radius of convergence is $$R=0$$

The series $$\sum_{n=0}^\infty n!x^n$$

* (d) A function which is differentiable at $$x=0$$ but not continuous at $$x=0$$

This doesn't exist because differentiability implies continuity.

* (e) A function whose domain is $$\mathbb{R}$$, which is discontinuous at every point in $$\mathbb{R}$$ 

The function

$$f(x) = \left\lbrace\begin{array}{cc}1 & x \in \mathbb{Q}\\ 0 & x\notin\mathbb Q\end{array}\right.$$

## Problem 3

* (a) State the definition of the radius of convergence of a power series $$\sum_{n=0}^\infty a_nx^n$$.

The radius of convergence is 

$$R = \left\lbrace\begin{array}{cc}0, & \beta = \infty\\ \infty, & \beta = 0\\ 1/\beta, & \text{otherwise}\end{array}\right.$$

where here $$\beta = \limsup \sqrt[n]{a_n}$$.

* (b) Suppose that $$\sum_{n=0}^\infty \lvert a_n\rvert < \infty$$. Prove that the radius of convergence of $$\sum_{n=0}^\infty a_nx^n$$ is at least $$R=1$$.

If $$\beta = \limsup \sqrt[n]{\lvert a_n\rvert } > 1$$ then $$\sum_{n=0}^\infty \lvert a_n\rvert$$ diverges.  Since it converges, we must have $$\beta\leq 1$$.  Therefore $$R\geq 1$$.

* (c) Under the assumption of (b), prove that the sequence of polynomials $$f_N(x) = \sum_{n=0}^N a_nx^n$$ converges uniformly on $$[-1,1]$$.

It suffices to show that $$(f_N(x))$$ is uniformly Cauchy on $$[-1,1]$$.

Since $$\sum_{n=0}^\infty \lvert a_k\rvert$$ converges, it satisfies the Cauchy criterion.  In other words, for all $$\epsilon > 0$$ there exists an $$n$$ such that $$n\geq m > N$$ implies that $$\sum_{k=m}^n \lvert a_k\rvert < \epsilon.$$

Suppose $$\lvert x\rvert \leq 1$$.  
Then for $$n>m > N$$ we calculate

$$\begin{align*}
\lvert f_n(x)- f_m(x)\rvert
  & = \left\lvert\sum_{k=m}^n a_kx^k\right\rvert\\
  & \leq \sum_{k=m}^n\lvert a_k\rvert \lvert x\rvert^k\\
  & \leq \sum_{k=m}^n\lvert a_k < \epsilon.
\end{align*}$$

Since this is independent of $$x$$ and $$\epsilon  >0$$ was arbitrary, this proves that $$(f_N(x))$$ is uniformly Cauchy on $$[-1,1]$$.


## Problem 4

* (a) Write down the definition of a function $$f(x)$$ being continuous at a point $$a\in\text{Dom}(f)$$.

A function $$f(x)$$ is continuous at $$x=a$$ if for all $$\epsilon > 0$$ there exists a $$\delta > 0$$ such that $$\lvert x-a\rvert < \delta$$ implies $$\lvert f(x)-f(a)\rvert < \epsilon$$.


* (b) Suppose that $$f(x)$$ is continuous at every point in $$(-1,1)$$ and that for every $$x\in (-1,1)$$ we have $$f(x^2) = f(x)$$.  Prove that $$f(x)$$ is a constant function on $$(-1,1)$$.

Suppose that $$x\in (-1,1)$$.  An inductive arguement proves that $$f(x) = f(x^{2^n})$$ for all $$n$$.  Moreover $$\lim x^{2^n} = 0$$.  Since $$f(x)$$ is continuous, it follows that $$\lim f(x^{2^n}) = f(0)$$.  Thus

$$f(x) = \lim f(x) = \lim f(x^{2^n}) = f(0).$$

In particular $$f(x) = f(0)$$ for all $$x$$, and we conclude that $$f(x)$$ is continuous.

## Problem 5

Consider the function

$$f(x) = \left\lbrace\begin{array}{cc} -1 & x < 0\\x-1 & x > 0\\ 0 & x=0\end{array}\right.$$

* (a) Write down the $$\epsilon,\delta$$ definition of the limit as $$x$$ approaches $$a$$ along $$S$$ of $$f(x)$$

The limit as $$x$$ approaches $$a$$ in $$S$$ of $$f(x)$$ is equal to $$L$$ means that for all $$\epsilon > 0$$ there exists a $$\delta > 0$$ such that

$$\lvert x-a\rvert < \delta \ \ \Rightarrow\ \ \lvert f(x)-L\rvert < \epsilon,\ \ \text{for all}\ x\in S.$$

* (b) If $$S=(-1,1)\backslash\{0\}$$, carefully show that the limit as $$x$$ approaches $$a$$ along $$S$$ of $$f(x)$$ exists and explain what it is

We claim that the limit is $$-1$$.
To see this, let $$\epsilon > 0$$.
Choose $$\delta=\epsilon$$.
Suppose $$0 < \lvert x-0\rvert < \delta$$.
If $$x < 0$$, then $$f(x)=-1$$ and therefore $$\lvert f(x)-(-1)\rvert = 0 < \epsilon.$$
If $$x > 0$$, then $$f(x)=x-1$$ and therefore $$\lvert f(x)-(-1)\rvert = \lvert x\rvert < \delta = \epsilon.$$
Thus in either case $$\lvert f(x)-(-1)\rvert < \epsilon$$.
Since $$\epsilon > 0$$ was arbitrary, this proves that the limit is $$-1$$.

* (c) If $$S=(-1,1)$$, carefully explain why the limit as $$x$$ approaches $$a$$ along $$S$$ does not exist

For $$\lim_{x\rightarrow 0} f(x) = L$$ to be true, we must have that for every sequence $$x_n$$ of values in $$S$$ converging to $$0$$, the limit $$\lim f(x_n)$$ converges to $$L$$.
If we take $$x_n = -1/(n+1)$$, then $$f(x_n) = -1$$ for all $$n$$ so $$\lim f(x_n) = -1$$.
However, if we take $$x_n = 0$$ for all $$n$$, then $$f(x_n) = 0$$ for all $$n$$, so $$\lim f(x_n) = 0$$.
Thus the limit does not exist.

* (d) Is $$f(x)$$ continuous at $$x=0$$?  Explain.

If $$f(x)$$ is continuous at $$x=0$$, then the limit as $$x\rightarrow 0$$ of $$f(x)$$ would exist and be equal to $$f(0)$$.
However, from (b) $$\lim_{x\rightarrow 0} f(x)=-1\neq f(0)$$.

## Problem 6

Consider the sequence of functions

$$f_n(x) = \frac{nx}{1 + n^2x}.$$

* (a) Write down the definition of a sequence of functions $$(f_n(x))$$ converging uniformly to $$f(x)$$ on $$S$$.

For all $$\epsilon > 0$$ there exists an $$N$$ such that $$n > N$$ implies $$\lvert f_n(x)-f(x)\rvert < \epsilon$$ for all $$x\in S$$.

* (b) Show that the sequence of functions $$f_n(x)$$ converges uniformly to the constant function $$f(x) = 0$$ on $$S=[0,1]$$

Notice that $$0 \leq f_n(x) \leq \frac{n}{1+n^2} \leq \frac{1}{n}$$ for all $$x\in [0,1]$$.

Let $$\epsilon > 0$$.  Choose $$N=1/\epsilon$$.  Then for $$n>N$$ and for all $$x\in [0,1]$$  we have

$$\lvert f_n(x)-0\rvert \leq \frac{n}{1+n^2}\leq \frac{1}{n} < \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves $$(f_n(x))$$ converges uniformly to $$f(x)$$ on $$[0,1]$$.

## Problem 7

Suppose that $$(f_n(x))$$ is a sequence of continuous functions on $$[0,1]$$ with the property that

$$\lvert f_{n+1}(x)- f_n(x)\rvert < \frac{1}{2}\lvert f_{n}(x)- f_{n-1}(x)\rvert$$

for all integers $$n>1$$ and all $$x\in [0,1]$$.

 * (a) Write down the definition of a sequence of functions being uniformly Cauchy

For all $$\epsilon > 0$$, there exists an $$N$$ such that $$m,n > N$$ implies that 

$$\lvert f_m(x)-f_n(x)\rvert < \epsilon\ \ \text{for all}\ \ x\in [0,1].$$

 * (b) Prove that the functions $$f_n(x)$$ converge to a continuous function $$f(x)$$ on $$[0,1]$$.

Using an inductive argument, we can prove that for $$n > m > 0$$

$$\lvert f_{n}(x)- f_m(x)\rvert < \frac{1}{2^{m-1}}\lvert f_{n-m+1}(x)- f_{1}(x)\rvert$$

Also, for any $$k>1$$ the triangle inequality says

$$\lvert f_k(x)-f_1(k)\rvert \leq \sum_{j=2}^k \lvert f_j(x)-f_{j-1}(x)\rvert \leq \sum_{j=2}^k \frac{1}{2^{j-2}}\lvert f_2(x)-f_1(x)\rvert = \left(2-2^{2-k}\right)\lvert f_2(x)-f_1(x)\rvert\leq 2\lvert f_2(x)-f_1(x)\rvert.$$

Consequently, for $$n>m>0$$ we have

$$\lvert f_{n}(x)- f_m(x)\rvert < \frac{1}{2^{m-2}}\lvert f_{2}(x)- f_{1}(x)\rvert.$$

By the Extreme Value Theorem, there exists $$M>0$$ such that $$\lvert f_2(x)-f_1(x)\rvert \leq M$$ for all $$x\in [0,1]$$.
Consequently, $$\lvert f_{n}(x)- f_m(x)\rvert < \frac{M}{2^{m-2}}$$.

Let $$\epsilon > 0$$.  Choose $$N=\log_2(M/\epsilon)+2$$.
Then for $$n>m>N$$ we have

$$\lvert f_{n}(x)- f_m(x)\rvert < \frac{M}{2^{m-2}} = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that $$(f_n(x))$$ satisfies the Cauchy criterion on $$[0,1]$$.
This proves that $$(f_n(x))$$ converges uniformly to some function $$f_n(x)$$ on $$[0,1]$$.
Since each $$f_n(x)$$ is continuous, it follows that $$f(x)$$ is continuous on $$[0,1]$$.


