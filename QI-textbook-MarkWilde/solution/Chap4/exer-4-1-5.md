## Exercise 4.1.5

For ensemble $\{\{1/2, |0\rangle\}, \{1/2, |1\rangle\}\}$, the corresponding density matrix is given by
$$
\begin{align}
\rho &= \sum_{x}p_{X}(x)|\psi_x\rangle\langle \psi_x| = \frac{1}{2}|0\rangle\langle 0| + \frac{1}{2}|1 \rangle\langle 1|\\
&= \frac{1}{2}\begin{pmatrix}
1 \\ 0 
\end{pmatrix} \begin{pmatrix}
1 & 0 
\end{pmatrix} + \frac{1}{2}\begin{pmatrix}
0 \\ 1 
\end{pmatrix} \begin{pmatrix}
0 & 1
\end{pmatrix} \\

&= \frac{1}{2}\begin{pmatrix}
1 & 0 \\ 0 & 0 
\end{pmatrix} + \frac{1}{2}\begin{pmatrix}
0 & 0 \\ 0 & 1
\end{pmatrix} =\frac{1}{2}\begin{pmatrix}
1 & 0 \\ 0 & 1
\end{pmatrix} \\
\end{align}\tag{1}\label{1}
$$
For ensemble $\{\{1/2, |+\rangle\}, \{1/2, |-\rangle\}\}$,  the corresponding density matrix is given by
$$
\begin{align}
\rho &= \sum_{x}p_{X}(x)|\psi_x\rangle\langle \psi_x| = \frac{1}{2}|+\rangle\langle +| + \frac{1}{2}|- \rangle\langle -|\\
&= \frac{1}{4}\begin{pmatrix}
1 \\ 1 
\end{pmatrix} \begin{pmatrix}
1 & 1 
\end{pmatrix} + \frac{1}{4}\begin{pmatrix}
1 \\ -1 
\end{pmatrix} \begin{pmatrix}
1 & -1
\end{pmatrix} \\

&= \frac{1}{4}\begin{pmatrix}
1 & 1 \\ 1 & 1 
\end{pmatrix} + \frac{1}{4}\begin{pmatrix}
1 & -1 \\ -1 & 1
\end{pmatrix} \\

&=\frac{1}{4}\begin{pmatrix}
2 & 0 \\ 0 & 2
\end{pmatrix}=\frac{1}{2}\begin{pmatrix}
1 & 0 \\ 0 & 1
\end{pmatrix} \\
\end{align}\tag{2}\label{2}
$$
From eq. $\eqref{1}$ and eq. $\eqref{2}$, we see that two ensembles have same density operator. 
