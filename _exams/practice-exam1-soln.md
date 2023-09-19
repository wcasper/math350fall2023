---
layout: page
title: Practice Exam 1 Solutions
permalink: /exams/practice-exam1-soln
---

Solve each of the following problems.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1 (True or False)
For each of the following, write TRUE if the statement is true and FALSE if the statement is false.  NO explanation is needed.
Assume both $$(s_n)$$ and $$(t_n)$$ are sequences of real numbers.

a) If $$s_n <  t_n$$ for all $$n$$ then $$\lim s_n < \lim t_n$$

FALSE

b) The Well-Ordering Principle is equivalent to the Axiom of Induction

TRUE

c) Any set of real numbers which is bounded above has a maximum

FALSE

d) Every bounded sequence of real numbers is a Cauchy sequence

FALSE

e) If $$\lim s_n=0$$, then $$\lim s_nt_n = 0$$

FALSE

## Problem 2

a) State the Completeness Axiom

The Completeness Axiom states that any set of real numbers which is bounded above has a supremum.

b) State the definition of a sequence $$(s_n)$$ converging to $$s$$

A sequence $$(s_n)$$ converges to $$s$$ if for all $$\epsilon > 0$$ there exists a number $$N$$ such that $$n>N$$ implies $$\lvert s_n-s\rvert < \epsilon$$.

c) Carefully state the Squeeze Theorem.

Let $$(a_n), (b_n),$$ and $$(s_n)$$ be sequences and suppose $$a_n \leq s_n\leq b_n$$ for all $$n$$.
If $$\lim a_n = s$$ and $$\lim b_n = s$$ for some real number $$s$$, then $$s_n$$ is a convergent sequence and also converges to $$s$$.

## Problem 3

a) Give the definition of a bounded set

A set $$A$$ is bounded if it is bounded above and bounded below, ie. if there exist real numbers $$m$$ and $$M$$ with $$m \leq x\leq M$$ for all $$x\in A$$.

b) Is the set

$$\left\lbrace\frac{1}{x^2-3}: x\in\mathbb Q\right\rbrace$$

bounded?  Carefully justify your answer.

The set is not bounded.
To see this, assum otherwise.
Then the set is bounded above by some number $$M > 0$$.
By density of the rationals, there exists a rational number $$x$$ with

$$\sqrt{3} < x < \sqrt{3 + \frac{1}{M}}.$$

It follows that

$$0 < x^2-3 < \frac{1}{M}$$

and therefore $$\frac{1}{x^2-3} > \frac{1}{M}$$.  This is a contradiction.

## Problem 4

Consider the sequence $$(s_n)$$ defined by

$$s_n = \frac{2n^2+3}{n^2+2n}.$$

a) Determine the limit of the sequence.

The limit of the sequence is $$2$$.

b) Carefully prove that the limit you found in (a) is correct by using the $$\epsilon,N$$-definition of a limit directly.

Let $$\epsilon > 0$$.
Choose $$N = 4/\epsilon$$.
Then for any natural number $$n > N$$ we have

$$\lvert s_n-2\rvert = \lvert \frac{3-4n}{n^2+2n}\rvert = \frac{4n-3}{n^2+2n} < \frac{4n}{n^2+2n} < \frac{4n}{n^2} = \frac{4}{n} < \frac{4}{N} = \epsilon.$$

Since $$\epsilon > 0$$ was arbitrary, this proves $$\lim s_n = 2.$$

## Problem 5

For any subset $$A\subseteq\mathbb{R}$$, define $$-A = \{-x: x\in A\}.$$

a) Suppose that $$A$$ is bounded.  Define the supremum of $$A$$.

The supremum of $$A$$ is a number which is an upper bound for a and which is less than or equal to any upper bound of $$A$$.
Put another way, $$\sup(A)$$ is a number satisfying two properties:
* $$\sup(A) \geq x$$ for all $$x\in A$$
* if $$L \geq x$$ for all $$x\in A$$ then $$L\geq \sup(A)$$

b) Prove that $$\sup(-A) = -\inf(A)$$ and $$\inf(-A)=-\sup(A)$$.
Note that

