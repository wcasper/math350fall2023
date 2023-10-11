---
layout: page
title: Homework 3 Solutions
permalink: /homework/hw3-soln
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

* 11.2, 11.4, 11.8
* 12.3 (a-f), 12.6, 12.8, 12.12

Also do the following three problems.

**Problem A:**  Let $$(r_n)$$ be a sequence where each rational number appears at least once.  Prove that if $$t$$ is any real number, then there exists a subsequence of $$(r_n)$$ which converges to $$t$$.

**Problem B:**  Suppose that $$(a_n)$$ is a sequence which converges to $$a$$ and that $$(s_n)$$ is a sequence with the property that for all $$k\in\mathbb{N}$$ there is a subsequence of $$s_n$$ which converges to $$a_k$$.  Prove that there is a subsequence of $$s_n$$ which converges to $$a$$.

[Hint: use the property that a number $$x$$ is the limit of a subsequence of $$(s_n)$$ if and only if for all $$\epsilon>0$$ the set $$\{n\in\mathbb{N}: \lvert s_n-x\rvert <  \epsilon\}$$ is infinite.]

**Problem C:**  Construct examples of each of the following:

* a sequence of numbers $$(s_n)$$ with $$\limsup s_n = -\infty$$
* a sequence of numbers $$(s_n)$$ with $$\limsup s_n = +\infty$$
* a sequence of **rational** numbers $$(r_n)$$ with $$\limsup r_n = \sqrt{3}$$ and $$\liminf r_n = \sqrt{2}$$


### Solutions

**Problem 11.2**

* (a) The sequences $$(b_n)$$, $$(c_n)$$ and $$(d_n)$$ are already monotone, so we can take the subsequence to be the whole sequence.  For $$(a_n)$$ we take the subsequence $$(t_n)$$ defined by $$t_k = a_{2k}\forall k\in\mathbb{N}$$.
* (b) The set of subsequential limits for $$(a_n)$$, $$(b_n)$$, $$(c_n)$$, and $$(d_n)$$ are given respectively by $$\{1,-1\}$$, $$\{0\}$$, $$\{\infty\}$$, and $$\{6/7\}.$$
* (c) 

$$\limsup a_n = 1,\ \ \ \liminf a_n = -1,$$ 

$$\limsup b_n = 0,\ \ \ \liminf b_n = 0,$$ 

$$\limsup c_n = +\infty,\ \ \ \liminf c_n = +\infty,$$ 

$$\limsup d_n = 6/7,\ \ \ \liminf d_n = 6/7.$$


* (d) This happens only when the limsup and liminf agree.  So  $$(b_n)$$ and $$(d_n)$$ converge and $$(c_n)$$ diverges to $$+\infty$$


**Problem 11.4**

* (a) Monotone subsequences are given by $$w_{2n}$$, $$x_{2n}$$, $$y_{2n}$$ and $$z_{8n}$$
* (b) The set of subsequential limits for $$(w_n)$$, $$(x_n)$$, $$(y_n)$$, and $$(z_n)$$ are given respectively by $$\{-\infty,\infty\}$$, $$\{0,5\}$$, $$\{0,2\}$$, and $$\{-\infty, 0, +\infty\}.$$
* (c) 

$$\limsup w_n = \infty,\ \ \ \liminf w_n = -\infty,$$ 

$$\limsup x_n = 5,\ \ \ \liminf x_n = 0,$$ 

$$\limsup y_n = 2,\ \ \ \liminf y_n = 0,$$ 

$$\limsup z_n = \infty,\ \ \ \liminf z_n = -\infty.$$


* (d)  None of the sequences converge or diverge to $$\pm\infty$$ because the limsup and liminfs are always different


**Problem 11.8**

Let $$A$$ be any set of real numbers and write $$-A = \{-x: x\in A\}$$.

Note that

$$\inf(-A)\leq -a\leq \sup(-A)\ \forall\ a\in A.$$

Multiplying everything by $$-1$$, we get 

$$-\sup(-A)\leq a\leq -\inf(-A) \forall\ a\in A.$$

This makes $$-\sup(-A)$$ a lower bound for $$A$$ and $$-\inf(-A)$$ an upper bound for $$A$$.  Therefore

