---
layout: page
title: Practice Final Exam Solutions
permalink: /exams/practice-final-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.

* (a) If $$f(x)$$ is Darboux integrable on $$[a,b]$$, then it is also Riemann integrable on $$[a,b]$$.  TRUE
* (b) If $$\lim s_n=0$$, and $$f(x)$$ is continuous everywhere then $$\lim f(s_n) = 0$$ FALSE
* (c) Every sequence has a convergent subsequence FALSE
* (d) If $$f(x)$$ is integrable on $$[a,b]$$, then it must be continuous on $$[a,b]$$ FALSE
* (e) If $$f(x)$$ differentiable on $$\mathbb{R}$$, then $$f'(x)$$ is continuous on $$\mathbb{R}$$ FALSE

## Problem 2

Give an example of each of the following, or explain why it doesn't exist.

* (a) A function which is not integrable. 

$$f(x) = \left\lbrace\begin{array}{cc}1 & x\in \mathbb Q\\ 0 & x\notin\mathbb{Q}\end{array}\right.$$

* (b) A nonconstant differentiable function $$f(x)$$ with $$f'(x) = 0$$ for all $$x$$.

Cannot exist by the Mean Value Theorem.

* (c) A continuous function $$f(x)$$ on $$\mathbb{R}$$ with $$\{f(x) : 0\leq x < 1\} = \{-5,7\}.$$

The continuous image of an interval must be an interval, so it cannot exist

* (d) A bounded set of real numbers with no maximum value.

$$\{1-\frac{1}{n}: n\in\mathbb{N}\}.$$

* (e) A sequence of differentiable functions which converge uniformly to $$f(x) = \lvert x\rvert$$

$$f_n(x) = \sqrt{x^2+\frac{1}{n}}.$$

## Problem 3

The following problem was famously considered by Euler, so blame him.

Let $$p_1=2$$, $$p_2=3$$, $$p_3=5$$, $$p_4=7$$, $$p_5=11$$, and so on be the sequence of all prime numbers in increasing order.  Determine the convergence or divergence of each of the following series.  Carefully justify your work

* (a) $$\sum_{n=0}^\infty \frac{(-1)}{p_n}$$

Since $$p_n$$ goes to $$\infty$$, $$\lim\frac{1}{p_n}$$ goes to $$0$$ and is monotone decreasing.  Therefore the Alternating Series Test tells us that this series converges.

* (b) $$\sum_{n=0}^\infty \frac{1}{p_n^2}$$

Note that $$p_n > n$$ for all $$n$$ and therefore $$\frac{1}{p_n^2} \leq \frac{1}{n^2}$$.  Since $$\sum_{n=1}^\infty \frac{1}{n^2}$$ converges ($$p$$-series), it follows that the original series also converges by the Comparison Test

* (c) $$\sum_{n=0}^\infty \frac{1}{p_n}$$.  You may assume without proof the bounds

$$n\log(n) - \frac{3}{2} < p_n < 2n\log(n).$$

We have that $$p_n < 2n\log(n)$$ and therefore $$\frac{1}{p_n} > \frac{1}{2n\log(n)}$$.
The series $$\sum\frac{1}{2n\log(n)}$$ diverges, for example by the integral test.
Therefore $$\sum_{n=1}^\infty \frac{1}{p_n}$$ diverges by the Comparison Test.

## Problem 4

* (a) Write down the definition of a function $$f(x)$$ being continuous at a point $$a\in\text{Dom}(f)$$.

For all $$\epsilon > 0$$ there exists $$\delta > 0$$ such that $$\lvert x-a\rvert < \delta$$ implies $$\lvert f(x)-f(a) \rvert < \epsilon$$ for all $$x\in\text{Dom}(f)$$.

* (b) Prove that the function

$$f(x) = \left\lbrace\begin{array}{cc}x\sin(1/x), & x\neq 0\\0, & x=0\end{array}\right.$$

is continuous at $$x=0$$.

Let $$\epsilon > 0$$.  Choose $$\delta = \epsilon$$.
Then for $$\lvert x - 0\rvert < \delta$$, we can consider two cases:

