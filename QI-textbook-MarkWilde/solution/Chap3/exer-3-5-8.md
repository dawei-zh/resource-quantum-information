## Exercise 3.5.8

Following the proof of no-cloning theorem, we can also prove the no-deletion theorem. Suppose for a contradiction that there exists an operator $U$ such that
$$
\begin{align}
U|\psi\rangle|\psi\rangle|A\rangle &= |\psi\rangle|0\rangle|A'\rangle \\
&= (\alpha|0\rangle + \beta|1\rangle) |0\rangle|A'\rangle
\end{align}\tag{1}\label{1}
$$
 Since the deletion is universial, it also deletes the state $|0\rangle$ and $|1\rangle$, 
$$
\begin{align}
U|0\rangle|0\rangle|A\rangle &= |0\rangle|0\rangle|A_0\rangle \\
U|1\rangle|1\rangle|A\rangle &= |1\rangle|0\rangle|A_1\rangle
\end{align}\tag{2}\label{2}
$$
Due to the linearity of quantum theory, from eq. $\eqref{2}$ we then have for a superposition state $\alpha|0\rangle + \beta|1\rangle$ as 
$$
\begin{align}
U|\psi\rangle|\psi\rangle|A\rangle &= U(\alpha|0\rangle + \beta|1\rangle)(\alpha|0\rangle + \beta|1\rangle)|A\rangle  \\
&= U(\alpha^{2}|0\rangle|0\rangle + \alpha\beta|0\rangle|1\rangle + \alpha\beta|1\rangle|0\rangle + \beta^2|1\rangle|1\rangle)|A\rangle \\
&= \alpha^{2}U|0\rangle|0\rangle|A\rangle + \alpha\beta U|0\rangle|1\rangle|A\rangle + \alpha\beta U|1\rangle|0\rangle|A\rangle + \beta^2 U|1\rangle|1\rangle|A\rangle \\
&= \alpha^{2}|0\rangle|0\rangle|A_0\rangle + \alpha\beta U|0\rangle|1\rangle|A\rangle + \alpha\beta U|1\rangle|0\rangle|A\rangle + \beta^2 |1\rangle|0\rangle|A_1\rangle
\end{align}\tag{3}\label{3}
$$
Compare eq. $\eqref{1}$ and eq. $\eqref{3}$​, we find that these two equations will not equal for all cases, since we have in general case, 
$$
\alpha^{2}|0\rangle|0\rangle|A_0\rangle + \alpha\beta U|0\rangle|1\rangle|A\rangle + \alpha\beta U|1\rangle|0\rangle|A\rangle + \beta^2 |1\rangle|0\rangle|A_1\rangle \neq \alpha|0\rangle |0\rangle|A'\rangle+ \beta|1\rangle |0\rangle|A'\rangle\tag{4}
$$
Thus, our result contradicts the existence of a universal quantum deletion. 
