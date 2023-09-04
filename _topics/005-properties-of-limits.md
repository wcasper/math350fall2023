---
layout: page
title: Properties of limits
---

Back in calculus, we learned several important properties of sequences, which we now wish to prove.


## Algebraic properties

**Theorem (Linearity of Limits):**

Let $$(s_n)$$ and $$(t_n)$$ be two convergent sequences and let $$k$$ be any real number.  Then the following are true.

1. $$\lim (ks_n) = k\lim s_n.$$
2. $$\lim (s_n+t_n) = \lim s_n + \lim t_n.$$

**Proof:**
For sake of clarity, we set $$s=\lim s_n$$ and $$t=\lim t_n$$.

First we will prove (1).
Let $$\epsilon > 0$$.
If $$k=0$$, the statement is obvious, so we will assume otherwise.
Then there exists $$N$$ such that whenever $$n>N$$ we have $$\lvert s_n-s\rvert < \epsilon/\lvert k\rvert.$$
It follows that 

$$\lvert ks_n-ks\rvert \leq k\lvert s_n-s\rvert < k\epsilon/\lvert k\rvert \leq \epsilon. $$

Since $$\epsilon$$ was arbitrary, we conclude that $$\lim (ks_n) = ks$$.

Now we will prove (2).
Let $$\epsilon > 0$$.
Then there exist $$M$$ and $$N$$ with both $$n>M$$ implying $$\lvert s_n-s\rvert < \epsilon/2$$ and $$n>N$$ implying $$\lvert t_n-t\rvert < \epsilon/2$$.
It follows from the triangle inequality that for $$n > \max(M,N)$$

$$\lvert s_n+t_n-(s+t)\rvert \leq \lvert s_n-s\rvert + \lvert t_n-t\rvert < \epsilon/2+\epsilon/2 = \epsilon.$$

Since $$\epsilon$$ was arbitrary, we conclude that $$\lim (s_n+t_n) = s+t$$.
:black_square_button:

To prove some further results, we will rely on the following lemma.

**Lemma:** Let $$(s_n)$$ be a convergent sequence.  Then there exists a number $$k>0$$ with $$\lvert s_n\rvert \leq k$$ for all $$n\in\mathbb N$$.

**Proof:**  Let $$s=\lim s_n$$.  Then there exists an $$N$$ such that for $$n > N$$ we have $$\lvert s_n-s\rvert < 1$$.

Define

$$k = \max\{\lvert s_1\rvert ,\lvert s_2\rvert ,\dots, \lvert s_N\lvert , 1+\lvert s\rvert\}.$$

Then if $$n\leq N$$ we have $$\lvert s_n\rvert \leq k$$.
Alternatively, if $$n>N$$ then the triangle inequality tells us

$$\lvert s_n\rvert = \lvert s_n-s+s\rvert \leq \lvert s_n-s\rvert + \lvert s\rvert\leq 1 + \lvert s\rvert \leq k$$.

:black_square_button:

**Defintion:** A sequence satisfying the conclusion of the previous lemma is called **bounded**.

**Theorem (Product Law for Limits):**

Let $$(s_n)$$ and $$(t_n)$$ be two convergent sequences.  Then the limit of the products is the product of the limits, ie.

$$\lim(s_nt_n) = (\lim s_n)(\lim t_n).$$

**Proof:**

For sake of clarity, we set $$s=\lim s_n$$ and $$t=\lim t_n$$.

Let $$\epsilon > 0$$.

By the previous Lemma, we can choose $$k>0$$ with $$\lvert s_n\rvert \leq k$$ for all $$n$$.
Then there exist $$M$$ and $$N$$ with both $$n>M$$ implying $$\lvert s_n-s\rvert < \frac{\epsilon}{2\lvert t\rvert)}$$ (or $$ < \epsilon/2 $$ if $$t=0$$) and $$n>N$$ implying $$\lvert t_n-t\rvert < \epsilon/2k$$.

Then the triangle inequality tells us that for $$n > \max(M,N)$$

$$\begin{align}
\lvert s_nt_n - st\rvert
  & = \lvert s_nt_n-s_nt+s_nt-st \rvert\\
  & \leq \lvert s_nt_n-s_nt \rvert + \lvert s_nt-st \rvert\\
  & \leq \lvert s_n\rvert\cdot \lvert t_n-t \rvert + \lvert s_n-s \rvert\cdot\lvert t\rvert\\
  & \leq k\cdot \lvert t_n-t \rvert + \lvert s_n-s \rvert\cdot\lvert t\rvert\\
  & < \epsilon/2 + \epsilon/2 = \epsilon.
\end{align}$$

