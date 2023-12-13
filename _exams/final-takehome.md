---
layout: page
title: Final Exam Takehome Portion
permalink: /exams/final-takehome
---

Solve each of the following problems.
Do **not** consult with online resources or other students or faculty.
You may use your book and your notes.
If the problem asks for a proof, be sure to carefully justify your work, including any theorems from class.

Note: you may NOT use a theorem or result from class to prove something when it makes the problem entirely trivial.  If you are unsure whether a particular theorem or result is allowed, just ask!

## Problem 1

Suppose that $$(f_n(x))$$ is a sequence of functions which are differentiable on every point in $$\mathbb{R}$$.

Suppose that the sequence converges pointwise on $$[a,b]$$ to a function $$f(x)$$ and that the sequence of derivatives $$f_n'(x)$$ converge *uniformly* on $$[a,b]$$ to a function $$g(x)$$. Prove that $$f(x)$$ is differentiable on $$(a,b)$$ and $$f'(x) = g(x)$$ for all $$x\in (a,b)$$.


## Problem 2

Suppose that $$g(x)$$ is a nonnegative, integrable function on $$[a,b]$$ and that

$$f(x) = \left\lbrace\begin{array}{cc}
g(x), & x \in \mathbb{Q}\\
0, & x\notin \mathbb{Q}
\end{array}\right.$$

Prove that $$U(f) = \int_a^b g(x)dx.$$

**Hint:** Try writing out the expressions for $$U(f,P)$$ and $$U(g,P)$$ for any parition $$P$$.  How do they compare?

## Problem 3

Let $$E = \{1/n^2: n\in\mathbb{N}\}$$.  Consider the function

$$f(x) = \left\lbrace\begin{array}{cc}
1, & x \in E\\
0, & x\notin E
\end{array}\right.$$

Determine if $$f(x)$$ is Riemann integrable on $$[0,1]$$, and if so what it's Darboux integral is.
Carefully justify your work.

**Hint:** Try choosing a partition whose points are very close to the elements of $$E$$.
For example, let $$0 < \epsilon < 1$$ and consider the partition

$$P = \left\lbrace \frac{1-\epsilon/(n+1)^2}{n^2}: n\in\mathbb{N}\right\rbrace\cup \left\lbrace \frac{1+\epsilon/(n+1)^2}{n^2}: n\in\mathbb{N}\right\rbrace$$

What is $$U(f,P)$$ for his partition?  As $$\epsilon$$ gets smaller, what does that imply about the infimum over all partitions $$U(f)$$?

