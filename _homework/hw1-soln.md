---
layout: page
title: Homework 1 Solutions
permalink: /homework/hw1-soln
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

* 1.1, 1.3, and 1.6
* 2.4 and 2.5
* 3.6 
* 4.1 (a-j), 4.5, 4.11, 4.12, 4.14
* 7.3 (a-j), 7.5
* 8.2, 8.4, 8.5, 8.7 8.9

### Solutions

**Problem 1.1:**

We will prove this using induction.
As a base case, we see that $$1^2=\frac{1}{6}1(1+1)(2\cdot 1+1)$$, so the statement is true for $$n=1$$.
Let $$k\geq 1$$ be an integer.
As an inductive assumption, assume that the statement is true for $$n=k$$.
In other words, assume

$$1^2+2^2+\dots +k^2 = \frac{1}{6}k(k+1)(2k+1).$$

Then using this assumption, we calculate

$$\begin{align}
1^2+2^2+\dots +k^2+(k+1)^2\\
  & = \frac{1}{6}k(k+1)(2k+1) + (k+1)^2\\
  & = \frac{1}{6}\left[k(k+1)(2k+1) + 6(k+1)^2\right]\\
  & = \frac{1}{6}(k+1)\left[k(2k+1) + 6(k+1)\right]\\
  & = \frac{1}{6}(k+1)(k+2)(2k+3)
\end{align}$$

This proves our inductive step.
Thus by the Principle of Induction, the statement holds for all $$n$$.
:black_square_button:

**Problem 1.3:** 

First, recall that by Example 1 (or the famous story of baby Gauss) that

$$1+2+\dots + n = \frac{n(n+1)}{2}.$$

Using this, it suffices to show that for all $$n\in\mathbb{N}$$

$$1^3+2^3+\dots +n^3 = \frac{n^2(n+1)^2}{4}.$$

We will prove this using induction.
As a base case, we see that $$1^3=\frac{1^2(1+1)^2}{4}$$, so the statement is true for $$n=1$$.
Let $$k\geq 1$$ be an integer.
As an inductive assumption, assume that the statement is true for $$n=k$$.
In other words, assume

$$1^3+2^3+\dots +k^3 = \frac{k^2(k+1)^2}{4}.$$

Then using this assumption, we calculate

$$\begin{align}
1^3+2^3+\dots +k^3+(k+1)^3\\
  & = \frac{k^2(k+1)^2}{4} + (k+1)^3\\
  & = \frac{k^2(k+1)^2 + 4(k+1)^3}{4}\\
  & = \frac{(k+1)^2(k^2 + 4(k+1))}{4}\\
  & = \frac{(k+1)^2(k+2)^2}{4}
\end{align}$$

This proves our inductive step.
Thus by the Principle of Induction, the statement holds for all $$n$$.
:black_square_button:

**Problem 1.6:**

We will prove this using induction.
As a base case, we see that $$11-4$$ is divisible by $$7$$.
Let $$k\geq 1$$ be an integer.
As an inductive assumption, assume that the statement is true for $$n=k$$.
In other words, assume

$$7\ \text{divides}\ 11^k-4^k.$$

Then using this assumption, we can write $$11^k-4^k = 7m$$ for some integer $$m$$ and therefore

$$11^{k+1}-4^{k+1} = 11^k\cdot 11 - 4^k\cdot 4 = 11^k\cdot 7+(11^k-4^k)\cdot 4 = 7(11^k + 4m).$$

is divisible by $$7$$.
This proves our inductive step.
Thus by the Principle of Induction, the statement holds for all $$n$$.
:black_square_button:


**Problem 2.4:**

The number is a solution of the equation

$$x^6-10x^3 + 22 = 0.$$

If this polynomial equation has a rational root, then the Rational Roots Theorem implies that the root will be one of the following numbers $$\pm 1,\pm 2,\pm 11,$$ and $$\pm 22$$.
However, none of these numbers are solutions.
Therefore there are no rational solutions.
It follows that our number cannot be rational.
:black_square_button:

**Problem 2.5:**

The number is a solution of the equation

$$x^6-22x^3 + 49.$$

If this polynomial equation has a rational root, then the Rational Roots Theorem implies that the root will be one of the following numbers $$\pm 1,\pm 7,\pm 49$$.
However, none of these numbers are solutions.
Therefore there are no rational solutions.
It follows that our number cannot be rational.
:black_square_button:

**Problem 3.6:*

* (a)

$$\lvert a + b + c\rvert \leq \lvert a + b \rvert + \lvert c\rvert \leq \lvert a \rvert + \lvert b\rvert + \lvert c\rvert.$$ 

* (b)

We proceed by using induction on $$n$$.
The base case of $$n=1$$ is trivial.
Let $$k\geq 1$$ be an integer.  As an inductive assumption, assume that the statement is true for $$n=k$$.  In other words, assume that for any sequence of $$k$$ real numbers $$a_1,\dots, a_k$$ we have

$$\lvert a_1 + a_2 + \dots + a_k\rvert \leq \lvert a_1 \rvert + \lvert a_2 \rvert + \dots + \lvert a_k\rvert.$$

Now suppose we have a sequence $$k+1$$ real numbers $$a_1,\dots,a_{k+1}$$.
By the triangle inequality, we have

$$\lvert a_1 + a_2 + \dots + a_k + a_{k+1}\rvert \leq \lvert a_1 + a_2 + \dots + a_k\rvert + \lvert a_{k+1}\rvert.$$

Combining this with our inductive assumption, it follows that

$$\lvert a_1 + a_2 + \dots + a_k + a_{k+1}\rvert \leq \lvert a_1 \rvert + \lvert a_2 \rvert + \dots + \lvert a_k\rvert + \lvert a_{k+1}\rvert.$$

This proves the inductive step.  Hence by the Principle of Induction, the statement is true for all $$n\in\mathbb N$$.
:black_square_button:

**Problem 4.1:**

* (a) $$1,2,3$$
* (b) $$1,2,3$$
* (c) $$7,8,9$$
* (d) $$4,5,6$$
* (e) $$1,2,3$$
* (f) $$0,1,2$$
* (g) $$3,4,5$$
* (h) NBA
* (i) $$2,3,4$$
* (j) $$1,2,3$$

**Problem 4.5:**

Recall that $$\max S$$ (if it exists) is the unique element of $$S$$ which is also an upper bound of $$S$$.
Suppose that $$\sup S$$ is an element of $$S$$.
Then $$\sup S$$ is an upper bound of $$S$$, so $$\sup S = \max S$$.
:black_square_button:

**Problem 4.11:**

We will prove this by contradiction.
Let $$A$$ be the set of all rational numbers between $$a$$ and $$b$$.
Assume $$A$$ is finite.
Then the set $$A$$ has a minimum value $$c$$.
However by the Density of the Rationals Theorem, there exists a rational number $$r$$ with $$a < r < c$$.  In particular, we know $$a < r < b$$, so $$r\in A$$.  Since $$r < c$$, this contradicts the minimality of $$c$$.
We conclude that $$A$$ cannot be finite.
:black_square_button:

**Problem 4.12:**

First of all we need to show that for any rational number $$r$$, the value $$r + \sqrt{2}$$ is irrational.
To see this, suppose that for some rational number $$r$$ we have that $$r+\sqrt{2}$$ is rational.  Then $$r + \sqrt{2} = s$$ for some rational number $$s$$.
This means that $$\sqrt{2} = s-r$$ is the difference of two rationals and therefore rational.
However, Example 2 of Section 2 showed that $$\sqrt{2}$$ is irrational, so this is a contradiction.
Thus $$r + \sqrt{2}$$ is irrational for all rational numbers $$r$$.

Now let $$a < b$$. Then $$a-\sqrt{2} < b - \sqrt{2}$$. By the Density of the Rationals Theorem, there exists a rational number $$r$$ with $$a-\sqrt{2} < r < b - \sqrt{2}$$.
It follows that $$a < r + \sqrt{2} < b$$.  This shows that there is an irrational number between $$a$$ and $$b$$.
:black_square_button:

