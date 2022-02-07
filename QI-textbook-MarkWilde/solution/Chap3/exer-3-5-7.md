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
We also notice that
$$
\begin{align}
(|\psi^{\perp}\rangle \otimes |\psi\rangle)(\langle \psi| \otimes \langle 1|)(|\psi\rangle \otimes |0\rangle) &= |\psi^{\perp}\rangle\langle \psi|\psi\rangle\otimes |\psi\rangle \langle 1|0\rangle = 0\tag{4a} \label{4a}\\
(|\psi\rangle \otimes |\psi^{\perp}\rangle)(\langle \psi^{\perp}| \otimes \langle 1|)(|\psi^{\perp}\rangle \otimes |0\rangle)& = |\psi\rangle\langle \psi^{\perp}|\psi^{\perp}\rangle\otimes |\psi^{\perp}\rangle \langle 1|0\rangle = 0\tag{4b}\label{4b}
\end{align}
$$
From eq. $\eqref{2}$, eq. $\eqref{3}$ and eq. $\eqref{4a}-\eqref{4b}$, we can construct a linear combination of them as $U$ to make eq. $\eqref{1a}-\eqref{1b}$ valid,  
$$
\begin{align}
U =& (|\psi\rangle \otimes |\psi\rangle)(\langle \psi| \otimes \langle 0|)+ (|\psi^{\perp}\rangle \otimes |\psi\rangle)(\langle \psi| \otimes \langle 1|)\\
&+(|\psi^{\perp}\rangle \otimes |\psi^{\perp}\rangle)(\langle \psi^{\perp}| \otimes \langle 0|) +(|\psi\rangle \otimes |\psi^{\perp}\rangle)(\langle \psi^{\perp}| \otimes \langle 1|)  \\
=& |\psi\rangle\langle \psi| \otimes |\psi\rangle\langle 0| 
+ |\psi^{\perp}\rangle\langle \psi| \otimes |\psi\rangle\langle 1|
+ |\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 0| 
+ |\psi\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 1|
\end{align}\tag{5}\label{5}
$$
The reason why we need to add eq. $\eqref{4a}-\eqref{4b}$ is to make sure $U$ is a unitary matrix (see below). To verify eq. $\eqref{5}$, we need to check whether it is unitary and it satisfies eq. $\eqref{1a}-\eqref{1b}$. 

