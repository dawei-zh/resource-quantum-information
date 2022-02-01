## Exercise 3.5.4

Consider a two-qubit operation as $H_1H_2({\rm CNOT})H_1H_2$, if we have for CNOT gate, 
$$
{\rm CNOT} = |0\rangle\langle 0|\otimes I + |1\rangle \langle 1|\otimes X\tag{1}
$$
and for the two-qubit Hadmard gate, $H_1H_2 = H\otimes H$, the given operation can be re-written as
$$
\begin{align}
H_1H_2({\rm CNOT})H_1H_2 &= (H\otimes H)(|0\rangle\langle 0|\otimes I + |1\rangle \langle 1|\otimes X)(H\otimes H) \\
&= (H\otimes H)(|0\rangle\langle 0|H\otimes IH + |1\rangle \langle 1|H\otimes XH) \\
&= H|0\rangle\langle 0|H\otimes HIH + H|1\rangle \langle 1|H\otimes HXH
\end{align}\tag{2}\label{2}
$$
For the Hadmard gate, 
$$
H= \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix}\tag{3}\label{3}
$$
we could see that $H$ is a Hermitian operator, $H^{\dagger} = H$. Also, we could have $HXH = Z$ and 
$$
HIH= HH = \frac{1}{2}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} = \frac{1}{2}\begin{pmatrix}
2 & 0 \\ 0 & 2
\end{pmatrix} = I\tag{4}\label{4}
$$
When Hadmard gate peforms on computational basis, we have
$$
\begin{align}
H|0\rangle &= \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix}\begin{pmatrix}
1 \\0
\end{pmatrix} = \frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\1
\end{pmatrix} = |+\rangle  \\

H|1\rangle &= \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix}\begin{pmatrix}
0 \\ 1
\end{pmatrix} = \frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ -1
\end{pmatrix} = |-\rangle
\end{align}\tag{5}\label{5}
$$
Using eq. $\eqref{4}-\eqref{5}$, and the given properties of Hadmard gate above, we could simplify eq. $\eqref{2}$ as
$$
\begin{align}
H_1H_2({\rm CNOT})H_1H_2 &= H|0\rangle\langle 0|H\otimes HIH + H|1\rangle \langle 1|H\otimes HXH \\
&= (H|0\rangle)(\langle 0|H^{\dagger})\otimes I + (H|1\rangle)(\langle 1|H^{\dagger})\otimes Z \\
&= |+\rangle\langle +|\otimes I + |-\rangle\langle -|\otimes Z
\end{align}\tag{6}
$$
