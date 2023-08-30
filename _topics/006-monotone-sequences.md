---
layout: page
title: Monotone sequences
---

## Basics

**Definition:**  A sequence $$(s_n)$$ is called **monotone increasing** or **increasing** if $$s_{n+1}\geq s_n$$ for all $$n\in\mathbb N$$.  A sequence $$(s_n)$$ is called **monotone decreasing** or **decreasing** if $$s_{n+1}\leq s_n$$ for all $$n\in\mathbb N$$.  In either case, we call the sequence a **monotone sequence**.

**Theorem:** A bounded monotone sequence converges.

**Proof:**

Suppose that $$(s_n)$$ is a monotone increasing bounded sequence.  Then the set $$A = \{s_n: n\in\mathbb N\}$$ is bounded above, and thus has a supremum $$s$$ by the completeness axiom.

Let $$\epsilon > 0$$.  Then $$s-\epsilon$$ is less than $$s$$ and therefore not an upper bound of $$A$$.  In particular there must exists an integer $$N$$ such that $$s_N > s-\psilon$$.
It follows that for any $$n\geq N$$ we have $$s_n\geq s_N>s-\epsilon$$ and therefore

$$\lvert s_n-s\rvert = s-s_n  < \epsilon.$$

Since $$\epsilon > 0 $$ was arbitrary, it follows that $$\lim s_n = s$$.

The proof for a monotone decreasing sequence follows from applying the previous result to $$(-s_n)$$ and using linearity properties of limits.
:black_square_button:

For unbounded sequences, we have another nice result.

**Theorem:** Unbounded monotone increasing sequences diverge to $$\infty$$ and unbounded monotone decreasing sequences diverge to $$-\infty$$.

**Proof:**

Can you try to prove this?
:black_square_button:

In particular, this means if $$(s_n)$$ is monotone the expression $$\lim s_n$$ will always make sense, either as a real number or as an extended real number, since if the sequence doesn't converge it must continue to get arbitrarily large.


## Decimal expansions

As a special case of this, we have **decimal expansions**.

**Definition:** Let $$K$$ be an arbitrary nonnegative integer and $$d_1,d_2,\dots$$ be single-digit positive integers.  By the expression

$$K.d_1d_2d_3d_4d_5\dots$$

we mean the limit of the monotone increasing sequence of partial sums

$$\lim_{n\rightarrow\infty} \left(K + \frac{d_1}{10} + \frac{d_2}{10} + \dots\right)$$

which exists by the rsult of the previous Lemma!


**Theorem:** Every real number can be expressed as a **decimal expansion**, but this expansion is not necessarily unique.
**Proof:** Can you prove this?  Can you find non-unique examples?
:black_square_button:


## Lim sup and lim inf

Given any sequence, we can 

**Definition:** We define 