**Problem 4.14:** 

* (a) We first prove that $$\sup A + \sup B \geq \sup (A+B)$$.
To do so suppose that $$x\in A + B$$.
Then $$x = a + b$$ for some $$a\in A$$ and $$b\in B$$.
Since $$\sup(A)$$ is an upper bound for $$A$$, we know that $$a\leq\sup(A)$$.
Likewise, $$b\leq\sup(B)$$.
Consequently

$$x= a +b\leq \sup(A) + \sup(B).$$

Now since $$x\in A + B$$ was arbitrary, this proves that $$\sup(A)+\sup(B)$$ is an upper bound of $$A+B$$.
Since $$\sup(A+B)$$ is the *least* of the upper bounds of $$A+B$$, we conclude that $$\sup A + \sup B \geq \sup(A+B)$$.
[Note: this also proved that $$A+B$$ is bounded above so that we know $$\sup(A+B)$$ actually exists!]

Next we must show that $$\sup A + \sup B\leq \sup (A+B)$$.
To do this, let $$\epsilon > 0$$.
Then $$\sup A-\epsilon/2$$ cannot be an upper bound of $$A$$, because it is less than th least upper bound.
In particular, there exists $$a\in A$$ with $$a > \sup (A)-\epsilon/2$$.
By a similar arguement, there exists $$b\in B$$ with $$b > \sup (B) - \epsilon/2$$.
Consequently

$$\sup(A+B)\geq a+b > \sup(A)+\sup(B)-\epsilon.$$

Thus we have shown

$$\sup(A+B) > \sup(A)+\sup(B)-\epsilon,\ \ \forall\ \epsilon > 0.$$ 

This implies that $$\sup(A+B)\geq\sup(A)+\sup(B)$$.

Combining both parts, we conclude that $$\sup(A+B)=\sup(A)+\sup(B)$$.

* (b) For any bounded set $$C$$, let $$-C = \{-c: c\in C\}$$.  Note that

$$\inf(-C)\leq -c\leq \sup(-C)\ \forall\ c\in C.$$

Multiplying everything by $$-1$$, we get 

$$-\sup(-C)\leq c\leq -\inf(-C) \forall\ c\in C.$$

This makes $$-\sup(-C)$$ a lower bound for $$C$$ and $$-\inf(-C)$$ an upper bound for $$C$$.  Therefore

$$-\sup(-C)\leq \inf(C)\leq\sup(C)\leq-\inf(-C)$$.

The same inequality works for any set $$C$$, so it also works if we switch our initial set $$C$$ with $$-C$$.  This gives the inequality

$$-\sup(C)\leq \inf(-C)\leq\sup(-C)\leq-\inf(C)$$.

Combining these two inequalities, we obtain $$\sup(-C)=-\inf(C)$$ and $$\inf(-C)=-\sup(C)$$.

Thn since $$(-A)+(-B)=-(A+B)$$, the result of part (a) tells us

$$\inf(A)+\inf(B) = -(\sup(-A)+\sup(-B)) = -\sup(-(A+B)) = \inf(A+B).$$

:black_square_button:

**Problem 7.3:**

* (a) $$1$$
* (b) $$1$$
* (c) $$0$$
* (d) $$1$$
* (e) does not converge
* (f) $$1$$
* (g) does not converge
* (h) does not converge
* (i) $$0$$
* (j) $$7/2$$

**Problem 7.5:**

* (a)

We write

$$s_n = (\sqrt{n^2+1}-n)\frac{\sqrt{n^2+1}+n}{\sqrt{n^2+1}+n} = \frac{1}{\sqrt{n^2+1}+n}.$$

As $$n$$ goes to $$\infty$$, the denominator goes to $$\infty$$ while the numerator is fixed, so the limit is $$0$$.

* (b) 

We write

