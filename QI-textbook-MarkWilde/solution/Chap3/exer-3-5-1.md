## Exercise 3.5.1

Here we would show the matrix representation of $I_1X_2$ and $X_1X_2$ are the same as tensor product of $I\otimes X$ and $X\otimes X$. 

* For $I_1X_2$ case, the matrix representation can be shown as
  $$
  \begin{align}
  &\begin{pmatrix}
  \langle 00 | I_1X_2| 00 \rangle & \langle 00 | I_1X_2| 01 \rangle & \langle 00 | I_1X_2| 10 \rangle & \langle 00 | I_1X_2| 11 \rangle \\
  \langle 01 | I_1X_2| 00 \rangle & \langle 01 | I_1X_2| 01 \rangle & \langle 01 | I_1X_2| 10 \rangle & \langle 01 | I_1X_2| 11 \rangle \\
  \langle 10 | I_1X_2| 00 \rangle & \langle 10 | I_1X_2| 01 \rangle & \langle 10 | I_1X_2| 10 \rangle & \langle 10 | I_1X_2| 11 \rangle \\
  \langle 11 | I_1X_2| 00 \rangle & \langle 11 | I_1X_2| 01 \rangle & \langle 11 | I_1X_2| 10 \rangle & \langle 11 | I_1X_2| 11 \rangle \\
  \end{pmatrix} \\
  =&
  \begin{pmatrix}
  \langle 00 |  01 \rangle & \langle 00 |  00 \rangle & \langle 00 |  11 \rangle & \langle 00 |  10 \rangle \\
  \langle 01 |  01 \rangle & \langle 01 |  00 \rangle & \langle 01 |  11 \rangle & \langle 01 |  10 \rangle \\
  \langle 10 |  01 \rangle & \langle 10 |  00 \rangle & \langle 10 |  11 \rangle & \langle 10 |  10 \rangle \\
  \langle 11 |  01 \rangle & \langle 11 |  00 \rangle & \langle 11 |  11 \rangle & \langle 11 |  10 \rangle \\
  \end{pmatrix} = \begin{pmatrix}
  0 & 1 & 0 & 0 \\
  1 & 0 & 0& 0 \\
  0 & 0 & 0 & 1 \\
  0 & 0 & 1 & 0 \\
  \end{pmatrix}
  \end{align}\tag{1}\label{1}
  $$
  The tensor product of $I\otimes X$ is given by
  $$
  \begin{align}
  I\otimes X &= \begin{pmatrix} 1 & 0 \\ 0 & 1\end{pmatrix} \otimes X = \begin{pmatrix} X & 0 \\ 0 & X\end{pmatrix} \\
  &= \begin{pmatrix}
  0 & 1 & 0 & 0 \\
  1 & 0 & 0& 0 \\
  0 & 0 & 0 & 1 \\
  0 & 0 & 1 & 0 \\
  \end{pmatrix}
  \end{align}\tag{2}\label{2}
  $$
  Compare eq. $\eqref{1}$ and eq. $\eqref{2}$, we conclude that the matrix representation of $I_1X_2$ is the same as tensor product $I\otimes X$.

* For $I_1X_2$ case, the matrix representation can be shown as
  $$
  \begin{align}
  &\begin{pmatrix}
  \langle 00 | X_1X_2| 00 \rangle & \langle 00 | X_1X_2| 01 \rangle & \langle 00 | X_1X_2| 10 \rangle & \langle 00 | X_1X_2| 11 \rangle \\
  \langle 01 | X_1X_2| 00 \rangle & \langle 01 | X_1X_2| 01 \rangle & \langle 01 | X_1X_2| 10 \rangle & \langle 01 | X_1X_2| 11 \rangle \\
  \langle 10 | X_1X_2| 00 \rangle & \langle 10 | X_1X_2| 01 \rangle & \langle 10 | X_1X_2| 10 \rangle & \langle 10 | X_1X_2| 11 \rangle \\
  \langle 11 | X_1X_2| 00 \rangle & \langle 11 | X_1X_2| 01 \rangle & \langle 11 | X_1X_2| 10 \rangle & \langle 11 | X_1X_2| 11 \rangle \\
  \end{pmatrix} \\
  =&
  \begin{pmatrix}
  \langle 00 |  11 \rangle & \langle 00 |  10 \rangle & \langle 00 |  01 \rangle & \langle 00 |  00 \rangle \\
  \langle 01 |  11 \rangle & \langle 01 |  10 \rangle & \langle 01 |  01 \rangle & \langle 01 |  00 \rangle \\
  \langle 10 |  11 \rangle & \langle 10 |  10 \rangle & \langle 10 |  01 \rangle & \langle 10 |  00 \rangle \\
  \langle 11 |  11 \rangle & \langle 11 |  10 \rangle & \langle 11 |  01 \rangle & \langle 11 |  00 \rangle \\
  \end{pmatrix} = \begin{pmatrix}
  0 & 0 & 0 & 1 \\
  0 & 0 & 1 & 0 \\
  0 & 1 & 0 & 0 \\
  1 & 0 & 0 & 0 \\
  \end{pmatrix}
  \end{align}\tag{3}\label{3}
  $$
  The tensor product of $I\otimes X$ is given by
  $$
  \begin{align}
  I\otimes X &= \begin{pmatrix} 0 & 1 \\ 1 & 0\end{pmatrix} \otimes X = \begin{pmatrix} 0 & X \\ X & 0\end{pmatrix} \\
  &= \begin{pmatrix}
  0 & 0 & 0 & 1 \\
  0 & 0 & 1 & 0 \\
  0 & 1 & 0 & 0 \\
  1 & 0 & 0 & 0 \\
  \end{pmatrix}
  \end{align}\tag{4}\label{4}
  $$
  Compare eq. $\eqref{3}$ and eq. $\eqref{4}$, we conclude that the matrix representation of $X_1X_2$ is the same as tensor product $X\otimes X$.
