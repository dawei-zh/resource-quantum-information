## Exercise 2.2.1

Suppose that for message $m\in [M]$ and a certain code $\mathcal{C}$, we have following relation
$$
\bar{p}_e = \frac{1}{M} \sum_{m} p_{e}(m, \mathcal{C}) \leq \epsilon \tag{1}\label{1}
$$
Let random variable $X = \{p_{e}(m, \mathcal{C})\}$ with size $M$, the expectation value of random variable $X$ is given by
$$
E(X) = \frac{1}{M}\sum_{m} p_{e}(m, \mathcal{C}) = \bar{p}_{e} \leq \epsilon \tag{2}
$$
In this problem, we need to prove that whether there is at least half of message $m$ with $p_{e}\leq 2\epsilon$, that is, we need to prove that the probability of getting $X\leq 2\epsilon$ is at least $1/2$​. According to the Markov's inequality, we have
$$
P(X\geq 2\epsilon) \leq \frac{E(X)}{2\epsilon} = \frac{1}{2}\tag{3}
$$
Equivalently, we have
$$
P(X\leq 2\epsilon) = 1 - P(X\geq 2\epsilon)  \geq  \frac{1}{2}\tag{4}\label{4}
$$
Namely, we conclude from eq. $\eqref{4}$ that if we have eq. $\eqref{1}$, we should have at least half of the message $m$ satisfies the condition $p_{e}(m,\mathcal{C}) \leq 2\epsilon$. 