$$-\sup(-A)\leq \inf(A)\leq\sup(A)\leq-\inf(-A)$$.

The same inequality works for any set $$A$$, so it also works if we switch our initial set $$A$$ with $$-A$$.  This gives the inequality

$$-\sup(A)\leq \inf(-A)\leq\sup(-A)\leq-\inf(A)$$.

Combining these two inequalities, we obtain $$\sup(-A)=-\inf(A)$$ and $$\inf(-A)=-\sup(A)$$.

Now consider the set $$A_N = \{s_n: n\geq N\}$$.  Using the above result, we have $$\inf A_N = -\sup(-A_N)$$.  Therefore using Linearity of Limits

$$\liminf s_n = \lim_{N\rightarrow\infty} \inf A_N = \lim_{N\rightarrow\infty} -\sup (-A_N) = -\lim_{N\rightarrow\infty}\sup(-A_N) = -\limsup(-s_n)$$.


**Problem 12.3 (a-f)**

* (a) $$0$$
* (b) $$1$$
* (c) $$2$$
* (d) $$3$$
* (e) $$4$$
* (f) $$0$$

**Problem 12.6**

* (a) 

First let $$A$$ be any bounded set of real numbers and let $$k\geq 0$$, and as an abuse of notation let $$kA := \{kx: x\in A\}.$$

Then $$\sup(A)$$ is an upper bound for $$A$$ and therefore $$a\leq \sup(A) for all $$a\in A$$.
Consequently $$ka\leq k\sup(A)$$ for all $$a\in A$$ making $$k\sup(A)$$ an upper bound of the set $$kA$$.
Hence $$\sup(kA)\leq k\sup(A)$$.

Likewise, $$\sup(kA)$$ is an upper bound of the set $$kA$$ and therefore $$b\leq \sup (kA)$$ for all $$b\in kA$$.
Equivalently, $$ka\leq \sup(kA)$$ for all $$a\in A$$.
It follows that $$a\leq \frac{1}{k}\sup(kA)$$ for all $$a\in A$$ and therefore $$\frac{1}{k}\sup(kA)$$ is an upper bound of $$A$$.
Hence $$\sup(A)\leq \frac{1}{k}\sup(kA)$$, or equivalently $$k\sup(A)\leq \sup(kA)$$.

Putting both inequalities together, we find $$\sup(kA) = k\sup(A).$$

Now consider the collection of sets $$A_N = \{s_n: n\geq N\}.$$
Applying the above result, we know $$\sup(kA_N) = k\sup(A_N)$$ and therefore by Linearity of Limits

$$\begin{align}
\limsup(ks_n)
  &= \lim_{N\rightarrow\infty}\sup(kA_N)\\
  & = \lim_{N\rightarrow\infty} k\sup(A_N)\\
  & = k\lim_{N\rightarrow\infty}\sup(A_N) = k\limsup(s_n).
\end{align}$$

* (b) We calculate

$$\liminf(ks_n) = -\limsup(-ks_n) = -\limsup(k(-s_n)) = -k\limsup(-s_n) = k\liminf(s_n).$$

* (c) If $$k < 0$$ then we get $$\limsup(ks_n) = k\liminf(s_n)$$ and $$\liminf(ks_n) = k\limsup(s_n).$$


**Problem 12.8**

Define

$$M_N^{(s)} = \sup\{s_n: n\geq N\},\ \ M_N^{(t)} = \sup\{t_n: n\geq N\},\ \ M_N^{(st)} = \sup\{s_nt_n: n\geq N\}.$$

Then for $$n\geq N$$ we have $$s_n\leq M_N^{(s)}$$ and $$t_n\leq M_N^{(t)}$$, and therefore

$$s_nt_n\leq M_N^{(s)}M_N^{(t)}.$$

In particular $$M_N^{(s)}M_N^{(t)}$$ is an upper bound for the set $$\{s_nt_n: n\geq N\}$$.  Thus it must be greater than the least upper bound, ie.

$$M_N^{(st)}\leq M_N^{(s)}M_N^{(t)}.$$

Taking the limit of both sides with respect to $$N$$ and applying the Product Law for Limits