$$s_n = (\sqrt{n^2+n}-n)\frac{\sqrt{n^2+n}+n}{\sqrt{n^2+n}+n} = \frac{n}{\sqrt{n^2+n}+n} = \frac{1}{\sqrt{1+1/n}+1/n}.$$

As $$n$$ goes to $$\infty$$, the numerator stays at $$1$$ while the denominator goes to $$1$$, so the limit is $$1$$.

* (c)

We write

$$s_n = (\sqrt{4n^2+n}-2n)\frac{\sqrt{4n^2+n}+2n}{\sqrt{4n^2+n}+2n} = \frac{n}{\sqrt{4n^2+n}+2n} = \frac{1}{\sqrt{4+1/n}+2/n}.$$

As $$n$$ goes to $$\infty$$, the numerator stays at $$1$$ while the denominator goes to $$\sqrt{4}=2$$, so the limit is $$1/2$$.


**Problem 8.2:**

* (a)  The limit is $$0$$.  To see this, let $$\epsilon > 0$$.  Choose $$N=1/\epsilon$$.

Then for $$n>N$$, we have

$$\lvert a_n-0\rvert = \frac{n}{n^2+1} <  \frac{n}{n^2} = \frac{1}{n} < \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that the limit is $$0$$.

* (b)  The limit is $$7/3$$.  To see this, let $$\epsilon > 0$$.  Choose $$N=106/(9\epsilon)$$.

Then for $$n>N$$ we have

$$\lvert b_n-\frac{7}{3}\rvert = \frac{106}{9n+21} <  \frac{106}{9n} < \frac{106}{9N} = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that the limit is $$7/3$$.

* (c)  The limit is $$4/7$$.  To see this, let $$\epsilon > 0$$.  Choose $$N=\frac{41}{49\epsilon}+\frac{5}{7}$$

Then for $$n>N$$ we have

$$\lvert c_n-\frac{4}{7}\rvert = \frac{41}{7(7n-5)}  < \frac{41}{7(7N-5)} = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that the limit is $$4/7$$.

* (d) The limit is $$2/5$$.  To see this, let $$\epsilon > 0$$.  Choose $$N = \frac{16}{25\epsilon}$$

Then for $$n>N$$ we have

$$\lvert d_n-\frac{2}{5}\rvert = \frac{16}{25n+10} < \frac{16}{25n} < \frac{16}{25N} =\epsilon$$.

Since $$\epsilon > 0$$ was arbitrary, this proves that the limit is $$2/5$$.

* (e) The limit is $$0$$.  To see this, let $$\epsilon > 0$$.  Choose $$N=\frac{1}{\epsilon}.$$

Then $$\lvert \sin(n)\rvert \leq 1$$, and therefore $$\frac{1}{n}\lvert \sin(n)\rvert \leq \frac{1}{n}$$.

Thus for $$n>N$$, we have

$$\lvert s_n-0\rvert = \frac{\lvert \sin(n)\rvert}{n} \leq \frac{1}{n} < \frac{1}{N}=\epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves that the limit is $$0$$.

**Problem 8.4:**  Let $$\epsilon > 0$$.  Since $$\lim s_n=0$$, we may choose $$N$$ such that $$n>N$$ implies $$\lvert s_n-0\rvert < \epsilon/M$$.  This means that for $$n>N$$

$$\lvert s_nt_n-0\rvert = \lvert s_n\rvert\cdot\lvert t_n\rvert < (\epsilon/M)M=\epsilon$$.

Since $$\epsilon> 0$$ was arbitrary, this proves $\lim s_nt_n = 0$$.

:black_square_button:

**Problem 8.5:**  

* (a)

Let $$\epsilon > 0$$.

Then we can choose $$N_1$$ and $$N_2$$ with $$\lvert a_n-s\rvert < \epsilon/3$$ whenevery $$n> N_1$$ and $$\lvert b_n-s\rvert < \epsilon/3$$ whenever $$n > N/3$$.
Furthermore, we can choose $$N_3$$ with $$a_n\leq s_n\leq b_n$$ whenever $$n>N_3$$.