Since $$\epsilon$$ was arbitrary, we conclude that $$\lim (s_nt_n) = st$$.
:black_square_button:



**Theorem (Quotient Law for Limits):**

Let $$(s_n)$$ and $$(t_n)$$ be two convergent sequences with $$t_n>0$$ for all $$n\in\mathbb N$$ and $$\lim t_n\neq 0$$.  Then the limit of the quotient is the quotient of the limits, ie.

$$\lim (s_n/t_n) = (\lim s_n)/(\lim t_n).$$

**Proof:**

For sake of clarity, we set $$s=\lim s_n$$ and $$t=\lim t_n$$.

We first prove that $$\lim 1/t_n = 1/t$$.

Let $$\epsilon > 0$$.

By our definition of convergence, there exists $$N_0$$ such that when $$n>N_0$$ we have $$\lvert t_n-t\rvert < \lvert t\rvert /2$$.
Consequently $$\lvert t_n\rvert > \lvert t\rvert /2$$, making $$1/\lvert t_nt\rvert  < 2/t^2$$.

Also there exists $$N_1>0$$ such that $$n>N_1$$ implies that $$\lvert t-t_n\rvert < \epsilon t^2/2$$.
As a consequence, when $$n>\max(N_0,N_1)$$

$$\lvert 1/t_n - 1/t \rvert  = \lvert t-t_n\rvert/\lvert t_nt \rvert < \epsilon$$

Since $$\epsilon$$ was arbitrary, we conclude that $$\lim (1/t_n) = 1/t$$.

Now for the more general case, we can apply the previous theorem to the product of sequences $$(s_n/t_n) = (s_n(1/t_n))$$.

:black_square_button:

**Theorem (Squeeze Theorem):**

Suppose that $$(s_n)$$, $$(t_n)$$ and $$(u_n)$$ are all sequences with $$s_n\leq t_n\leq u_n$$ for all but finitely many $$n$$.  Assume moreover that $$(s_n)$$ and $$(u_n)$$ converge to the same value.  Then  $$t_n$$ converges and

$$\lim s_n = \lim t_n = \lim u_n$$.

**Proof:**

Let $$L$$ be the limit of $$(s_n)$$ and let $$\epsilon > 0$$.

Then we can choose $$N_1$$ and $$N_2$$ with $$\lvert s_n-L\rvert < \epsilon/3$$ whenevery $$n> N_1$$ and $$\lvert u_n-L\rvert < \epsilon/3$$ whenever $$n > N/3$$.
Furthermore, we can choose $$N_3$$ with $$s_n\leq t_n\leq u_n$$ whenever $$n>N_3$$.

Therefore for $$n>\max(N_1,N_2,N_3)$$ we have $$s_n\leq t_n\leq u_n$$ we know

$$\begin{align}
\lvert t_n-L\rvert 
 & \leq \lvert t_n-s_n+s_n-L\rvert\\
 & \leq \lvert t_n-s_n \rvert + \lvert s_n-L\rvert\\
 & \leq \lvert u_n-s_n \rvert + \lvert s_n-L\rvert\\
 & \leq \lvert u_n-L+L-s_n \rvert + \lvert s_n-L\rvert\\
 & \leq \lvert u_n-L\rvert +\lvert L-s_n \rvert + \lvert s_n-L\rvert < \epsilon.
\end{align}$$

Since $$\epsilon$$ was arbitrary, this proves $$\lim t_n = L$$.

:black_square_button:


**Exercise:**  Try to prove that if $$(s_n)$$ is a convergent sequence of nonnegative numbers, then $$\lim s_n$$ is also nonnegative.


## Infinite limits

**Definition:** We say that the limit of a sequence **diverges to** infinity, and write $$\lim s_n = \infty$$, when for all $$M>0$$ there exists $$N$$ such that $$n\geq N$$ implies $$s_n>M$$.
We say that the limit of a sequence **diverges to** negative infinity, and write $$\lim s_n = -\infty$$, when for all $$M>0$$ there exists $$N$$ such that $$n\geq N$$ implies $$s_n < -M$$.
When a sequence converges or diverges to $$\infty$$ or $$-\infty$$, then the **limit of the sequence exists**.

**Theorem:**  Let $$(s_n)$$ and $$(t_n)$$ be two sequences with $$\lim s_n = \infty$$ and with $$\lim t_n > 0$$.  Then $$\lim s_nt_n = \infty$$.

**Theorem:**  Let $$(s_n)$$ be a sequence with $$s_n>0$$ for all $$n\in\mathbb N$$.  Then $$\lim s_n = \infty$$ if and only if $$\lim 1/s_n = 0$$.