- Case 1: $$x=0$$.  In this case $$\lvert f(x)-f(0)\rvert = \lvert f(0)-f(0)\rvert =0$$.
- Case 2: $$x\neq 0$$.  In this case $$\lvert \sin(1/x)\rvert \leq 1$$ and therefore

$$\lvert f(x)-f(0)\rvert = \lvert x\sin(1/x)-0\rvert \leq \lvert x\rvert = \lvert x-0\rvert < \delta = \epsilon.$$

Thus in either case, $$\lvert f(x)-f(0)\rvert < \epsilon$$.  Since $$\epsilon > 0$$ was arbitrary, this proves that $$f(x)$$ is continuous at $$x=0$$.

* (c) Prove that the function

$$g(x) = \left\lbrace\begin{array}{cc}\sin(1/x), & x\neq 0\\0, & x=0\end{array}\right.$$

is not continuous at $$x=0$$.

Recall that $$f(x)$$ is continuous at $$a$$ if and only if for **every** sequence $$(s_n)$$ of values in $$\text{Dom}(f)$$ converging to $$a$$, we have $$\lim f(s_n)=f(a)$$.
Consider the sequence $$s_n = \frac{2}{(4n+1)\pi}$$.  Then $$\lim s_n = 0$$ but $$f(s_n) = 1$$ for all $$n$$ and therefore $$\lim f(s_n) = 1\neq f(0)$$.

## Problem 5

* (a) Write down the definition of $$f(x)$$ being differentiable at $$x=a$$.

This means that the limit $$\lim_{x\rightarrow a}\frac{f(x)-f(a)}{x-a}$$ exists.

* (b) Prove using only basic definitions and algebra that $$f(x) = x^3$$ is differentiable a $$x=8$$.

Let $$\epsilon > 0$$.  Choose $$\delta = $$

Then we calculate

$$\lim_{x\rightarrow 8}\frac{f(x)-f(8)}{x-8} = \lim_{x\rightarrow 8}\frac{x^3-8^3}{x-8} = \lim_{x\rightarrow 8}\frac{(x-8)(x^2+8x+8^2)}{x-8}$$.

Since the limit as we approach $$x=8$$ never considers the value of our expression *at* the point $$x=8$$ itself, this simplifies to $$\lim_{x\rightarrow 8}(x^2+8x+8^2)$$.
Then since polynomials are continuous everywhere, we can simply evaluate this at $$x=8$$, getting

$$\lim_{x\rightarrow 8}\frac{f(x)-f(8)}{x-8} = 3\cdot 8^2.$$

In particular the limit exists and the function is differentiable at $$x=8$$.

* (c) Carefully prove that $$g(x) = \lvert x\rvert$$ is NOT differentiable at $$x=0$$.

For $$x>0$$, we have $$g(x)=x$$, from which we calculate

$$\lim_{x\rightarrow 0+}\frac{g(x)-g(0)}{x-0} = \lim_{x\rightarrow 0+} \frac{x-0}{x-0} = \lim_{x\rightarrow 0+}1 = 1.$$


For $$x<0$$, we have $$g(x)=-x$$, from which we calculate

$$\lim_{x\rightarrow 0-}\frac{g(x)-g(0)}{x-0} = \lim_{x\rightarrow 0-} \frac{-x-0}{x-0} = \lim_{x\rightarrow 0-}-1 = -1.$$

Since the left and right limits exist but aren't equal, we conclude that the limit $$\lim_{x\rightarrow 0}\frac{g(x)-g(0)}{x-0}$$ does not exist.

## Problem 6

* (a) State the Mean Value Theorem

Let $$f(x)$$ be a function which is continuous on $$[a,b]$$ and differentiable on $$(a,b)$$.  Then there exists a value $$c\in (a,b)$$ with

$$f'(c) = \frac{f(b)-f(a)}{b-a}.$$

* (b) State the Intermediate Value Theorem

