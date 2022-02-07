## Exercise 3.3.9

The Hadmard gate is given by
$$
H = \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix}\tag{1}\label{1}
$$
We can check that Hadmard gate given in eq. $\eqref{1}$ is its own inverse, 
$$
HH = \frac{1}{2}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} = \frac{1}{2}\begin{pmatrix}
2 & 0 \\ 0 & 2
\end{pmatrix} = \begin{pmatrix}
1 & 0 \\ 0 & 1
\end{pmatrix} = I\tag{2}
$$
We can also check that,
$$
\begin{align}
|0\rangle\langle + | + |1\rangle \langle -| &= 
\frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ 0 
\end{pmatrix}\begin{pmatrix}
1 & 1
\end{pmatrix} + \frac{1}{\sqrt{2}}\begin{pmatrix}
0 \\ 1 
\end{pmatrix}\begin{pmatrix}
1 & -1
\end{pmatrix} \\
&= \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 1 \\ 0 & 0
\end{pmatrix} + \frac{1}{\sqrt{2}}\begin{pmatrix}
0 & 0 \\ 1 & -1
\end{pmatrix}\\
&= \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} = H
\end{align}\tag{3}\label{3}
$$
That is, Hadmard gate can be re-written as $H = |0\rangle\langle + | + |1\rangle \langle -|$. Also, we can check 
$$
\begin{align}
|+\rangle\langle 0 | + |-\rangle \langle 1| &= 
\frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ 1 
\end{pmatrix}\begin{pmatrix}
1 & 0
\end{pmatrix} + \frac{1}{\sqrt{2}}\begin{pmatrix}
1 \\ -1 
\end{pmatrix}\begin{pmatrix}
0 & 1
\end{pmatrix} \\
&= \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 0 \\ 1 & 0
\end{pmatrix} + \frac{1}{\sqrt{2}}\begin{pmatrix}
0 & 1 \\ 0 & -1
\end{pmatrix}\\
&= \frac{1}{\sqrt{2}}\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} = H
\end{align}\tag{4}\label{4}
$$
From eq. $\eqref{3}$ and eq. $\eqref{4}$, we have
$$
H = |0\rangle\langle + | + |1\rangle \langle -| = |+\rangle\langle 0 | + |-\rangle \langle 1|  \tag{5}
$$

---

We can also prove the identity without the matrix form of Hadmard gate. The Hadmard gate can take $|+\rangle$ and $|-\rangle$ into $|0\rangle$ and $|1\rangle$, respectively. The definition of Hadmard gate
$$
H = |0\rangle\langle + | + |1\rangle \langle -|\tag{6}
$$
satisfies the definition, 
$$
\begin{align}
H|+\rangle &= |0\rangle\langle + |+\rangle + |1\rangle \langle -|+\rangle = |0\rangle\\
H|-\rangle &= |0\rangle\langle + |-\rangle + |1\rangle \langle -|-\rangle = |1\rangle
\end{align}\tag{7}\label{7}
$$
For $|+\rangle\langle 0| + |-\rangle\langle 1|$, note that $|0\rangle = (|+\rangle+|-\rangle)/\sqrt{2}$ and $|1\rangle = (|+\rangle-|-\rangle)/\sqrt{2}$, we have
$$
\begin{align}
(|+\rangle\langle 0| + |-\rangle\langle 1|)|+\rangle &= |+\rangle\langle 0|+\rangle + |-\rangle\langle 1|+\rangle \\
&= \frac{1}{\sqrt{2}}|+\rangle(\langle +|+\langle -|)|+\rangle + \frac{1}{\sqrt{2}}|-\rangle(\langle +|-\langle -|)|+\rangle \\
&= \frac{1}{\sqrt{2}}(|+\rangle\langle +|+\rangle+|+\rangle\langle -|+\rangle+|-\rangle\langle +|+\rangle - |-\rangle\langle -|+\rangle ) \\
&= \frac{1}{\sqrt{2}}(|+\rangle+|-\rangle) = |0\rangle 
\end{align}\tag{8}\label{8}
$$
Also, 
$$
\begin{align}
(|+\rangle\langle 0| + |-\rangle\langle 1|)|-\rangle &= |+\rangle\langle 0|-\rangle + |-\rangle\langle 1|-\rangle \\
&= \frac{1}{\sqrt{2}}|+\rangle(\langle +|+\langle -|)|-\rangle + \frac{1}{\sqrt{2}}|-\rangle(\langle +|-\langle -|)|-\rangle \\
&= \frac{1}{\sqrt{2}}(|+\rangle\langle +|-\rangle+|
+\rangle\langle -|-\rangle
+|-\rangle\langle +|-\rangle 
-|-\rangle\langle -|-\rangle ) \\
&= \frac{1}{\sqrt{2}}(|+\rangle-|-\rangle) = |1\rangle 
\end{align}\tag{9}\label{9}
$$
From eq. $\eqref{7}-\eqref{9}$, we conclude that
$$
H = |0\rangle\langle + | + |1\rangle \langle -| = |+\rangle\langle 0 | + |-\rangle \langle 1|  \tag{10}
$$
