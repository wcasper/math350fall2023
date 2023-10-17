---
layout: page
title: Practice Exam 2 Solutions
permalink: /exams/practice-exam2-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.

a) if $$(s_n)$$ and $$(t_n)$$ are bounded sequences, then $$\limsup(s_n+t_n) = (\limsup s_n) + (\limsup t_n)$$

FALSE

b) every sequence has a monotone increasing subsequence

FALSE

c) there exists a sequence $$(s_n)$$ with the property that every irrational number appears in the sequence at least once

FALSE

d) every bounded sequence has a monotone convergent subsequence

TRUE

e) if $$\sum a_n$$ is a convergent series with $$a_n \geq 0$$ for all $$n$$, then $$\sum a_n$$ is absolutely convergent

TRUE

## Problem 2

a) Write the definition of a function $$f(x)$$ being continuous at a point $$a\in\mathbb{R}$$

For all $$\epsilon > 0$$ there exists $$\delta > 0$$ such that for every $$x\in\text{Dom}(f)$$ we have

$$\lvert x-a\rvert < \delta\quad\Rightarrow\quad\lvert f(x)-f(a)\rvert < \epsilon.$$

b) Carefully state the Ratio Test

Suppose that $$\sum a_n$$ is a series of nonzero terms and let $$\alpha = \liminf \lvert \frac{a_{n+1}}{a_n}\rvert$$ and $$\beta = \limsup \lvert \frac{a_{n+1}}{a_n}\rvert$$.  If $$\beta < 1$$ then the series converges absolutely.  If $$\alpha > 1$$ then the series diverges.  Otherwise the test is inconclusive.

c) Write the definition of $$(t_n)$$ being a subsequence of $$(s_n)$$

There exists a sequence of positive integers $$(n_k)$$ with $$n_k < n_{k+1}$$ for all $$k\in\mathbb{N}$$ such that $$t_k = s_{n_k}$$ for all $$k\in\mathbb{N}$$

## Problem 3

Without using any theorems about series, do the following.

* (a) State the Cauchy Criterion for series

The Cauchy Criterion for a series $$\sum a_k$$ says that the sequence of partial sums is a Cauchy sequence.  Equivalently, it says that for all $$\epsilon > 0$$ there exists $$N$$ such that for all $$n > m > N$$ we have $$\left\lvert \sum_{k=m}^n a_k \right\rvert < \epsilon.$$

* (b) Prove that if $$\sum_{n=1}^\infty b_n$$ is absolutely convergent, then it is convergent.

Suppose that $$\sum_{n=1}^\infty b_n$$ is absolutely convergent.
Then $$\sum_{n=1}^\infty \lvert b_n\rvert $$ is convergent.
Therefore it satisfies the Cauchy Criterion that for all $$\epsilon > 0$$ there exists $$N$$ such that for all $$n > m > N$$ we have $$\left\lvert \sum_{k=m}^n \lvert b_k\rvert \right\rvert < \epsilon.$$

Therefore by the triangle inequality

$$\left\lvert \sum_{k=m}^n \lvert b_k\rvert \right\rvert \leq \sum_{k=m}^n \lvert b_k\rvert < \epsilon.$$

Thus $$\sum b_k$$ satisfies the Cauchy Criterion and must converge.

* (c) Prove that if $$\lvert b_n\rvert\leq a_n$$ for all $$n$$ and $$\sum_{n=1}^\infty a_n$$ converges, then $$\sum_{n=1}^\infty b_n$$ is absolutely convergent.

Since $$\lvert b_n\rvert\leq a_n$$ for all $$n$$, and $$\sum_{n=1}^\infty a_n$$ converges, the Comparison Test implies that $$\sum_{n=1}^\infty \lvert b_n\rvert converges.
Hence $$\sum_{n=1}^\infty b_n$$ is absolutely convergent.


## Problem 4

Let $$(a_n)$$ be a bounded sequence of real numbers.  Prove that

$$\limsup e^{a_n} = e^{\limsup a_n}.$$

Note that $$e^x$$ is monotone increasing, so it preserves inequalities!

