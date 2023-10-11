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

Do the following book problems.

* 9.4, 9.12, 9.15
* 10.3, 10.6, 10.8
* 11.1

### Solutions

**Solution to 9.4**

* (a) The first four terms are

$$s_1 = 1,\ \ s_2 = \sqrt{2},\ \ s_3 = \sqrt{1+\sqrt{2}},\ \ s_4 = \sqrt{1 + \sqrt{1+\sqrt{2}}}.$$

* (b) Note that $$s_{n+1}^2 = s_n + 1$$.  Taking the limit of both sides and using Limit Laws, we see that the limit $$s=\lim s_n$$ satisfies

$$s^2 = s+1.$$

The solutions of this are $$\frac{1}{2}(1\pm\sqrt{5})$$.  The sequence is all positive, so the limit must be nonnegative and is therefore $$\frac{1+\sqrt{5}}{2}$$.

**Solution to 9.12**

* (a) Since $$L < 1$$, we can choose a positive integer $$N$$ such that $$n > N$$ implies

$$\left\lvert\left\lvert \frac{s_{n+1}}{s_n} \right\rvert - L\right\rvert < \frac{1-L}{2}.$$

Then for $$n > N$$ we have $$\lvert s_{n+1}/s_n\rvert  < L + \frac{1+L}{2}$$ or equivalently $$\lvert s_n \rvert \leq a$$ for $$a := \frac{1+L}{2} \in [0,1).$$
A basic inductive argument then shows

$$0 \leq \lvert s_{N+k+1} \rvert \leq a^k\lvert s_{N+1}\rvert\ \forall k\in\mathbb{N}.$$

Now $$N$$ is fixed, but we can still take the limit as $$k\rightarrow\infty$$.  Since $$0 \leq a < 1$$, $$\lim_k a^k = 0$$.
Therefore since

$$-a^k\lvert s_{N+1}\rvert\leq s_{N+k+1}\leq a^k\lvert s_{N+1}\rvert$$

the Squeeze Theorem tells us that

$$\lim_{n\rightarrow\infty} s_n = \lim_{k\rightarrow\infty} s_{N+k+1} = 0.$$

* (b) Consider the sequence $$t_n = 1/\lvert s_n\rvert$$.  Then by using Limit Laws, we see

$$\lim_{n\rightarrow\infty} \left\lvert \frac{t_{n+1}}{t_n}\right\rvert = \lim_{n\rightarrow\infty} \frac{1}{\frac{s_{n+1}}{s_n}} = \frac{1}{L} < 1.$$
Therefore by applying the result of part (a) to the sequence $$(t_n)$$, we know that $$\lim t_n = 0.$$
Hence by Theorem 9.10, $$\lim \lvert s_n\rvert = +\infty$$.

**Solution to 9.15**

To solve this, let $$s_n = a^n/n!$$ and note that $$\frac{s_{n+1}}{s_n} = a/n$$.  Therefore

$$\lim_{n\rightarrow\infty} \left\lvert\frac{s_{n+1}}{s_n}\right\rvert = \lim_{n\rightarrow\infty}\frac{\lvert a\rvert }{n} = 0 < 1.$$

By Problem 9.12, we find that $$\lim_{n\rightarrow\infty} a_n = 0.$$

**Solution to 10.3**

The sequence $$(s_n)$$ is defined by

$$s_n = K + \frac{d_1}{10} + \frac{d_2}{10^2} + \dots + \frac{d_n}{10^n}.$$

Therefore

$$s_n \leq K + \frac{9}{10} + \frac{9}{10^2} + \dots + \frac{9}{10^n}$$

and using our geometric sum formula

$$1 + r + r^2 + \dots + r^{n-1} = \frac{1-r^n}{1-r}$$

with $$r = \frac{1}{10}$$, we find that

$$
\begin{align}
s_n & \leq K + \frac{9}{10}(1 + \frac{1}{10} + \dots + \frac{1}{10^{n-1}}\\
    &    = K + \frac{9}{10}\frac{1-10^{-n}}{1-10^{-1}} = K + 1-\frac{1}{10^n} < K+1
\end{align}$$

Thus $$s_n < K+1$$ for all $$n\in\mathbb{N}$$.


**Solution to 10.6**

* (a)  We calculate that for all $$n,k\in\mathbb{N}$$

$$\begin{align}
\lvert s_{n+k}-s_n\rvert
  & = \lvert s_{n+k}-s_{n+k-1}+-s_{n+k-1}-s_{n+k-2}+s_{n+k-2}-\dots + s_{n+1}-s_n\rvert\\
  & \leq \lvert s_{n+k}-s_{n+k-1}\rvert + \lvert s_{n+k-1}-s_{n+k-2}\rvert + \dots + \lvert s_{n+1}-s_{n}\rvert\\
  & \leq 2^{-(n+k-1)} + 2^{-(n+k-2)} + \dots + 2^{-n}\\
  & =  2^{-n}(2^{-(k-1)} + 2^{-(k-2)} + \dots + 1) = 2^{1-n}(1-2^{-k}) < 2^{1-n}.
\end{align}$$

Now let $$\epsilon > 0$$.
Choose $$N = 1-\log_2(\epsilon)$$.
Suppose that $$m,n>N$$ and without loss of generality assume $$m>n$$.  Then for $$k=m-n$$ the above calculation shows

$$\lvert s_m-s_n\rvert \leq 2^{1-n} < 2^{1-N}=\epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this shows $$(s_n)$$ satisfies the definition of a Cauchy sequence.

* (b) Consider the sequence defined by

$$s_n = \frac{1}{1} + \frac{1}{2} + \frac{1}{3} + \frac{1}{n}$$.

Then $$\lvert s_{n+1}-s_n\rvert = \frac{1}{n+1} < \frac{1}{n}$$ for all $$n\in\mathbb N$$.

Furthermore,  $$s_n$$ represents the left Riemann sum of the monotone decreasing function $$f(x) = \frac{1}{x}$$ on the interval $$[1,n+1]$$ with $$n$$ rectangles.  Hence

$$s_n\geq \int_1^{n+1}\frac{1}{x} dx = \ln(n+1).$$

Since $$\lim \ln(n+1) = +\infty$$, it follows that $$\lim s_n = \infty$$.  In particular $$(s_n)$$ is not bounded and therefore not Cauchy!

**Solution to 10.8**

We need to show that $$\sigma_{n+1} \geq \sigma_n$$ for all $$n$$.

Since the sequence is increasing, we know that $$a_{n}\geq a_k$$ for all $$1\leq k \leq n$$.
Using this, we calculate

$$\sigma_{n+1}-\sigma_n
  & = \frac{n(a_1+\dots+a_n+a_{n+1})-(n+1)(a_1+\dots+a_n)}{n(n+1)}\\
  & = \frac{na_{n+1}-(a_1+\dots+a_n)}{n(n+1)}\\
  & \leq \frac{na_{n+1}-na_n}{n(n+1)} = \frac{a_{n+1}-a_n}{n+1} \geq 0.
$$

**Solution to 11.1**

* (a) 

$$(a_1,a_2,a_3,\dots) = (1,5,1,5,1,5,1,5,\dots)$$

* (b) Let $$(t_n)$$ be the subsequence of $$(s_n)$$ defined by $$t_k = s_{2k}$$.  Then $$t_k = 5$$ for all $$k$$.
