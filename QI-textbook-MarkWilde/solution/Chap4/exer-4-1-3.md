## Exercise 4.1.3

The unnormalized maximally entagled vector is defined by
$$
|\Gamma\rangle_{RS} = \sum_{i=0}^{d-1} |i\rangle_{R}\otimes |i\rangle_{S}\tag{1}
$$
where $d$ is the dimension of vector space $R\otimes S$. $|i\rangle_{R}$ and $|i\rangle_{S}$ are orthonormal basis in vector space $R$ and $S$, respectively. We need to use the properties of tensor product to prove the statement. The definition of operator $A\otimes B$ on vector space $R\otimes S$​ is given by
$$
(A\otimes B)\sum_{i} |r_{i}\rangle \otimes |s_{i}\rangle = \sum_{i} A|r_{i}\rangle \otimes B|s_{i}\rangle\tag{2}
$$
where $|r_{i}\rangle $and $|s_i\rangle$ are arbitrary vectors in vector space $R$ and $S$, respectively. Therefore, 
$$
\begin{align}
\langle \Gamma|_{RS} I_{R}\otimes A_{S} |\Gamma\rangle_{RS} &= \langle \Gamma|_{RS} I_{R}\otimes A_{S} \left(\sum_{i=0}^{d-1} |i\rangle_{R}\otimes |i\rangle_{S}\right) \\
&= \langle \Gamma|_{RS}\left(\sum_{i=0}^{d-1} I_{R}|i\rangle_{R}\otimes A_{S}|i\rangle_{S}\right) \\
&=  \left(\sum_{j=0}^{d-1} \langle j|_{R} \otimes \langle j|_{S} \right)\left(\sum_{i=0}^{d-1} |i\rangle_{R}\otimes A_{S}|i\rangle_{S}\right) \\
\end{align}\tag{3}\label{3}
$$
where we use $i$ and $j$ to clarify contribution from $|\Gamma\rangle_{RS}$ and $\langle\Gamma|_{RS}$. Note also that for the inner product of $R\otimes S$, we have
$$
\left(\sum_{i}a_{i}|r_i\rangle \otimes |s_i\rangle, \sum_{j}b_{j}|r'_j\rangle \otimes |s'_j\rangle\right) = \left(\sum_{i}a^{*}_{i}\langle r_i| \otimes \langle s_i|\right) \left(\sum_{j}b_{j}|r'_j\rangle \otimes |s'_j\rangle\right) = \sum_{i,j}a^{*}_{i}b_{j}\langle r_i|r'_j\rangle \otimes \langle s_i|s'_j\rangle\tag{4}\label{4}
$$
From eq. $\eqref{4}$, we can simplify eq. $\eqref{3}$ and get
$$
\begin{align}
\langle \Gamma|_{RS} I_{R}\otimes A_{S} |\Gamma\rangle_{RS} &= \sum_{i,j}\langle j|i\rangle_{R}\langle j|A_{S}|i\rangle_{S} \\
&= \sum_{i}\langle i|i\rangle_{R}\langle i|A_{S}|i\rangle_{S} \\
&= \sum_{i}\langle i|A_{S}|i\rangle_{S} \\
&= {\rm Tr}\{ A_{S}\} 
\end{align}\tag{5}
$$
where the second and third identity comes from the orthonormality of $|i\rangle_{R}$. 
