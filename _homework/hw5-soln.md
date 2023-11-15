---
layout: page
title: Homework 5
permalink: /homework/hw5
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

Do the following book problems.

* 17.9, 17.11, 17.12, 17.14
* 18.4, 18.9, 18.10

### Solutions


**Solution to 17.9:**

* (a) Let $$\epsilon > 0$$.  Choose $$\delta = \min\{1,\epsilon/3\}$$.  Then for $$\lvert x-x_0\rvert < \delta$$ we have
$$\lvert x+2\rvert\leq 3$$ and therefore 

$$\lvert f(x)-f(x_0)\rvert = \lvert x^2-2^2\rvert = \lvert x-2\rvert\cdot \lvert x+2\rvert \leq 3\lvert x-2\rvert < 3\delta \leq \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that $$f(x)$$ is continuous at $$x_0$$.

* (b) Let $$\epsilon > 0$$.  Choose $$\delta = \epsilon^2$$.  Then for $$\lvert x-x_0\rvert < \delta$$ we have

$$\lvert f(x)-f(x_0)\rvert = \lvert \sqrt{x}-\sqrt{0} \rvert = \sqrt{\lvert x-0\rvert} < \sqrt{\delta} = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that $$f(x)$$ is continuous at $$x_0$$.

* (c) Let $$\epsilon > 0$$.  Choose $$\delta = \epsilon$$.  Then for $$\lvert x-x_0\rvert < \delta$$ and $$x\neq 0$$ we have
$$\lvert \sin(1/x)\rvert \leq 1$$ and therefore

$$\lvert f(x)-f(x_0)\rvert = \lvert x\sin(1/x)-0 \rvert \leq \lvert x\rvert < \delta = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that $$f(x)$$ is continuous at $$x_0$$.

* (d) Let $$\epsilon > 0$$.  Choose $$\delta = \min\{1,\epsilon/(2\lvert x_0\rvert + 1)^2\}$$.  Then for $$\lvert x-x_0\rvert < \delta$$, the triangle inequality says

$$\lvert x^2+x_0x+x_0^2\rvert \leq x^2+\lvert x_0x\rvert +x_0^2 \leq x^2+2\lvert x_0x\rvert +x_0^2 = (\lvert x_0\rvert +\lvert x\rvert)^2 \leq (2\lvert x_0\rvert + 1)^2.$$

Therefore 

$$\lvert f(x)-f(x_0)\rvert = \lvert x^3-x_0^3 \rvert = \lvert x-x_0\rvert\cdot\lvert x^2+2x_0x+x_0^2\rvert < \delta(2\lvert x_0\rvert + 1)^2 < \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that $$f(x)$$ is continuous at $$x_0$$.

**Solution to 17.11:**

If $$f(x)$$ is continuous at $$x_0$$ then every sequence $$(x_n)$$ converging to $$x_0$$ satisfies $$\lim f(x_n) = f(x_0)$$, so the statement holds for monic sequences as a specil case.

Conversely, suppose that $$\lim f(x_n) = f(x_0)$$ for all *monotonic* sequences $$(x_n)$$ converging to $$x_0$$.
Now let $$(x_n)$$ be any sequence converging to $$x_0$$, not necessarily monotonic.
Consider the sequence $$y_n = f(x_n)$$.  We don't yet know if this sequence converges or not, but it must have a subsequence $$(y_{n_k})$$ with $$\lim y_{n_k}$$ converging to $$\limsup y_n$$.
The corresponding sequence $$(x_{n_k})$$ has a monotone subsequence $$x_{n_{k_j}}$$.  Since this is a subsequence of the convergent sequence $$(x_n)$$ it must also converge, specifically to $$x_0$$.
Then by our assumption $$\lim_{j\rightarrow\infty} f(x_{n_{k_j}}) = f(x_0)$$.
Thus the convergent sequence $$(y_{n_k})$$ has a subsequence converging to $$f(x_0)$$.
It follows that $$y_{n_k}$$ must also converge to $$f(x_0)$$.  Hence $$\limsup y_n = f(x_0)$$.
Repeating this argument with $$\limsup$$ replaced with $$\liminf$$, we also get $$\liminf y_n = f(x_0)$$.
Consequently, $$\lim y_n$$ exists and is equal to $$f(x_0)$$, ie. $$\lim f(x_n) = f(x_0)$$.
Since $$(x_n)$$ was an arbitrary sequence, it follows that $$f(x)$$ is continuous at $$x_0$$.

**Solution to 17.12:**

* (a) Let $$x_0\in (a,b)$$.  Then by the Density of Rationals, for all $$n\in\mathbb{N}$$, there exists a rational number $$r_n$$ with $$a < x_0 < \min\{a+\frac{1}{n},b\}$$.
Then $$r_n\in (a,b)$$ for all $$n$$ and the Squeeze Theorem tells us that $$\lim r_n = x_0$$.  Since $$f(x)$$ is continuous at $$x_0$$, it follows that

