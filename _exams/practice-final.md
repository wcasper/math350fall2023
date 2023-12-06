---
layout: page
title: Practice Final Exam 
permalink: /exams/practice-final
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.

* (a) If $$f(x)$$ is Darboux integrable on $$[a,b]$$, then it is also Riemann integrable on $$[a,b]$$.
* (b) If $$\lim s_n=0$$, and $$f(x)$$ is continuous everywhere then $$\lim f(s_n) = 0$$
* (c) Every sequence has a convergent subsequence
* (d) If $$f(x)$$ is integrable on $$[a,b]$$, then it must be continuous on $$[a,b]$$
* (e) If $$f(x)$$ differentiable on $$\mathbb{R}$$, then $$f'(x)$$ is continuous on $$\mahbb{R}$$

## Problem 2

Give an example of each of the following, or explain why it doesn't exist.

* (a) A function which is not integrable.
* (b) A nonconstant differentiable function $$f(x)$$ with $$f'(x) = 0$$ for all $$x$$.
* (c) A continuous function $$f(x)$$ on $$\mathbb{R}$$ with $$\{f(x) : 0\leq x < 1\} = \{-5,7\}.$$
* (d) A bounded set of real numbers with no maximum value.
* (e) A sequence of differentiable functions which converge uniformly to $$f(x) = \lvert x\rvert$$

## Problem 3

The following problem was famously considered by Euler, so blame him.

Let $$p_1=2$$, $$p_2=3$$, $$p_3=5$$, $$p_4=7$$, $$p_5=11$$ be the sequence of all prime numbers in increasing order.  Determine the convergence or divergence of each of the following series.  Carefully justify your work

* (a) $$\sum_{n=0}^\infty \frac{(-1)}{p_n}$$
* (b) $$\sum_{n=0}^\infty \frac{1}{p_n^2}$$
* (c) $$\sum_{n=0}^\infty \frac{1}{p_n}$$.  You may assume without proof the bounds

$$n\log(n) - \frac{3}{2} < p_n < 2n\log(n).$$

## Problem 4

* (a) Write down the definition of a function $$f(x)$$ being continuous at a point $$a\in\text{Dom}(f)$$.
* (b) Prove that the function

$$f(x) = \left\lbrace{\begin{array}{cc}x\sin(1/x), & x\neq 0\\0, & x=0\end{array}\right.$$

is continuous at $$x=0$$.
* (c) Prove that the function

$$g(x) = \left\lbrace{\begin{array}{cc}\sin(1/x), & x\neq 0\\0, & x=0\end{array}\right.$$

is not continuous at $$x=0$$.

## Problem 5

* (a) Write down the definition of $$f(x)$$ being differentiable at $$x=a$$.
* (b) Prove using only basic definitions and algebra that $$f(x) = x^3$$ is differentiable a $$x=8$$.
* (c) Carefully prove that $$g(x) = \lvert x\rvert$$ is NOT differentiable at $$x=0$$.

## Problem 6

* (a) State the Mean Value Theorem
* (b) State the Intermediate Value Theorem
* (c) Prove that the polynomial 
$$f(x) = x^{2023} + x^15 + 3x^5 + 2x - 6$$
has exactly one real root, and that this root must lie in the interval $$(0,1)$$.

## Problem 7

Let $$f(x)$$ be a bounded function on the interval $$[a,b]$$.

* (a) Write the definition of the lower Darboux sum $$L(f,P)$$ of $$f(x)$$ on a partition $$P = \{a_0,\dots, a_n\}$$ on $$[a,b]$$
* (b) Write the definition of the upper Darboux sum $$U(f)$$ of $$f(x)$$ on $$[a,b]$$
* (c) Prove that $$L(f,P)\leq U(f,P)$$ for any partition $$P$$ of $$[a,b]$$
* (d) Prove that if $$P$$ and $$P'$$ are any two partitions of $$[a,b]$$ then, $$L(f,P)\leq U(f,P')$$.  You can use the fact that if $$P$$ and $$Q$$ are partitions and $$P\subseteq Q$$, then $$L(f,P)\leq L(f,Q)$$ and $$U(f,Q)\leq U(f,P)$$.
* (c) Prove that $$L(f)\leq U(f)$$.  




