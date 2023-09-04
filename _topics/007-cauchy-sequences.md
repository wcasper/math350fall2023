---
layout: page
title: Cauchy Sequences
---

In mathematics, a Cauchy sequence is a sequence whose terms are getting closer and closer together.
One of the most important properties of the real numbers is that Cauchy sequences converge.
The significance of this is a bit harder to appreciate when we are focused on the real numbers only.
For other collections of numbers, or more generally in the context of metric spaces Cauchy sequences do not necessarily converge.
When they do, it is a special property called **completeness**, which indicates that the space has no missing points (from a certian point of view).

**Definition:** A sequence of real numbers $$(s_n)$$ is called a **Cauchy sequence** if for all $$\epsilon > 0$$ there exists a real number $$N$$ with 

$$m,n > N\ \Longrightarrow $$\lvert s_m-s_n\rvert < \epsilon.$$

**Lemma:** Convergent sequences are cauchy.

**Proof:** Suppose that $$(s_n)$$ is a convergent sequence, with limit $$s$$.  Then for all $$\epsilon > 0$$ there exists $$N$$ with $$n > N$$ implying $$\lvert s_n-s\rvert < \epsilon / 2$$.

Thus for $$m,n > N$$ we have

$$\lvert s_m-s_n\rvert = \lvert s_m-s+s-s_n\rvert \leq \lvert s_m-s\rvert + \lvert s-s_n\rvert < \epsilon/2 + \epsilon/2 = \epsilon$$.


**Lemma:** Cauchy sequences are bounded.

**Proof:**  Suppose that $$(s_n)$$ is a Cauchy sequence.  Then there exists an $$N$$ such that $$m,n > N$$ implies $$\lvert s_n-s_m\rvert < 1.$$

This implies that if $$n > N$$ then we have

$$\lvert s_n\lvert = \lvert s_n-s_{N+1} + s_{N+1}\rvert  \leq \lvert s_n-s_{N+1}\rvert + \lvert s_{N+1}\rvert < 1 + \lvert s_{N+1}\rvert.$$

Thus for all integers $$n > 0$$ we know $$\lvert s_n\rvert \leq k$$ for 

$$k = \max\{\lvert s_1 \rvert, \lvert s_2\rvert ,\dots, \lvert s_N\rvert ,\lvert s_{N+1}\rvert +1\}.$$

In particular the sequence is bounded.
:black_square_button:


**Theorem:** A sequence $$(s_n)$$ of real numbers converges if and only if it is Cauchy.

**Proof:**

We have already shown that convergent sequences are Cauchy, so it suffices to show the converse.

Suppose that $$(s_n)$$ is a Cauchy sequence.
Then $$(s_n)$$ is bounded and therefore $$\liminf s_n$$ and $$\limsup s_n$$ are well-defined.
Thus to prove convergence, it suffices to show $$\liminf s_n = \limsup s_n$$.

Let $$\epsilon > 0$$.
Since $$(s_n)$$ is Cauchy, we can choose $$N$$ such that $$m,n > N$$ implies $$\lvert s_m-s_n\rvert < \epsilon$$.
This implies that for all $$m, n >N$$ we have $$s_n < s_m + \epsilon$$.
Consequently for all $$m\geq N$$ we have 

$$\limsup s_n < s_m +\epsilon$$

Hence 

$$\limsup s_n < \liminf s_n +\epsilon$$

Since $$\epsilon$$ was arbitrary, it follows that $$\limsup s_n \leq \liminf s_n$$.
Since $$\liminf s_n\leq \limsup s_n$$, we conclude that $$\liminf s_n = \limsup s_n$$.
:black_square_button:


