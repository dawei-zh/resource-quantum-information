## Exercise 3.3.5

The Pauli matrices are given by
$$
X = \begin{pmatrix}
0 & 1\\ 1 &0
\end{pmatrix},Y= \begin{pmatrix}
0 & -i\\ i &0
\end{pmatrix},Z = \begin{pmatrix}
1 & 0\\ 0 &-1
\end{pmatrix} \tag{1}\label{1}
$$
For commutator part, we have

* The Pauli matrices commute with itself, that is
  $$
  \begin{align}
  [X, X] &= XX - XX =0 \tag{2a}\label{2a}\\
  [Y, Y] &= YY - YY =0 \tag{2b}\label{2b}\\
  [Z, Z] &= ZZ - ZZ =0 \tag{2c}\label{2c}
  \end{align}
  $$

* The Pauli matrices does not commute with other Pauli matrices, that is, 

  *  For $[X, Y]$​, we have
    $$
    \begin{align}
    [X, Y] = XY - YX &= \begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix} - \begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix} \\ 
    
    &= \begin{pmatrix}
    i & 0\\ 0 &-i
    \end{pmatrix} - \begin{pmatrix}
    -i & 0\\ 0 & i
    \end{pmatrix} \\
    
    &= 2i\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix} = 2iZ
    \end{align}\tag{3}
    $$

  * For $[Y, Z]$​, we have
    $$
    \begin{align}
    [Y, Z] = YZ-ZY &= \begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix}\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix} - \begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix} \\ 
    
    &= \begin{pmatrix}
    0 & i\\ i & 0
    \end{pmatrix} - \begin{pmatrix}
    0 & -i\\ -i & 0
    \end{pmatrix} \\
    
    &= 2i\begin{pmatrix}
    0 & 1\\ 1 & 0
    \end{pmatrix} = 2iX
    \end{align}\tag{4}
    $$

  * For $[Z, X]$​, we have
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
    \end{align}\tag{5}
    $$

For anticommute part, we have

* The Pauli matrices does not anticommute with itself, that is
  $$
  \begin{align}
  \{X, X\} &= XX + XX = 2I  \tag{6a}\\
  \{Y, Y\} &= YY + YY = 2I \tag{6b}\\
  \{Z, Z\} &= ZZ + ZZ = 2I \tag{6c}
  \end{align}
  $$
  since $X, Y, Z$ square to the identity (exercise 3.3.3). 

* The Pauli matrices  anticommute with other Pauli matrices, that is, 

  * For $\{X, Y\}$​, we have
    $$
    \begin{align}
    \{X, Y\} &= \{Y, X\} = XY + YX \\
    &= \begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix} + \begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix} \\ 
    
    &= \begin{pmatrix}
    i & 0\\ 0 &-i
    \end{pmatrix} + \begin{pmatrix}
    -i & 0\\ 0 & i
    \end{pmatrix} = 0
    \end{align}\tag{7}\label{7}
    $$

  * For $\{Y, Z\}$​, we have
    $$
    \begin{align}
    \{Y, Z\} =  \{Z, Y\} &= YZ+ZY \\
    &= \begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix}\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix} + \begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix} \\ 
    
    &= \begin{pmatrix}
    0 & i\\ i & 0
    \end{pmatrix} + \begin{pmatrix}
    0 & -i\\ -i & 0
    \end{pmatrix} = 0
    \end{align}\tag{8}\label{8}
    $$

  * For $\{Z, X\}$​, we have
    $$
    \begin{align}
    \{Z, X\} &= \{X, Z\} = ZX+XZ \\
    &= \begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix} + \begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix}\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix} \\ 
    
    &= \begin{pmatrix}
    0 & 1\\ -1 & 0
    \end{pmatrix} + \begin{pmatrix}
    0 & -1\\ 1 & 0
    \end{pmatrix} =0 
    \end{align}\tag{9}\label{9}
    $$

Therefore, from eq. $\eqref{2a}-\eqref{2c}$ and eq. $\eqref{7}-\eqref{9}$, we conclude that the Pauli matrices either commute or anticommute, that is, 
$$
\begin{align}
[X, X] &= [Y, Y] =[Z, Z] = 0 \tag{10a}\\
\{X, Y\} = \{Y, X\} &= \{Y, Z\} =  \{Z, Y\} = \{Z, X\} = \{X, Z\} =0\tag{10b}
\end{align}
$$
