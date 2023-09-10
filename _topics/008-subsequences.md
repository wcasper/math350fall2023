---
layout: page
title: Subsequences
---

**Definition:** A **subsequence** of a sequence $$(s_n)$$ is a sequence $$(t_n)$$ satisfying $$t_k = s_{n_k}$$ for some sequence of positive integers $$n_1,n_2,\dots$$ satisfying $$n_k\leq n_{k+1}$$ for all $$k$$.

Our typical primary question about sequences is convergence.
Likewise, we are interested in the convergence of subsequences of sequences.

**Theorem:** A sequence $$(s_n)$$ converges to $$s$$ if and only if every subsequence of $$(s_n)$$ also converges to $$s$$.
**Proof:**

The sequence itself is a subsequence, so clearly if every subsequence converges to $$s$$, then $$(s_n)$$ also converges to $$s$$.
Conversely, suppose that $$(s_n)$$ converges to $$s$$ and let $$t_k=s_{n_k}$$ be a subsequence.

Let $$\epsilon > 0$$.
Then there exists $$N$$ such that $$n\geq N$$ implies $$\lvert s_n-s\rvert < \epsilon$$.
Furthermore, since the sequence $$n_k$$ diverges to $$\infty$$, there exists $$M$$ such that $$k\geq M$$ implies $$n_k > N$$.
Consequently when $$k > M$$ we have $$\lvert t_k-s\rvert < \epsilon.$$

:black_square_button:

For some results, it is helpful to restrict our attention to monotonic sequences for certain nice behavior.
We can use subsequences to achieve this.

**Theorem (Monotone Subsequence Theorem):**  Any sequence $$s_n$$ has a monotonic subsequence.

**Proof:**

Consider the set $$A = \{n\in\mathbb N: s_n\geq s_k\ \forall k > n\}$$.
Suppose that $$A$$ is infinite.
Then we can choose a subsequence $$t_k = s_{n_k}$$ with $$n_k$$ in $$A$$ for all $$k$$.  By definition, this will be a monotone decreasing sequence.