$$\begin{align}\limsup (s_nt_n)
  & = \lim_{N\rightarrow\infty}M_N^{(st)}\\
  & \leq \lim_{N\rightarrow\infty}(M_N^{(s)}M_N^{(t)})\\
  & = \left(\lim_{N\rightarrow\infty}M_N^{(s)}\right)\left\lim_{N\rightarrow\infty}M_N^{(t)}\right)\\
  & = (\limsup s_n)(\limsup t_n).
\end{align}$$


**Problem 12.12**

* (a) 

First of all, let 

$$M_N = \sup\{s_n: n\geq N\},\ \ \ \widetilde{M_N} = \sup\{\sigma_n: n\geq N\}.$$

Then for any $$n> M > N$$ we have

$$\begin{align}
\sigma_n = \frac{s_1+\dots+s_n}{n}
  & = \frac{s_1+\dots + s_N}{n} + \frac{s_{N+1}+\dots + s_n}{n}\\
  & \geq \frac{s_1+\dots + s_N}{n} + \frac{(n-N)M_N}{n}\\
  & \geq \frac{s_1+\dots + s_N}{M} + \frac{(n-N)M_N}{n}\\
  & \geq \frac{s_1+\dots + s_N}{M} + M_N
\end{align}$$

Thus $$\frac{s_1+\dots + s_N}{M} + \frac{(n-N)M_N}{n}$$ will be an upper bound of the set $$\{\sigma_n: n\geq N\}$$ and consequently

$$\widetilde{M_N} \leq \frac{s_1+\dots + s_N}{M} + M_N.$$

Taking the limit as $$M\rightarrow\infty$$, this gives

$$\widetilde{M_N} \leq  M_N.$$

Now taking the limit as $$N\rightarrow\infty$$, we get

$$\limsup\sigma_n = \lim_{N\rightarrow\infty}\widetilde{M_N}\leq \lim_{N\rightarrow\infty} M_N=\limsup s_n.$$


This was true for *any* sequence, so we can also apply it to the sequence $$(-s_n)$$, to get

$$\limsup(-\sigma_n)\leq \limsup (-s_n).$$

Equivalently, 

$$-\liminf(\sigma_n)\leq -\liminf (s_n).$$

Now multiplying by $$-1$$, we find

$$\liminf \sigma_n \geq \liminf s_n.$$

Putting all of this together, we have

$$\liminf s_n \leq \liminf \sigma_n \leq\limsup \sigma_n \leq\limsup s_n.$$

* (b) 

Suppose that $$\lim s_n$$ exists and is equl to $$s$$.  Then $$\liminf s_n = \limsup s_n = s.$$  Therefore

$$s = \liminf s_n \leq \liminf \sigma_n \leq\limsup \sigma_n \leq\limsup s_n = s.$$

It follows that $$\liminf\sigma_n = \limsup \sigma_n = s.$$  Therefore $$\lim \sigma_n$$ exists and is equal to $$s$$.

* (c) Consider the sequence $$(s_n)$$ defined by $$s_n = (-1)^n$$.  The limit of this sequence does not exist.  However,

$$(\sigma_1,\sigma_2,\sigma_3,\dots) = (-1, 0 -1/3, 0, -1/5, 0, -1/6, 0,\dots)$$

in other words $$\sigma_n = -1/n$$ if $$n$$ is odd and $$0$$ if $$n$$ is even.  In particular $$\lim \sigma_n$$ exists and is equal to $$0$$.

**Problem A:**  

Recall that by a previous exercise, between any two different real numbers there are infinitely many rational numbers.
Consequently, for any real numbers $$a$$ and $$b$$ and any integer $$N$$, the set

$$\{n\in\mathbb{N}: n >N\ \ \text{and}\ \ a < r_n < b\}$$

is non-empty!

Choose $$n_1\in\mathbb{N}$$ so that $$r_{n_1}$$ is a rational number between $$t-1$$ and $$1$$.
Define $$n_k$$ recursively by choosing $$n_1$$ so that $$t-1 < r_{n_1} < t$$  and more generally

$$n_{k+1} \in \{n\in\mathbb{N}: n > n_{k+1}\ \ \text{and}\ \ t-\frac{1}{k} < r_n < t\}.$$

Then since $$n_1 < n_2 < n_3 < \dots$$ the sequence $$(t_n)$$ defined by $$t_k := r_{n_k}$$ for all $$k\in\mathbb{N}$$ is a subsequence of $$(r_n)$$.