Now let $$M_N = \sup\{a_n: n\geq N\}$$ and $$K_N = \sup\{e^{a_n}: n\geq N\}.$$
We know that $$M_N \geq a_n$$ for all $$n\geq N$$ and therefore e^{M_N}\geq e^{a_n}$$ for all $$n\geq N$$.  Hence $$e^{M_N}$$ is an upper bound for $$\{e^{a_n}: n\geq N\}$$ and must be greater than the least upper bound, ie. $$K_N\leq e^{M_N}.$$

Additionally $$\ln(x)$$ is a monotone increasing function, so it preserves inequalities!
We know that $$e^{a_n}\leq K_N$$ for all $$n\geq N$$ and therefore $$a_n\leq \ln(K_N)$$ for all $$n\geq N$$.
Therefore $$\ln(K_N)$$ is an upper bound of $$\{a_n: n\geq N\}$$ and must be greater than the least upper bound $$M_N$$, ie. $$M_N\leq \ln(K_N)$$.
Exponentiating, this gives $$e^{M_N}\leq K_N$$.
Putting this together with the previous paragraph, we have $$e^{M_N} = K_N.$$

Then taking the limit and using the fact that $$e^x$$ is continuous, we find

$$\limsup e^{a_n} = \lim K_N = \lim e^{M_N} = e^{\lim M_N} = e^{\limsup a_n}.$$


## Problem 5

For each of the following series, determine if it diverges, converges, or converges absolutely.
Carefully justify your answer.

* $$\sum_{n=1}^\infty \frac{\cos((2n+1)\pi)}{n}$$

This is the same as the series $$\sum_{n=1}^\infty \frac{-1}{n}$$ which is a divergent harmonic series.

* $$\sum_{n=2}^\infty \frac{1}{(\ln(n))^n}$$

This converges by the Root Test.

* $$\sum_{n=3}^\infty \frac{n^2-\sqrt{n}}{4-n^2}$$

This diverges by the Test for Divergence.

* $$\sum_{n=0}^\infty (-1)^n\frac{3^n}{2^{n+2}}$$

This diverges by the Test for Divergence.

* $$\sum_{n=1}^\infty \frac{n}{e^n}$$

This converges by the Ratio Test.

## Problem 6

Let $$\mathbb{I}$$ be the set of all irrational numbers in the interval $$[0,1]$$.
Consider the function

$$f: I\rightarrow [0,1]$$

defined via decimal expansions by

$$f(0.d_1d_2d_3d_4d_5d_6\dots) = 0.d_1d_3d_5d_7\dots$$

* (a) Prove that this function is well defined.

Since irrational numbers have unique decimal expansions, the function is well defined.

* (b) Prove that $$f(x)$$ is surjective.

Let $$\pi = 3.p_1p_2p_3p_4\dots$$ .  Since $$\pi$$ is irrational, the digits $$(p_j)$$ never start repeating.

Now let $$0.d_1d_2d_3\dots$$ be a decimal expansion of any number in $$[0,1]$$.

Then $$x = 0.d_1p_1d_2p_2d_3p_3\dots$$ is irrational because the digits don't repeat and

$$f(x) = 0.d_1d_2d_3d_4\dots$$

This proves that $$f$$ is surjective.

* (c) If we replace $$I$$ with the interval $$[0,1]$$ above, is it still well-defined? Carefully explain.

Unfortunately, we have $$1 = 1.00000000\dots$$ and $$1 = 0.99999999\dots$$, so the above rule sends $$1$$ to both $$0$$ and $$1$$.
Therefore the function is not well-defined.

## Problem 7

Consider the function

$$f(x) = \left\lbrace\begin{array}{cc}\sin(1/x), & x\neq 0\\0 & x=0\end{array}\right.$$

* Prove that $$f(x)$$ is continuous at every point $$a\in\mathbb R$$ with $$a\neq 0$$

The rational function $$g(x)=1/x$$ is continuous at every point in its domain (ie. where $$x\neq 0$$) and $$\sin(x)$$ is continuous at every point.  So the composition of functions $$f(x) = \sin(g(x))$$ is continuous at every point different from $$0$$.

* Prove that $$f(x)$$ is not continuous at $$x=0$$.

Consider the sequence $$a_n = \frac{1}{2\pi n + \pi/2}$$.  We have $$f(a_n) = 1$$ for all $$n$$ and therefore

$$\lim f(a_n) = \lim 1 = 1\neq f(0).$$

Thus $$f(x)$$ is not continuous at $$x=0$$.