Alternatively, suppose $$A$$ is finite.
Then choose $$N_0$$ such that $$s_n\notin A$$ for all $$n>N_0$$.
Let $$t_1 = N_0+1$$.
Then for each $$k$$ define $$t_k$$ recursively by selecting $$t_{k+1} > t_k$$ and $$s_{t_{k+1}} > s_{t_k}$$ (which exists since $$t_k\notin A$$.
Then $$(t_k)$$ is a monotone increasing sequence.

:black_square_button:


**Corollary:** Let $$(s_n)$$ be a sequence with a subsequence converging to $$t$$.  Then $$(s_n)$$ has a monotonic subsequence converging to $$t$$.  The same is true if we replace converging with diverging to $$\pm\infty$$.

**Proof:**
Immediataely follows from the previous two theorems.
:black_square_button:

One of the most important fundamental results about subseqeuences is the following.

**Theorem (Heine-Borel Theorem):** Every bounded sequence has a convergent subsequence.

**Proof:**  If $$(s_n)$$ is a bounded sequence, then it has a monotone subsequence.  Since bounded monotone sequences converge, this subsequence will converge.
:black_square_button:


### Limits of subsequences

From the above, we know that bounded sequences have convergent bounded subsequences.
One important question is what values such subsequences converge to.

**Theorem:**

Let $$(s_n)$$ be a sequence.
* (a) Let $$t$$ be a real number.  There is a subsequence of $$(s_n)$$ converging to $$t$$ if and only if $$\{n\in\mathbb{N}: \lvert s_n-t\rvert < \epsilon\}$$ is an infinite set for all $$\epsilon>0$$.
* (b) The sequence $$(s_n)$$ is unbounded above if and only if there is a subsequence diverging to $$\infty$$.
* (c) The sequence $$(s_n)$$ is unbounded below if and only if there is a subsequence diverging to $$-\infty$$.

**Proof:**

* (a)  Suppose $$t$$ is a real number and $$(s_n)$$ has a subsequence converging to $$t$$.
Then for all $$\epsilon > 0$$, there exists an integer $$N$$ such that

$$\{n\in \mathbb{N}: n\geq N\}\subseteq\{n\in\mathbb{N}: \lvert s_n-t\rvert < \epsilon\}.$$

In particular, the set is infinite.
Conversely, suppose that $$\{n\in\mathbb{N}: \lvert s_n-t\rvert < \epsilon\}$$ is infinite for all $$\epsilon > 0$$.
Then let $$n_1=1$$ and for each integer $$k\geq 1$$, choose $$n_{k+1}$$ recusively by 

$$n_{k+1}\in \{n\in\mathbb{N}: \lvert s_n-t\rvert < 1/k,n_{k+1}\geq n_k\}.$$

This is well-defined, since the set on the right hand side is infinite and never empty.  Then by definition $$\lvert s_{n_k}-t\rvert < 1/k$$ for all $$k > 1$$, and it follows that $$s_{n_k}$$ converges to $$t$$.

* (b)  Clearly, if there is a subsequence diverging to $$\infty$$, then the sequence cannot be bounded above.  Conversely, suppose $$(s_n)$$ is not bounded above. 
Then let $$n_1=1$$ and for each integer $$k\geq 1$$, choose $$n_{k+1}$$ recusively by 

$$n_{k+1}\in \{n\in\mathbb{N}: s_n > k,n_{k+1}\geq n_k\}.$$

This is well-defined, since otherwise the sequence would be bounded.  Then $$s_{n_k} > k$$ for all $$k$$ and therefore the subsequence diverges to infinity.

* (c) Apply (b) and linearity to the sequence $$(-s_n)$$.

:black_square_button:


**Theorem:**

Let $$(s_n)$$ be any sequence.
Then there exist subsequences converging monotonically to $$\limsup s_n$$ and $$\liminf s_n$$.

**Proof:**
We will prove this for $$\limsup s_n$$, since the proof for $$\liminf s_n$$ is similar.
It suffices to prove that we have subsequences converging to $$\limsup s_n$$ and $$\liminf s_n$$, since by selecting a further subsequence we can make the convergence monotonic.
if $$(s_n)$$ is not bounded above, then $$\limsup s_n=\infty$$ and the result is true by the previous problem.
Therefore assume $$s_n$$ is bounded above.
If $$\limsup s_n = \pm\infty$$, then this is a consequence of the previous theorem.  Therefore assume otherwise.

Then the sequence $$M_N = \sup\{s_n: n\geq N\}$$ converges to $$M := \limsup s_n$$.
Therefore for each $$k$$ there exists an integer $$N_k$$ such that $$\lvert M_{N_k}-M\rvert < \frac{1}{2k}$$, and we can take $$N_k > k$$.
Furthermore, we can choose $$m_k\geq N_k$$ such that $$s_{m_k}>M_{m_k}-\frac{1}{2k}$$.
This implies

$$\lvert s_{m_k}-M\rvert = \lvert s_{m_k}-M_{N_k}+M_{N_k}-M\rvert \leq M_{N_k}-s_{m_k} +\lvert M_{N_k}-M\rvert < \frac{1}{k}.$$

Since $$m_k \geq N_k > k$$, the sequence $$(m_k)$$ diverges to infinity, so we can choose a subsequence $$n_j = m_{k_j}$$ satisfying $$n_{j+1} > n_j$$ for all $$j$$.
The sequence $$(s_{m_k})$$ converges to $$M$$, so the subsequence $$s_{n_j}$$ does too.  

:black_square_button:


**Theorem:**

Let $$(s_n)$$ be any sequence.
If $$t$$ is the limit of a convergent subsequence of $$(s_n)$$ then

$$\liminf s_n\leq t\leq \limsup s_n.$$


