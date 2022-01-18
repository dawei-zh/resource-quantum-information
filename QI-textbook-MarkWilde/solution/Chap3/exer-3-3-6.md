## Exercise 3.3.6

If we label Pauli matrices as 
$$
\sigma_0 = I, \sigma_1 = X, \sigma_2 = Y, \sigma_3 = Z \tag{1}\label{1}
$$
we need to verify ${\rm Tr}\{\sigma_{i}\sigma_{j}\} = 2\delta_{ij}$. 

* For $i=j$, we should verify ${\rm Tr}\{\sigma_{i}\sigma_{j}\} = 2$. Since $\sigma_0, \sigma_1, \sigma_2, \sigma_3$ are Hermitian and unitary operator, we do have 
  $$
  \sigma_0\sigma_0 = \sigma_1\sigma_1 = \sigma_2\sigma_2 = \sigma_3\sigma_3 = I \tag{2}
  $$
  and thus, 
  $$
  {\rm Tr}(\sigma_0\sigma_0) = {\rm Tr}(\sigma_1\sigma_1) = {\rm Tr}(\sigma_2\sigma_2) = {\rm Tr}(\sigma_3\sigma_3) = {\rm Tr}I = 2 \tag{3}
  $$

* For $i\neq j$, we should verify ${\rm Tr}\{\sigma_{i}\sigma_{j}\} = 0$.

  * For ${\rm Tr}\{\sigma_{0}\sigma_{1}\}$ and ${\rm Tr}\{\sigma_{1}\sigma_{0}\}$,
    $$
    {\rm Tr}\{\sigma_{0}\sigma_{1}\} = {\rm Tr}\{\sigma_{1}\sigma_{0}\} = {\rm Tr}(\sigma_1) = {\rm Tr}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix} = 0\tag{4}
    $$

  * For ${\rm Tr}\{\sigma_{0}\sigma_{2}\}$ and ${\rm Tr}\{\sigma_{2}\sigma_{0}\}$,
    $$
    {\rm Tr}\{\sigma_{0}\sigma_{2}\} ={\rm Tr}\{\sigma_{2}\sigma_{0}\} = {\rm Tr}(\sigma_2) = {\rm Tr}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix} = 0\tag{5}
    $$

  * For ${\rm Tr}\{\sigma_{0}\sigma_{3}\}$ and ${\rm Tr}\{\sigma_{3}\sigma_{0}\}$,
    $$
    {\rm Tr}\{\sigma_{0}\sigma_{3}\} = {\rm Tr}\{\sigma_{3}\sigma_{0}\} = {\rm Tr}(\sigma_3) = {\rm Tr}\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix} = 0\tag{6}
    $$

  * For ${\rm Tr}\{\sigma_{1}\sigma_{2}\}$,
    $$
    {\rm Tr}\{\sigma_{1}\sigma_{2}\} = {\rm Tr}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix} = {\rm Tr}\begin{pmatrix}
    i & 0\\ 0 & -i
    \end{pmatrix} = 0\tag{7}
    $$

  * For ${\rm Tr}\{\sigma_{1}\sigma_{3}\}$,
    $$
    {\rm Tr}\{\sigma_{1}\sigma_{3}\} = {\rm Tr}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix}\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix} = {\rm Tr}\begin{pmatrix}
    0 & -1\\ 1 & 0
    \end{pmatrix} = 0\tag{8}
    $$

  * For ${\rm Tr}\{\sigma_{2}\sigma_{1}\}$​,
    $$
    {\rm Tr}\{\sigma_{2}\sigma_{1}\} = {\rm Tr}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix} = {\rm Tr}\begin{pmatrix}
    -i & 0\\ 0 & i
    \end{pmatrix} = 0\tag{9}
    $$

  * For ${\rm Tr}\{\sigma_{2}\sigma_{3}\}$​,
    $$
    {\rm Tr}\{\sigma_{2}\sigma_{3}\} = {\rm Tr} \begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix}\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix} = {\rm Tr}\begin{pmatrix}
    0 & i\\ i & 0
    \end{pmatrix} = 0\tag{10}
    $$

  * For ${\rm Tr}\{\sigma_{3}\sigma_{1}\}$​,
    $$
    {\rm Tr}\{\sigma_{3}\sigma_{1}\} = {\rm Tr}\begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix}\begin{pmatrix}
    0 & 1\\ 1 &0
    \end{pmatrix} = {\rm Tr}\begin{pmatrix}
    0 & 1\\ -1 & 0
    \end{pmatrix} = 0\tag{11}
    $$

  * For ${\rm Tr}\{\sigma_{3}\sigma_{2}\}$​,
    $$
    {\rm Tr}\{\sigma_{3}\sigma_{2}\} = {\rm Tr} \begin{pmatrix}
    1 & 0\\ 0 &-1
    \end{pmatrix}\begin{pmatrix}
    0 & -i\\ i &0
    \end{pmatrix} = {\rm Tr}\begin{pmatrix}
    0 & -i\\ -i & 0
    \end{pmatrix} = 0\tag{12}
    $$
