## Exercise 3.3.3

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
In this problem, we need to verify $X$, $Y$, $Z$ are all Hermitian, unitary, square to identity and their eigenvalue are $\pm 1$. 

* For $X$, according to eq. $\eqref{1}$, 
  $$
  X^{\dagger} = \begin{pmatrix}
  0 & 1\\ 1 &0
  \end{pmatrix} = X \tag{2}
  $$
  which shows that $X$ is Hermitian. Also, 
  $$
  X^{\dagger}X = \begin{pmatrix}
  0 & 1\\ 1 &0
  \end{pmatrix} \begin{pmatrix}
  0 & 1\\ 1 &0
  \end{pmatrix} =  \begin{pmatrix}
  1 & 0\\ 0 & 1
  \end{pmatrix} = I\tag{3}
  $$
  which shows that $X$ is unitary. Meanwhile, since $X^{\dagger} = X$ we have $X^{\dagger}X = X^2 = I$, which shows that $X$ square to identity. Finally, the eigenvalue $\lambda$ of $X$​ is the solution of the following equation,
  $$
  |X - \lambda I|= \begin{vmatrix}
  -\lambda & 1 \\ 1 & -\lambda 
  \end{vmatrix} = \lambda^2 - 1 = 0 \iff \lambda = \pm 1\tag{4}
  $$
  which shows eigenvalues of $X$ are $\pm 1$. 

* For $Y$, according to eq. $\eqref{1}$, 
  $$
  Y^{\dagger} = \begin{pmatrix}
  0 & -i\\ i &0
  \end{pmatrix}^{\dagger} = \begin{pmatrix}
  0 & -i\\ i &0
  \end{pmatrix} = Y \tag{5}
  $$
  which shows that $Y$ is Hermitian. Also, 
  $$
  Y^{\dagger}Y = \begin{pmatrix}
  0 & -i\\ i &0
  \end{pmatrix} \begin{pmatrix}
  0 & -i\\ i &0
  \end{pmatrix} =  \begin{pmatrix}
  1 & 0\\ 0 & 1
  \end{pmatrix} = I\tag{6}
  $$
  which shows that $Y$ is unitary. Meanwhile, since $Y^{\dagger} = Y$ we have $Y^{\dagger}Y = Y^2 = I$, which shows that $Y$ square to identity. Finally, the eigenvalue $\lambda$ of $Y$​ is the solution of the following equation,
  $$
  |Y - \lambda I|= \begin{vmatrix}
  -\lambda & -i \\ i & -\lambda 
  \end{vmatrix} = \lambda^2 - 1 = 0 \iff \lambda = \pm 1\tag{7}
  $$
  which shows eigenvalues of $Y$ are $\pm 1$. 

* For $Z$, according to eq. $\eqref{1}$, 
  $$
  Z^{\dagger} = \begin{pmatrix}
  1 & 0\\ 0 &-1
  \end{pmatrix} = Z \tag{8}
  $$
  which shows that $Z$ is Hermitian. Also, 
  $$
  Z^{\dagger}Z = \begin{pmatrix}
  1 & 0\\ 0 &-1
  \end{pmatrix}\begin{pmatrix}
  1 & 0\\ 0 &-1
  \end{pmatrix} =  \begin{pmatrix}
  1 & 0\\ 0 & 1
  \end{pmatrix} = I\tag{9}
  $$
  which shows that $Z$ is unitary. Meanwhile, since $Z^{\dagger} = Z$ we have $Z^{\dagger}Z = Z^2 = I$, which shows that $Z$ square to identity. Finally, the eigenvalue $\lambda$ of $Z$​ is the solution of the following equation,
  $$
  |Z - \lambda I|= \begin{vmatrix}
  1-\lambda & 0 \\ 0 & -1-\lambda 
  \end{vmatrix} = \lambda^2 - 1 = 0 \iff \lambda = \pm 1\tag{10}
  $$
  which shows eigenvalues of $Z$ are $\pm 1$. 
