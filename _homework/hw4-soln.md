---
layout: page
title: Homework 4
permalink: /homework/hw4-soln
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

* 14.2, 14.4, 14.7, 14.8
* 15.1, 15.3
* 16.4(a-c), 16.5(a-c), 16.6, 16.7

### Solutions

**Solution to 14.2:**

* (a) We have $$n^2+n-2 \geq n^2$$ for all $$n\geq 2$$ and therefore $$\frac{n-1}{n^2} > \frac{1}{n+2}.$$

The series $$\sum \frac{1}{n+2}$$ is the harmonic series (minus the first two terms) and diverges.
By the Comparison Test, it follows that $$\sum \frac{n-1}{n^2}$$ diverges.

* (b) This diverges by the Test for Divergence.

* (c) This converges since it is a $$p$$-series with $$p=2$$.
* (d) This converges by the Ratio Test
* (e) This converges by the Ratio Test
* (f) This converges by the Root Test
* (g) This converges by the Ratio Test

**Solution to 14.4:**

* (a) Note $$\frac{1}{(n+(-1)^n)^2} \leq \frac{1}{(n-1)^2}$$.  Since $$\sum_{n=2}^\infty \frac{1}{(n-1)^2} = \sum_{n=1}^\infty \frac{1}{n^2}$$ converges to $$\pi^2/6$$, so the Comparison Test implies that the series converges.
* (b) This is a telescoping sum.  The $$N$$'th partial sum is $$s_N = \sqrt{N+1} - 1$$, and since the partial sums diverge, the series does not converge.
* (c) We calculate 

$$\frac{a_{n+1}}{a_n} = \frac{(n+1)n^n}{(n+1)^{n+1}} = \frac{n^n}{(n+1)^n} = \frac{1}{\left(1+\frac{1}{n}\right)^{n}}.$$

Therefore 

$$\lim\frac{a_{n+1}}{a_n} = \frac{1}{\lim \left(1+\frac{1}{n}\right)^{n}} = \frac{1}{e} < 1.$$

By the Ratio Test, the series converges.


**Solution to 14.7:**

Since $$\sum a_n$$ converges, the sequence $$(a_n)$$ converges to $$0$$.
In particular the sequence is bounded, ie. there exists $$k > 0$$ such that $$\lvert a_n\rvert \leq k$$ for all $$n$$.
Since $$p-1 \geq 0$$, this implies $$\lvert a_n^{p-1}\rvert \leq k^{p-1}$$ for all $$n$$.
Thus $$a_n^p\leq k^{p-1}a_n$$ and since $$\sum k^{p-1}a_n = k^{p-1}\sum a_n$$ converges, the series $$\sum a_k^p$$ converges by the comparison test.

**Solution to 14.8:**

Since $$\sum a_n$$ and $$\sum b_n$$ are convergent series, the limits of the partial sums $$\lim_{N\rightarrow\infty} \sum_{n\leq N} a_n$$ and $$\lim_{N\rightarrow\infty} \sum_{n\leq N} b_n$$ exist.
By Linearity of Limits, we have that the limit

$$\begin{align}
\lim_{N\rightarrow\infty} \sum_{n\leq N} (a_n+b_n)\\
  & = \lim_{N\rightarrow\infty} \left(\left(\sum_{n\leq N} a_n\right) + \left(\sum_{n\leq N} b_n\right)\right)\\
  & = \lim_{N\rightarrow\infty} \left(\sum_{n\leq N} a_n\right) + \lim_{N\rightarrow\infty}\left(\sum_{n\leq N} b_n\right)
\end{align}$$

exists.  Therefore the sum $$\sum (a_n+b_n)$$ converges.

By the AM-GM Inequality, we know $$\sqrt{a_nb_n}\leq \frac{1}{2}(a_n+b_n)\leq (a_n + b_n)$$.

So $$\sqrt{a_nb_n}$$ converges by the Comparison Test.


**Solution to 15.1:**

* (a) Converges by Alternating Series Test
* (b) Diverges by Ratio Test

**Solution to 15.3:**

Viewing $$\sum_{n=2}^N \frac{1}{n\log(n)^p}$$ as a left and a right Riemann sum, we obtain the inequalities 

$$\int_2^{N+1} \frac{1}{x\log(x)^p} dx \leq \sum_{n=2}^N \frac{1}{n\log(n)^p} \leq \int_1^N\frac{1}{x\log(x)^p} dx.$$

If $$p > 1$$, then the integral on the right converges, forcing the sum to converge.
If $$p \leq 1$$, then the integral on the left diverges, forcing the sum to diverge.


**Solution to 16.4(a-c):**

* (a) $$2/10$$
* (b) $$1/45$$ 
* (c) $$2/99$$


**Solution to 16.5(a-c):**

* (a) $$0.125$$
* (b) $$0.0625$$
* (c) $$0.\overline{6}$$

**Solution to 16.6:**

$$\begin{align}
1/7 &= 0.\overline{142857}
2/7 &= 0.\overline{285714}
3/7 &= 0.\overline{428571}
4/7 &= 0.\overline{571428}
5/7 &= 0.\overline{714285}
6/7 &= 0.\overline{857142}
\end{align}$$

The repeated digits are cyclically permuted.

**Solution to 16.7:**

The given number is not rational.  To see this suppose that it was.
Then its decimal expansion would have the form

$$0.d_1d_2\dots d_r\overline{d_{r+1}d_{r+2}\dots d_{r+k}}.$$

However at some point the number $$1111\dots 1$$ (with $$r+k+1$$) many $$1$$'s has to occur in the expansion.
This is only possible if $$d_{r+1}=d_{r+2}=\dots=d_{r_k}=1$$.
Likewise, at some point the number $$2222\dots 2$$ (with $$r+k+1$$) many $$2$$'s has to occur in the expansion.
This is only possible if $$d_{r+1}=d_{r+2}=\dots=d_{r_k}=2$$.
This is a contradiction.
Therefore the number is not rational.