Furthermore, 

$$t-\frac{1}{k}\leq r_{n_k} \leq t$$

So by the Squeeze Theorem, $$\lim t_k = \lim r_{n_k} = t.$$


**Problem B:**  Suppose that $$(a_n)$$ is a sequence which converges to $$a$$ and that $$(s_n)$$ is a sequence with the property that for all $$k\in\mathbb{N}$$ there is a subsequence of $$s_n$$ which converges to $$a_k$$.  Prove that there is a subsequence of $$s_n$$ which converges to $$a$$.

Our idea is to avoid actually having to construct a subsequence converging to $$a$$ by applying Theorem 11.2.  By this theorem, if we can show $$\{n: \lvert s_n-a\rvert < \epsilon\}$$ is an infinite set for all $$\epsilon > 0$$ then $$a$$ must be the limit of a subsequence of $$(s_n)$$.
This is an existence proof (as opposed to a constructive proof).

Let $$\epsilon > 0$$.

Then since $$a_n$$ converges to $$a$$, there exists an integer $$N$$ such $$n>N$$ implies $$\lvert a_n-a\rvert < \epsilon /2.$$

Moreover, $$a_{N+1}$$ is the limit of a subsequence of $$(s_n)$$ so the set

$$\{n: \lvert s_n-a_{N+1}\rvert < \epsilon/2\}$$

is infinite by Theorem 11.2.

Now by the Triangle Inequality, if $$\lvert s_n-a_{N+1}\rvert < \epsilon/2$$ we have 

$$\lvert s_n-a\rvert = \lvert s_n - a_{N+1}+a_{N+1}- a\rvert \leq \lvert s_n - a_{N+1}\rvert + \lvert a_{N+1}- a\rvert < \epsilon/2 + \epsilon/2 = \epsilon.$$

Thus we have

$$\{n: \lvert s_n-a_{N+1}\rvert < \epsilon/2\}\subseteq \{n: \lvert s_n-a\rvert < \epsilon\}.$$

In particular both sets must be infinite.  Since $$\epsilon > 0$$ was arbitrary, this shows that $$a$$ is the limit of some subsequence of $$(s_n)$$.


**Problem C:**  Construct examples of each of the following:

* a sequence of numbers $$(s_n)$$ with $$\limsup s_n = -\infty$$
* a sequence of numbers $$(s_n)$$ with $$\limsup s_n = +\infty$$
* a sequence of **rational** numbers $$(r_n)$$ with $$\limsup r_n = \sqrt{3}$$ and $$\liminf r_n = \sqrt{2}$$

* For the first sequence, take $$s_n = -n$$
* For the second sequence, take $$s_n = n$$
* For the third sequence, we need to work a bit.

For each $$k\in\mathbb{N}$$, let $$a_k$$ and $$b_k$$ be rational numbers satisfying

$$\sqrt{3} < a_k < \sqrt{3} + \frac{1}{k},\ \ \text{and}\ \ \sqrt{2}-\frac{1}{k} < b_k < \sqrt{2}.$$

Then the Squeeze Theorem implies $$\lim a_k = \sqrt{3}$$ and $$\lim b_k = \sqrt{2}.$$

Without loss of generality, we may assume that $$a_k$$ and $$b_k$$ are monically decreasing and increasing, respectively (since otherwise we could replace them with monotone subsequences of the previous sequences).

Now make a new sequence $$(r_n)$$ by splicing together the previous two sequences:

$$(r_1,r_2,r_3,r_4,\dots) = (a_1,b_1,a_2,b_2,a_3,b_3,\dots)$$

or equivalently

$$r_k = \left\lbrace\begin{array}{cc}a_{(k+1)/2}, & k\ \text{odd}\\ a_{k/2}, & k\ \text{even}\end{array}\right.$$

Then 

$$\limsup r_k = \lim_{N\rightarrow\infty}\sup\{r_k: k\geq N\} = \lim_{N\rightarrow\infty} a_{\lceil n/2\rceil} = \sqrt{3}.$$

$$\liminf r_k = \lim_{N\rightarrow\infty}\inf\{r_k: k\geq N\} = \lim_{N\rightarrow\infty} b_{\lceil n/2\rceil} = \sqrt{2}.$$


