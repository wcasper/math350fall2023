---
layout: page
title: Homework 6 Solution
permalink: /homework/hw6-soln
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

* 19.2, 19.3
* 20.11, 20.13, 20.18, 
* 23.2, 23.4, ,23.7

**Solution to 19.2:**

* (a) 
Let $$\epsilon > 0$$.
Choose $$\delta = \epsilon/3$$.
Then for $$x,a\in\mathbb R$$ with $$\lvert x-a\rvert < \delta$$ we have

$$\lvert f(x)-f(a)\rvert = \lvert 3x+11-(3a+11)\rvert = 3\lvert x-a\rvert < \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary and $$\delta$$ depends only on $$\epsilon$$, this proves that $$f(x)$$ is uniformly continuous on $$\mathbb R$$.

* (b)
Let $$\epsilon > 0$$.
Choose $$\delta = \min\{1,\epsilon/4\}$$.
Then for $$x\in\mathbb R$$ and $$a\in [0,3]$$ with $$\lvert x-a\rvert < \delta$$, we have
$$\lvert x+a\rvert \leq 4$$ and therefore

$$\lvert f(x)-f(a)\rvert = \lvert x^2-a^2\rvert = \lvert x-a\rvert\cdot\lvert x+a\rvert < 3\delta = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary and $$\delta$$ depends only on $$\epsilon$$, this proves that $$f(x)$$ is uniformly continuous on $$\mathbb R$$.

* (c)
Let $$\epsilon > 0$$.
Choose $$\delta = \min\{1/4,\epsilon/8\}$$.
Then for $$x\in\mathbb R\backslash\{0\}$$ and $$a\in [1/2,\infty)$$ with $$\lvert x-a\rvert < \delta$$, we have
$$1/\lvert ax\rvert \leq 8$$ and therefore

$$\lvert f(x)-f(a)\rvert = \lvert 1/x-1/a\rvert = \lvert x-a\rvert/\lvert ax\rvert < 8\delta = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary and $$\delta$$ depends only on $$\epsilon$$, this proves that $$f(x)$$ is uniformly continuous on $$\mathbb R$$.

**Solution to 19.3:**

* (a)
Let $$\epsilon > 0$$.
Choose $$\delta = \min\{1/2,\epsilon/2\}$$.
Then for $$x\in\mathbb R\backslash\{-1\}$$ and $$a\in [0,2]$$ with $$\lvert x-a\rvert < \delta$$, we have
$$1/lvert (a+1)(x+1)\rvert \leq 2$$ and therefore

$$\lvert f(x)-f(a)\rvert = \lvert x/(x+1)-a/(a+1)\rvert = \lvert x-a\rvert/\lvert (a+1)(x+1)\rvert < 2\delta = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary and $$\delta$$ depends only on $$\epsilon$$, this proves that $$f(x)$$ is uniformly continuous on $$\mathbb R$$.


* (b)

Let $$\epsilon > 0$$.
Choose $$\delta = \min\{1/4,3\epsilon/2\}$$.
Then for $$x\in\mathbb R\backslash\{-1\}$$ and $$a\in [1,\infty)$$ with $$\lvert x-a\rvert < \delta$$, we have
$$1/lvert (2a+1)(2x+1)\rvert \leq 2/15$$ and therefore

$$\lvert f(x)-f(a)\rvert = \lvert 5x/(2x-1)-5a/(2a-1)\rvert = 5\lvert x-a\rvert/\lvert (2a+1)(2x+1)\rvert < 2\delta/3 = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary and $$\delta$$ depends only on $$\epsilon$$, this proves that $$f(x)$$ is uniformly continuous on $$\mathbb R$$.



**Solution to 20.11:**

* (a) $$2a$$
* (b) $$1/2\sqrt{b}$$
* (c) $$3a^2$$

**Solution to 20.13:**

* (a) Use the Product Law and Linearity for limits.
* (b) Use the Quotient Law for limits.
* (c) Use Linearity, plus the fact that $$\sqrt{x}$$ is continuous in its domain.

**Solution to 20.18:**

We calculate that for $$x\neq 0$$

$$\frac{\sqrt{1+3x^2}-1}{x^2} = \frac{3x^2}{x^2(\sqrt{1+3x^2}+1)} = \frac{3}{\sqrt{1+3x^2}+1}.$$

Therefore 

$$\lim_{x\rightarrow 0}\frac{\sqrt{1+3x^2}-1}{x^2} =\lim_{x\rightarrow 0} \frac{3}{\sqrt{1+3x^2}+1}.$$

The latter function is continuous (polynomials + square root are continuous; so are compositions and linear combinations and quotients) at $$x=0$$, so we can evaluate the limit by evaluating the function at $$x=0$$.  Thus the limit is $$3/2$$.

**Solution to 23.2:**

* (a) $$R = 1$$ and the interval is $$(-1,1)$$
* (b) $$R = 1$$ and the interval is $$[-1,1)$$
* (c) $$R = 1$$ and the interval is $$(-1,1)$$
* (d) $$R = 1/\sqrt{3}$$ and the interval is $$(-1/\sqrt{3},1/\sqrt{3})$$

**Solution to 23.4:**

* (a) $$\limsup \sqrt[n]{\lvert a_n\rvert } = 6/5$$, $$\liminf \sqrt[n]{\lvert a_n\rvert} = 2/5$$, $$\limsup \lvert a_{n+1}/a_n\rvert = \infty$$, and $$\liminf\lvert a_{n+1}/a_n\rvert = 0$$
* (b) Both series diverge by the Test for Divergence
* (c) The radius of convergence is $$5/6$$ and the interval of convergence is $$(-5/6,5/6)$$

**Solution to 23.7:**

* (a) If $$x$$ is not an integer multiple of $$\pi$$, then $$\lvert \cos x \rvert < 1$$ and therefore $$\lim (\cos x)^n = 0$$.
* (b) If $$x$$ is an even integer multiple of $$\pi$$ then $$\cos(x) = 1$$ and therefore $$\lim (\cos x)^n =1$$ so the limit is $$1$$
* (c) If $$x$$ is an odd integer multiple of $$\pi$$ then $$\cos(x) = -1$$ and therefore $$\lim (\cos x)^n =(-1)^n$$, so the limit doesn't exist


