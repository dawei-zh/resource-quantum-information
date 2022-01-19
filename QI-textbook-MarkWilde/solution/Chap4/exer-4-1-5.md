## Exercise 4.1.5

For ensemble $\{\{1/2, |0\rangle\}, \{1/2, |1\rangle\}\}$​, the corresponding quantum state is given by
$$
|\psi\rangle = a|0\rangle + b|1\rangle \tag{1}\label{1}
$$
where $|a|^2 = |b|^2 = 1/2$. Note that $a$ and $b$ can be any complex number with its modulus as $1/2$. According to eq. $\eqref{1}$, the corresponding density matrix is given by
$$
\begin{align}
\rho &= |\psi\rangle\langle \psi| =(a|0\rangle + b|1\rangle)(a^{*}\langle 0| + b^{*}\langle 1| ) \\
&= |a|^2 |0\rangle\langle 0 | + ab^{*}|0\rangle\langle 1|+ a^{*}b|1\rangle\langle 0| + |b|^2 |1\rangle\langle 1|
\end{align}\tag{2}\label{2}
$$
For ensemble $\{\{1/2, |+\rangle\}, \{1/2, |-\rangle\}\}$, the corresponding quantum state is given by
$$
|\phi\rangle = c|+\rangle + d|-\rangle \tag{3}\label{3}
$$
where $|c|^2 = |d|^2 = 1/2$. Note that $c$ and $d$ can be any complex number with its modulus as $1/2$. According to eq. $\eqref{3}$, the corresponding density matrix is given by
$$
\begin{align}
\rho &= |\phi\rangle\langle \phi| =(c|+\rangle + d|-\rangle)(c^{*}\langle +| + d^{*}\langle -| ) \\
&= |c|^2 |+\rangle\langle + | + cd^{*}|+\rangle\langle -|+ c^{*}d|-\rangle\langle +| + |d|^2 |-\rangle\langle -|
\end{align}\tag{4}\label{4}
$$
Suppose that 
$$
|0\rangle = \begin{pmatrix}
1 \\ 0
\end{pmatrix}, |1\rangle = \begin{pmatrix}
0 \\ 1
\end{pmatrix}, |+\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ 1
\end{pmatrix}, |-\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ -1
\end{pmatrix}\tag{5}
$$
Eq. $\eqref{2}$ becomes
$$
\begin{align}
\rho &= |a|^2 \begin{pmatrix}1 & 0 \\ 0 & 0\end{pmatrix} + ab^{*}\begin{pmatrix}0 & 1 \\ 0 & 0\end{pmatrix}+ a^{*}b\begin{pmatrix}0 & 0 \\ 1 & 0\end{pmatrix}+ |b|^2 \begin{pmatrix}0 & 0 \\ 0 & 1\end{pmatrix} \\
&=\begin{pmatrix}
|a|^2 & ab^{*} \\
a^{*}b & |b|^2
\end{pmatrix}
\end{align}
$$
Eq. $\eqref{4}$​ becomes
$$
\begin{align}
\rho &= \frac{|c|^2}{2} \begin{pmatrix}1 & 1 \\ 1 & 1\end{pmatrix} + \frac{cd^{*}}{2}\begin{pmatrix}1 & -1 \\ 1 & -1\end{pmatrix}+ \frac{c^{*}d}{2}\begin{pmatrix}1 & 1 \\ -1 & -1\end{pmatrix}+ \frac{|d|^2}{2} \begin{pmatrix}1 & -1 \\ -1 & 1\end{pmatrix} \\
&= \frac{1}{2}\begin{pmatrix}
|c|^2 + cd^{*} + c^{*}d + |d|^2 & |c|^2 - cd^{*} + c^{*}d - |d|^2 \\
|c|^2 + cd^{*} - c^{*}d - |d|^2 & |c|^2 - cd^{*} - c^{*}d + |d|^2
\end{pmatrix}
\end{align}
$$




