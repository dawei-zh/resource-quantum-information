## Exercise 2.1.1

For a given information source $\{x\in \mathcal{X}, p(x)\}$, the entropy $H(X)$ is given by
$$
H(X) = -\sum_{x\in\mathcal{X}} p_{X}(x)\log p_{X}(x)\tag{1} \label{1}
$$ { }
For a certain information source with each variable $x_{i}$​ is uniformly random, the probability distribution is 
$$
p(x_{i}) = \frac{1}{|\mathcal{X}|}\text{ for all }x_{i}\in \mathcal{X} \tag{2}\label{2}
$$
where $|\mathcal{X}|$ is the size of the variable's alphabet. Substitute eq. $\eqref{2}$ into eq. $\eqref{1}$, we get the entropy for the uniform random variable as
$$
\begin{align}
H(X) &= -\sum_i{}\frac{1}{|\mathcal{X}|}\log \left(\frac{1}{|\mathcal{X}|}\right) \\
&= -|\mathcal{X}|\cdot\frac{1}{|\mathcal{X}|}\log \left(\frac{1}{|\mathcal{X}|}\right) \\
&= -\log \left(\frac{1}{|\mathcal{X}|}\right) = \log|\mathcal{X}|
\end{align}\tag{3}
$$
