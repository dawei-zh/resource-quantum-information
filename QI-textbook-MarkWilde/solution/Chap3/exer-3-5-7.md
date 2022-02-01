## Exercise 3.5.7

Suppose we have two quantum state $|\psi\rangle$ and $|\psi^{\perp}\rangle$ with $\langle \psi|\psi^{\perp}\rangle = 0$, we want to find a unitary  $U$ that 
$$
\begin{align}
U(|\psi\rangle \otimes |0\rangle) &= |\psi\rangle \otimes |\psi\rangle \tag{1a} \label{1a}\\
U(|\psi^{\perp}\rangle \otimes |0\rangle) &= |\psi^{\perp}\rangle \otimes |\psi^{\perp}\rangle \tag{1b}\label{1b}\\
\end{align}
$$
A unitary matrix $U$ can be written in the form $U = \sum_{i}\lambda_i|i\rangle\langle i |$, which inspire us to find a linear combination of something in the form $|i\rangle\langle j |$. 

From eq. $\eqref{1a}$, we notice that 
$$
(|\psi\rangle \otimes |\psi\rangle)(\langle \psi| \otimes \langle 0|)(|\psi\rangle \otimes |0\rangle) = |\psi\rangle\langle \psi|\psi\rangle\otimes |\psi\rangle \langle 0|0\rangle = |\psi\rangle \otimes |\psi\rangle \tag{2}\label{2}
$$
From eq. $\eqref{1b}$​, we notice that 
$$
(|\psi^{\perp}\rangle \otimes |\psi^{\perp}\rangle)(\langle \psi^{\perp}| \otimes \langle 0|)(|\psi^{\perp}\rangle \otimes |0\rangle) = |\psi^{\perp}\rangle\langle \psi^{\perp}|\psi^{\perp}\rangle\otimes |\psi^{\perp}\rangle \langle 0|0\rangle = |\psi^{\perp}\rangle \otimes |\psi^{\perp}\rangle \tag{3}\label{3}
$$
From eq. $\eqref{2}$ and eq. $\eqref{3}$, we can construct a linear combination of them as $U$ to make eq. $\eqref{1a}-\eqref{1b}$ valid,  
$$
\begin{align}
U &= (|\psi\rangle \otimes |\psi\rangle)(\langle \psi| \otimes \langle 0|) + (|\psi^{\perp}\rangle \otimes |\psi^{\perp}\rangle)(\langle \psi^{\perp}| \otimes \langle 0|)\\
&=  |\psi\rangle\langle \psi| \otimes |\psi\rangle\langle 0| + |\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 0|
\end{align}\tag{4}\label{4}
$$
To verify eq. $\eqref{4}$, we need to check whether it is unitary and it satisfies eq. $\eqref{1a}-\eqref{1b}$. 

* To verify whether eq. $\eqref{4}$ is unitary, we need to adopt the property
  $$
  (A\otimes B)^{\dagger} = A^{\dagger}\otimes B^{\dagger}, (A+B)^{\dagger} = A^{\dagger} + B^{\dagger}\tag{5}
  $$
  From eq. $\eqref{4}$, we know that
  $$
  \begin{align}
  U^{\dagger} &= (|\psi\rangle\langle \psi| \otimes |\psi\rangle\langle 0|)^{\dagger} + (|\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 0|)^{\dagger} \\
  &= (|\psi\rangle\langle \psi|)^{\dagger} \otimes (|\psi\rangle\langle 0|)^{\dagger} + (|\psi^{\perp}\rangle \langle \psi^{\perp}|)^{\dagger} \otimes(|\psi^{\perp}\rangle \langle 0|)^{\dagger}  \\
  &= |\psi\rangle\langle \psi| \otimes |0\rangle\langle \psi| + |\psi^{\perp}\rangle \langle \psi^{\perp}|\otimes|0\rangle \langle \psi^{\perp}|
  \end{align}\tag{6}
  $$
  Then we could have
  $$
  \begin{align}
  U^{\dagger}U =& 
  (|\psi\rangle\langle \psi|    \otimes    |0\rangle\langle \psi| + 
  |\psi^{\perp}\rangle \langle \psi^{\perp}|    \otimes    |0\rangle \langle \psi^{\perp}|)
  
  (|\psi\rangle\langle \psi|    \otimes    |\psi\rangle\langle 0| + 
  |\psi^{\perp}\rangle \langle \psi^{\perp}|    \otimes    |\psi^{\perp}\rangle \langle 0|) \\
  
  =& |\psi\rangle\langle \psi|\psi\rangle\langle \psi|   \otimes    |0\rangle\langle \psi|\psi\rangle\langle 0| +
  |\psi\rangle\langle \psi|\psi^{\perp}\rangle \langle \psi^{\perp}|    \otimes   |0\rangle\langle \psi |\psi^{\perp}\rangle \langle 0| \\
  
  &+ |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi\rangle\langle \psi|\otimes  |0\rangle \langle \psi^{\perp}|\psi\rangle\langle 0| +
  
  |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes |0\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \langle 0|
  \\ 
  =& |\psi\rangle\langle \psi|    \otimes    |0\rangle\langle 0| + |\psi^{\perp}\rangle \langle \psi^{\perp}|    \otimes    |0\rangle \langle 0|\\
  \end{align}\tag{7}
  $$
  For a

  