$$\inf(-A)\leq -a\leq \sup(-A)\ \forall\ a\in A.$$

Multiplying everything by $$-1$$, we get 

$$-\sup(-A)\leq a\leq -\inf(-A) \forall\ a\in A.$$

This makes $$-\sup(-A)$$ a lower bound for $$A$$ and $$-\inf(-A)$$ an upper bound for $$A$$.  Therefore

$$-\sup(-A)\leq \inf(A)\leq\sup(A)\leq-\inf(-A)$$.

The same inequality works for any set $$A$$, so it also works if we switch our initial set $$A$$ with $$-A$$.  This gives the inequality

$$-\sup(A)\leq \inf(-A)\leq\sup(-A)\leq-\inf(A)$$.

Combining these two inequalities, we obtain $$\sup(-A)=-\inf(A)$$ and $$\inf(-A)=-\sup(A)$$.



## Problem 6

Define a sequence $$(s_n)$$ recursively by letting $$s_1 = 3$$ and more generally

$$s_{n+1} = \frac{1}{2}s_n +\frac{3}{2s_n}.$$

a) Prove that the sequence is monotone.

We first use induction to prove that $$s_n$$ is positive for all $$n\in\mathbb{N}$$.
Our base case is obvious since $$s_1 = 3 > 0$$.
As an inductive assumption, suppose that $$s_n>0$$.
Then $$s_{n+1}$$ is the sum of two positive numbers and therefore positive.
Thus by PMI, $$s_n$$ is positive for all $$n$$.

Next note that for any $$n\in\mathbb{N}$$, 

$$s_{n+1}-\sqrt{3} = \frac{1}{2}s_n +\frac{3}{2s_n} - \sqrt{3} = \frac{s_n^2-2s_n\sqrt{3} + 3}{2s_n} = \frac{(s_n-\sqrt{3})^2}{2s_n} > 0.$$
Thus $$s_{n}-\sqrt{3}>0$$ for all $$n\in\mathbb{N}$$.

Then we calculate

$$s_{n}-s_{n+1} = \frac{1}{2}s_n-\frac{3}{2s_n} = \frac{s_n^2-3}{2s_n} > 0.$$

This proves that the sequence is monotone decreasing.


b) Prove that the sequence converges.

It's monotone decreasing and bounded below by $$0$$, so it converges.

c) Determine the limit of the sequence.

Let's let $$s$$ be the limit.  Taking the limit of both sides of the update equation

$$s_{n+1} = \frac{1}{2}s_n +\frac{3}{2s_n}$$

we get

$$s = \frac{1}{2}s + \frac{3}{2s}.$$


This simplifies to $$s^2-3=0$$ so $$s=\sqrt{3}$$ or $$s=-\sqrt{3}$$.
Since the limit of a positive sequence cannot be negative, it follows that the limit is $$\sqrt{3}$$.

## Problem 7

Suppose that $$(s_n)$$ is a bounded sequence of real numbers (not necessarily convergent) and that $$t_k = s_{n_k}$$ is a convergent subsequence.

a) Define $$\limsup s_n$$ and explain why it is well-defined

It is defined by

$$\limsup s_n = \lim_{N\rightarrow\infty} M_N,\ \ \text{for} M_N = \sup\{s_n: n\geq N\}.$$

Each of these sets is bounded, and therefore has a supremum by the Completeness Axiom.
Therefore the sequence $$M_N$$ is well-defined.
The sequence $$M_N$$ is monotone decreasing and bounded below by the lower bound of the sequence $$(s_n)$$, so it converges.  Thus its limit, $$\limsup s_n$$, is well-defined.

b) Prove that

$$\lim t_k\leq \limsup s_n.$$

We have that $$t_k\leq M_{n_k}$$ for all $$k$$.  The sequence $$M_{n_k}$$ is a subsequence of the convergent sequence $$(M_N)$$ and therefore converges to $$\limsup s_n$$.
Therefore by taking the limit of both sides, we find

$$\lim t_k\leq \lim M_{n_k} = \limsup s_n.$$




