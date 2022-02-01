## Exercise 3.4.4

Consider operator $Z_0 = Z - \langle Z\rangle I $ and $X_0 = X - \langle X \rangle I$, we could find that 
$$
\begin{align}
[Z_0, X_0] &= Z_0X_0- X_0Z_0 \\
&= (Z - \langle Z\rangle)(X - \langle X \rangle)- (X - \langle X \rangle)(Z - \langle Z\rangle) \\
&= ZX - \langle X\rangle Z - \langle Z\rangle X +\langle Z\rangle\langle X\rangle I - XZ + \langle Z\rangle X  + \langle X\rangle Z - \langle X\rangle\langle Z\rangle I \\
&= ZX - XZ \\
&= [Z, X]
\end{align}\tag{1}
$$
Also, 
$$
\begin{align}
[Z, X] = ZX-XZ &= \begin{pmatrix}
1 & 0\\ 0 &-1
\end{pmatrix}\begin{pmatrix}
0 & 1\\ 1 &0
\end{pmatrix} - \begin{pmatrix}
0 & 1\\ 1 &0
\end{pmatrix}\begin{pmatrix}
1 & 0\\ 0 &-1
\end{pmatrix} \\ 

&= \begin{pmatrix}
0 & 1\\ -1 & 0
\end{pmatrix} - \begin{pmatrix}
0 & -1\\ 1 & 0
\end{pmatrix} \\

&= 2\begin{pmatrix}
0 & 1\\ -1 & 0
\end{pmatrix} = 2i\begin{pmatrix}
0 & -i\\ i & 0
\end{pmatrix} = 2iY
\end{align}\tag{2}
$$