Let $$f(x)$$ be a function which is continuous on $$[a,b]$$.  Then for every value of $$y$$ strictly between $$f(a)$$ and $$f(b)$$, there exists a value $$c\in (a,b)$$ with $$f(c)=y$$.

* (c) Prove that the polynomial 
$$f(x) = x^{2023} + x^{15} + 3x^5 + 2x - 6$$
has exactly one real root, and that this root must lie in the interval $$(0,1)$$.

Note that polynomials are continuous and differentiable everywhere, so they satisfy the assumptions of both IVT and MVT.
Now $$f(0) = -6$$ and $$f(1) = 1$$.
Therefore IVT says that there will be some value $$c\in (0,1)$$ satisfying $$f(c) = 0$$.  In particular $$f(x)$$ has at least one real root, and it lies inside the expected interval.

Now suppose that $$f(x)$$ has another real root at some value $$d\in\mathbb{R}$$.
Then $$f(d) = 0 = f(c)$$, so by Rolle's Theorem (or MVT), there exists a point $$x$$ between $$c$$ and $$d$$ with $$f'(x) = 0$$.
However,

$$f'(x) = 2023x^{2022} + 15x^{14} + 15x^4 + 2 > 0,$$

so this is impossible.  Therefore $$f(x)$$ can have only one real root.


## Problem 7

Let $$f(x)$$ be a bounded function on the interval $$[a,b]$$.

* (a) Write the definition of the lower Darboux sum $$L(f,P)$$ of $$f(x)$$ on a partition $$P = \{a_0,\dots, a_n\}$$ on $$[a,b]$$

$$L(f,P) = \sum_{k=1}^n (a_k-a_{k-1})\inf\{f(x): a_{k-1}\leq x\leq a_k\}.$$

* (b) Write the definition of the upper Darboux integral $$U(f)$$ of $$f(x)$$ on $$[a,b]$$

$$U(f) = \inf\{ U(f,P): P\ \text{is a partition of}\ [a,b]\}.$$

* (c) Prove that $$L(f,P)\leq U(f,P)$$ for any partition $$P$$ of $$[a,b]$$

Note that $\inf\{f(x): a_{k-1}\leq x\leq a_k\}\leq\sup\{f(x): a_{k-1}\leq x\leq a_k\}$$ for all $$k$$ and therefore

$$L(f,P) = \sum_{k=1}^n (a_k-a_{k-1})\inf\{f(x): a_{k-1}\leq x\leq a_k\} \leq \sum_{k=1}^n (a_k-a_{k-1})\sup\{f(x): a_{k-1}\leq x\leq a_k\} = U(f,P).$$

* (d) Prove that if $$P$$ and $$P'$$ are any two partitions of $$[a,b]$$ then, $$L(f,P)\leq U(f,P')$$.  You can use the fact that if $$P$$ and $$Q$$ are partitions and $$P\subseteq Q$$, then $$L(f,P)\leq L(f,Q)$$ and $$U(f,Q)\leq U(f,P)$$.

Let $$Q = P\cup P'$$. Then $$Q$$ is also a partition and $$P\subseteq Q$$ and $$P'\subseteq Q$$.
It follows that $$L(f,P)\leq L(f,Q)$$ and $$ U(f,P')\geq U(f,Q)$$.  Thus by part (c)

$$L(f,P)\leq L(f,Q)\leq U(f,Q)\leq U(f,P').$$

* (c) Prove that $$L(f)\leq U(f)$$.  

For any partition $$P'$$, (d) tells us $$U(f,P')$$ is an upper bound of $$\{L(f,P): P\ \text{is a partition of}\ [a,b]\}$$.  Therefore $$U(f,P')$$ is greater than or equal to its least upper bound, ie. it's supremum $$L(f)$$.
Since $$P'$$ was arbitrary, this tells us that $$L(f)$$ is a lower bound of $$\{ U(f,P): P\ \text{is a partition of}\ [a,b]\}$$.  Therefore $$L(f)$$ is less than it's greatest lower bound, ie. it's infimum $$U(f)$$.  Hence $$L(f)\leq U(f)$$.