Therefore for $$n>\max(N_1,N_2,N_3)$$ we have $$a_n\leq s_n\leq b_n$$ we know

$$\begin{align}
\lvert s_n-s\rvert
 & \leq \lvert s_n-a_n+a_n-s\rvert\\
 & \leq \lvert s_n-a_n \rvert + \lvert a_n-s\rvert\\
 & \leq \lvert b_n-a_n \rvert + \lvert a_n-s\rvert\\
 & \leq \lvert b_n-s+s-a_n \rvert + \lvert a_n-s\rvert\\
 & \leq \lvert b_n-s\rvert +\lvert s-a_n \rvert + \lvert a_n-s\rvert < \epsilon.
\end{align}$$

Since $$\epsilon > 0$$ was arbitrary, this proves $$\lim s_n = s$$.

* (b)

By linearity properties of sequences, we know $$\lim -t_n= 0$$.
Since $$-t_n < s_n < t_n$$, we can apply the Squeeze Theorem to find $$\lim s_n=0$$.

:black_square_button:

**Problem 8.7:**

* (a) Suppose that the limit exists and is equal to $$L$$.
Then we can choose $$N$$ such that $$n>N$$ implies $$\lvert \cos(n\pi/3)-L\rvert < 1/2$$.
Suppose $$n > N$$ is a positive odd integer.  Then $$3n > N$$, so 

$$\lvert \cos(3n\pi/3)-L\rvert = \lvert -1-L\rvert < 1/2$$

Moreover $$6n > N$$ also, so

$$\lvert \cos(6n\pi/3)-L\rvert = \lvert 1-L\rvert < 1/2$$

Combined, this shows that $$L$$ is a number simultaneously greater than $$1/2$$ and less than $$-1/2$$, which is impossible.

* (b) Bounded sequences converge.  Since this sequence is unbounded, it does not converge.

* (c) Suppose that the limit exists and is equal to $$L$$.
Then we can choose $$N$$ such that $$n>N$$ implies $$\lvert \sin(n\pi/3)-L\rvert < 1/4$$.
Suppose $$n > N$$ is a positive integer.  Then $$6n+1 > N$$, so 

$$\lvert \sin((6n+1)\pi/3)-L\rvert = \lvert 1/2-L\rvert < 1/4$$

Moreover $$6n > N$$ also, so

$$\lvert \sin(6n\pi/3)-L\rvert = \lvert 0-L\rvert < 1/4$$

The first inequality implies $$L > 1/4$$.  The second implies, $$L < 1/4$$.  This is a contradiction.

**Problem 8.9:**

* (a) Suppose that $$s_n \geq a$$ for all but finitely many $$n$$ and that the seqeuence converges.

Let $$s=\lim s_n$$.  We will prove $$s\geq a$$ by contradiction.  Suppose that $$s < a$$.
Then we can choose $$N_1$$ such that $$n>N_1$$ implies $$\lvert s_n-s\rvert < a-s$$.
Also, we can choose $$N_2$$ such that $$n>N_2$$ implies $$s_n\geq a$$ (dodging the finitely many terms where this inquality doesn't hold).
Thus for $$n>\max(N_1,N_2)$$, we have $$a-s < s_n-s$$ and

$$s_n-s \leq \lvert s_n-s\rvert < a-s$$.

This is a contradiction.  Therefore, $$s\geq a$$.

* (b) Suppose that $$s_n \leq b$$ for all but finitely many $$n$$ and that the seqeuence converges.  Then $$-s_n \geq -b$$ for all but finitely many $$n$$ and therefore $$\lim -s_n \geq -b$$ by the result of (a).  Then by linearity properties of limits

$$\lim s_n = -\lim -s_n \leq b.$$

This proves (b).

* (c)  Since $$s=\lim s_n$$ is $$\geq a$$ by (a) and $$\leq b$$ by (b), we get $$s\in [a,b]$$.