* To verify whether eq. $\eqref{5}$ is unitary, we need to adopt the property
  $$
  (A\otimes B)^{\dagger} = A^{\dagger}\otimes B^{\dagger}, (A+B)^{\dagger} = A^{\dagger} + B^{\dagger}\tag{6}
  $$
  From eq. $\eqref{5}$, we know that
  $$
  \begin{align}
  U^{\dagger} =& (|\psi\rangle\langle \psi| \otimes |\psi\rangle\langle 0|)^{\dagger}
  +  (|\psi^{\perp}\rangle\langle \psi| \otimes |\psi\rangle\langle 1|)^{\dagger} \\
  &+ (|\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 0|)^{\dagger} 
  + (|\psi\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 1|)^{\dagger}\\
  =& (|\psi\rangle\langle \psi|)^{\dagger} \otimes (|\psi\rangle\langle 0|)^{\dagger} 
  +(|\psi^{\perp}\rangle\langle \psi| )^{\dagger} \otimes (|\psi\rangle\langle 1|)^{\dagger} \\
  &+(|\psi^{\perp}\rangle \langle \psi^{\perp}|)^{\dagger} \otimes(|\psi^{\perp}\rangle \langle 0|)^{\dagger} 
  + (|\psi\rangle \langle \psi^{\perp}|  \otimes(|\psi^{\perp}\rangle \langle 1|)^{\dagger} \\
  =& |\psi\rangle\langle \psi| \otimes |0\rangle\langle \psi| 
  + |\psi\rangle\langle \psi^{\perp}| \otimes |1\rangle\langle \psi|
  + |\psi^{\perp}\rangle \langle \psi^{\perp}|\otimes|0\rangle \langle \psi^{\perp}| 
  +  |\psi^{\perp}\rangle \langle \psi|\otimes|1\rangle \langle \psi^{\perp}|
  \end{align}\tag{7}
  $$
  Then we could have
  $$
  \begin{align}
  U^{\dagger}U =& 
  (|\psi\rangle\langle \psi| \otimes |0\rangle\langle \psi| 
  + |\psi\rangle\langle \psi^{\perp}| \otimes |1\rangle\langle \psi|
  + |\psi^{\perp}\rangle \langle \psi^{\perp}|\otimes|0\rangle \langle \psi^{\perp}| 
  +  |\psi^{\perp}\rangle \langle \psi|\otimes|1\rangle \langle \psi^{\perp}|)
  \\&\cdot
  (|\psi\rangle\langle \psi| \otimes |\psi\rangle\langle 0| 
  + |\psi^{\perp}\rangle\langle \psi| \otimes |\psi\rangle\langle 1|
  + |\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 0| 
  + |\psi\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 1|)
  
  \\\\
  =& |\psi\rangle\langle \psi|\psi\rangle\langle \psi|   \otimes    |0\rangle\langle \psi|\psi\rangle\langle 0| 
  + |\psi\rangle\langle \psi|\psi^{\perp}\rangle\langle \psi|   \otimes    |0\rangle\langle \psi|\psi\rangle\langle 1|
   \\
  
  &+ |\psi\rangle\langle \psi|\psi^{\perp}\rangle \langle \psi^{\perp}|    \otimes   |0\rangle\langle \psi|\psi^{\perp}\rangle \langle 0|  
  + |\psi\rangle\langle \psi|\psi\rangle \langle \psi^{\perp}|    \otimes   |0\rangle\langle \psi|\psi^{\perp}\rangle \langle 1|
  
  \\\\ 
  
  &+|\psi\rangle\langle \psi^{\perp}|\psi\rangle\langle \psi|   \otimes    |1\rangle\langle \psi|\psi\rangle\langle 0|
  + |\psi\rangle\langle \psi^{\perp}|\psi^{\perp}\rangle\langle \psi|  \otimes    |1\rangle\langle \psi|\psi\rangle\langle 1|
   \\
  
  &+ |\psi\rangle\langle \psi^{\perp}|\psi^{\perp}\rangle \langle \psi^{\perp}|   \otimes   |1\rangle\langle \psi|\psi^{\perp}\rangle \langle 0| 
  + |\psi\rangle\langle \psi^{\perp}|\psi\rangle \langle \psi^{\perp}|    \otimes   |1\rangle\langle \psi|\psi^{\perp}\rangle \langle 1| \\\\
  &+ |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi\rangle\langle \psi|\otimes  |0\rangle \langle \psi^{\perp}|\psi\rangle\langle 0|
  + |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle\langle \psi|\otimes  |0\rangle \langle \psi^{\perp}|\psi\rangle\langle 1|
  \\
  
  
  
  &+ |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \langle \psi^{\perp}|  \otimes |0\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \langle 0| 
  + |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi\rangle \langle \psi^{\perp}| \otimes |0\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \langle 1|
  
  \\\\%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
  
  
  &+ |\psi^{\perp}\rangle \langle \psi|\psi\rangle\langle \psi|\otimes  |1\rangle \langle \psi^{\perp}|\psi\rangle\langle 0| 
  + |\psi^{\perp}\rangle \langle \psi|\psi^{\perp}\rangle\langle \psi|\otimes  |1\rangle \langle \psi^{\perp}|\psi\rangle\langle 1|
  \\
  
  
  
  &+ |\psi^{\perp}\rangle \langle \psi|\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes |1\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \langle 0| 
  + |\psi^{\perp}\rangle \langle \psi|\psi\rangle \langle \psi^{\perp}| \otimes |1\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \langle 1|
  
  
  \\%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
  \\
  =& |\psi\rangle\langle \psi|    \otimes    |0\rangle\langle 0| 
  + |\psi\rangle\langle \psi|    \otimes    |1\rangle\langle 1| 
  + |\psi^{\perp}\rangle \langle \psi^{\perp}|    \otimes    |0\rangle \langle 0| 
  +|\psi^{\perp}\rangle \langle \psi^{\perp}|    \otimes    |1\rangle \langle 1|
  \end{align}\tag{8}\label{8}
  $$
  Since $\{|0\rangle, |1\rangle\}$ and $\{|+\rangle, |-\rangle\}$​ are all orthonormal basis, we should have
  $$
  \begin{align}
  |0\rangle\langle 0| + |1\rangle\langle 1| = I, \;
  |\psi\rangle\langle \psi|  + |\psi^{\perp}\rangle \langle \psi^{\perp}|  = I\tag{9}
  \end{align}
  $$
   Therefore, from eq. $\eqref{8}$ we know that $U^{\dagger}U = I$. 
  
* To verify whether eq. $\eqref{5}$ satisfies eq. $\eqref{1a}$, we have
  $$
  \begin{align}
  U(|\psi\rangle \otimes |0\rangle) =& 
  |\psi\rangle\langle \psi| \otimes |\psi\rangle\langle 0| (|\psi\rangle \otimes |0\rangle)
  + |\psi^{\perp}\rangle\langle \psi| \otimes |\psi\rangle\langle 1|(|\psi\rangle \otimes |0\rangle) \\
  
  &+ |\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 0|(|\psi\rangle \otimes |0\rangle) 
  + |\psi\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 1| (|\psi\rangle \otimes |0\rangle)\\
  =& |\psi\rangle\langle \psi|\psi\rangle \otimes |\psi\rangle\langle 0|0\rangle 
  + |\psi^{\perp}\rangle\langle \psi|\psi\rangle  \otimes |\psi\rangle\langle 1|0\rangle \\
  &+ |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi\rangle \otimes|\psi^{\perp}\rangle \langle 0|0\rangle + |\psi\rangle \langle \psi^{\perp}|\psi\rangle \otimes|\psi^{\perp}\rangle \langle 1|0\rangle \\
  =& |\psi\rangle \otimes |\psi\rangle
  \end{align}\tag{10}
  $$
  
* To verify whether eq. $\eqref{5}$​ satisfies eq. $\eqref{1b}$​, we have
  $$
  \begin{align}
  U(|\psi\rangle \otimes |0\rangle) =& 
  |\psi\rangle\langle \psi| \otimes |\psi\rangle\langle 0| (|\psi^{\perp}\rangle \otimes |0\rangle)
  + |\psi^{\perp}\rangle\langle \psi| \otimes |\psi\rangle\langle 1|(|\psi^{\perp}\rangle \otimes |0\rangle)\\
  
  &+ |\psi^{\perp}\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 0|(|\psi^{\perp}\rangle \otimes |0\rangle) 
  + |\psi\rangle \langle \psi^{\perp}| \otimes|\psi^{\perp}\rangle \langle 1| (|\psi^{\perp}\rangle \otimes |0\rangle)\\
  =& |\psi\rangle\langle \psi|\psi^{\perp}\rangle \otimes |\psi\rangle\langle 0|0\rangle 
  + |\psi^{\perp}\rangle\langle \psi|\psi^{\perp}\rangle  \otimes |\psi\rangle\langle 1|0\rangle \\
  &+ |\psi^{\perp}\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \otimes|\psi^{\perp}\rangle \langle 0|0\rangle
  + |\psi\rangle \langle \psi^{\perp}|\psi^{\perp}\rangle \otimes|\psi^{\perp}\rangle \langle 1|0\rangle \\
  =& |\psi^{\perp}\rangle \otimes |\psi^{\perp}\rangle
  \end{align}\tag{11}
  $$
  