$$f(x_0) = \lim f(r_n) = \lim 0 = 0.$$

Thus $$f(x)=0$$ for all $$x\in (a,b)$$.

* (b) Apply (a) to the function $$h(x) = f(x)-g(x)$$, which is continuous by the linearity property of continuity.  Then $$h(x)=0$$ on $$(a,b)$$ and therefore $$f(x)=g(x)$$ for all $$x\in (a,b)$$

**Solution to 17.14:**

Let $$a\in \mathbb{Q}$$ and consider the sequence $$a_n = a + \frac{\sqrt{2}}{n}$$.
Then $$a_n$$ is irrational for all $$n$$ and therefore $$f(a_n) = 0$$.  Moreover $$\lim a_n = a$$.  Since $$\lim f(a_n) = \lim 0 = 0\neq f(a)$$, this proves that $$f(x)$$ is NOT continuous at $$x=a$$.

Now suppose that $$a$$ is irrational.
To prove that $$f(x)$$ is continuous at $$x=a$$, we will assume otherwise and obtain a contradiction.
Suppose that $$f(x)$$ is not continuous at $$x=a$$.
Then there exists an $$\epsilon > 0$$ such that for all $$\delta > 0$$ there exists a real number $$x$$ with $$\lvert x-a\rvert < \delta$$ but $$\lvert f(x)-0\rvert \geq \epsilon.$$
Fix such an $$\epsilon$$.
For each $$n$$, choose $$x_n\in\mathbb R$$ with $$\lvert x_n-a\rvert < \frac{1}{n}$$ but $$\lvert f(x_n)\rvert \geq \epsilon$$.
This implies that each $$x_n$$ is rational, ie. $$x_n = p_n/q_n$$ for some relatively prime integers $$p_n,q_n$$ with $$q_n > 0$$.
Using the definition of $$f(x)$$, we find $$f(x_n) = 1/q_n$$.
Thus $$1/q_n \geq \epsilon$$ for all $$n$$, making $$q_n \leq 1/\epsilon$$.

Since $$(x_n)$$ converges, it must be bounded.
Therefore there exists a constant $$K$$ with $$\lvert p_n\rvert / q_n < K$$ for all $$n$$.
Hence $$\lvert p_n\rvert < K/\epsilon$$ for all $$n$$.
This means that the $$x_n$$'s all belong to the **finite** set

$$E = \{p/q: p,q\in\mathbb{Z},\ \lvert p\rvert < K/\epsilon,\ \ 1\leq q\leq 1/\epsilon\}.$$

This forces $$(x_n)$$ to converge to one of the points in $$E$$.  However all the points in $$E$$ are rational, and since $$x_n$$ converges to the irrational number $$a$$, this is a contradiction.

**Solution to 18.4:**

Consider the function $$f(x) = \frac{1}{x-x_0}$$.  This is a rational function, so it is continuous everywhere in its domain.
Moreoever, $$x_0\notin S$$, so $$S\subseteq \text{Dom}(f)$$ and $$f$$ is continuous on $$S$$.  However $$\lim x_n = x_0$$, and therefore for any $$K > 0$$ there exists an integer $$N$$ with $$\lvert x_n-x_0\rvert < 1/K$$.  It follows that $$\lvert f(x)\rvert > 1/K$$.
Since $$K > 0$$ was arbitrary, this proves that $$f(x)$$ is unbounded.

**Solution to 18.9:**

Let $$f(x) = a_0 + a_1x + \dots + a_nx^n$$ be a polynomial with $$a_n\neq 0$$ and $$n$$ odd.
Then

$$\lim_{x\rightarrow\pm\infty} f(x)/x^n = \pm a_n$$.

Therefore there exists an $$M > 0$$ such that $$x > M$$ implies , $$f(x)$$ has the same sign as $$a_n$$ and $$f(-x)$$ has the opposite sign of $$a_n$$.
In particular, there must be values $$a,b\in\mathbb{R}$$ with $$f(a)$$ and $$f(b)$$ having opposite signs.
Since $$f(x)$$ is continuous on $$(a,b)$$, the Intermediate Value Theorem implies that there exists a point between $$a$$ and $$b$$ where $$f(x)=0$$.
Thus $$f(x)$$ has at least one real root.


**Solution to 18.10:**

The function $$g(x)$$ satisfies $$g(0) = f(1)-f(0)$$ and $$g(1) = f(2)-f(1) = f(0)-f(1) = -g(0)$$.
If $$g(0) = 0$$, then $$f(0) = f(1)$$ so $$x=0$$ and $$y=1$$ works.
Otherwise, $$g(0)$$ and $$g(1)$$ have opposite signs, so the Intermediate Value Theorem implies that there exists an $$c\in (0,1)$$ with $$g(c) = 0$$. This implies $$f(c) = f(c+1)$$, so $$x=c$$ and $$y=c+1$$ works.


