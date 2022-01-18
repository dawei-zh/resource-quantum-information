## Exercise 3.3.4

The Pauli matrix $Y$ in the computational basis is
$$
Y= \begin{pmatrix}
0 & -i\\ i &0
\end{pmatrix} \tag{1}\label{1}
$$
The eigenvalue $\lambda$ of $Y$​ is the solution of the following equation,
$$
|Y - \lambda I|= \begin{vmatrix}
-\lambda & -i \\ i & -\lambda 
\end{vmatrix} = \lambda^2 - 1 = 0 \iff \lambda = \pm 1\tag{2}
$$
The corresponding eigenstates are given by
$$
\begin{align}
Y|v_1\rangle &= \begin{pmatrix}
0 & -i\\ i &0
\end{pmatrix}\begin{pmatrix}
a \\ b
\end{pmatrix} = \begin{pmatrix}
a \\ b
\end{pmatrix} \iff |v_1\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ i
\end{pmatrix} \tag{3a}\\

Y|v_2\rangle &= \begin{pmatrix}
0 & -i\\ i &0
\end{pmatrix}\begin{pmatrix}
c \\ d
\end{pmatrix} = -\begin{pmatrix}
c \\ d
\end{pmatrix} \iff |v_2\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ -i
\end{pmatrix}\tag{3b}
\end{align}
$$
