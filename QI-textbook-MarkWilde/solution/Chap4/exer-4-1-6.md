## Exercise 4.1.6

The density matrix $\rho$ of a given ensemble $\mathcal{E} = \{p_{X}(x), |\psi_x\rangle\}$ is defined as
$$
\rho = \sum_{x\in\mathcal{X}}p_{X}(x)|\psi_x\rangle\langle \psi_x|\tag{1}\label{1}
$$
We can decompose the density matrix by spectral theorem as
$$
\rho = \sum_{x=0}^{d-1}\lambda_x |\phi_x\rangle\langle \phi_x|\tag{2}\label{2}
$$
where $\lambda_x$ are eigenvalues and $\{|\phi_x\rangle\}$ are orthonormal basis (also eigenvector of $\lambda_x$). According to eq. $\eqref{2}$, the trace of density matrix is given by
$$
{\rm Tr}\rho = \sum_{y}\langle\phi_y| \rho |\phi_y\rangle =1 \tag{3}\label{3}
$$
Combine eq. $\eqref{2}$ and eq. $\eqref{3}$, we have
$$
\begin{align}
{\rm Tr}\rho &= \sum_{y=0}^{d-1}\langle\phi_y| \rho |\phi_y\rangle \\
&= \sum_{y=0}^{d-1}\langle\phi_y|\left(\sum_{x=0}^{d-1}\lambda_x |\phi_x\rangle\langle \phi_x|\right) |\phi_y\rangle \\
&= \sum_{x, y=0}^{d-1}\langle\phi_y|\lambda_x |\phi_x\rangle\langle \phi_x|\phi_y\rangle \\
&= \sum_{y=0}^{d-1}\lambda_y = 1 \\
\end{align}\tag{4}\label{4}
$$
Note also that $\rho\geq 0$, which means that for any vector $|v\rangle$, we should have
$$
\langle v|\rho|v\rangle \geq 0\tag{5}\label{5}
$$
where vector $|v\rangle$ can be expanded by basis $\{|\phi_{k}\rangle\}$ as $|v\rangle = \sum_{x=0}^{d-1}c_x|\phi_x\rangle$. From eq. $\eqref{2}$ and eq. $\eqref{5}$, we should have
$$
\begin{align}
\langle v|\rho|v\rangle &= \left(\sum_{x=0}^{d-1}c^{*}_x\langle \phi_x|\right)\left(\sum_{y=0}^{d-1}\lambda_y |\phi_y\rangle\langle \phi_y|\right)\left(\sum_{z=0}^{d-1}c_z|\phi_z\rangle\right) \\
&= \sum_{x,y,z=0}^{d-1} c^{*}_xc_z\lambda_y\langle \phi_x|\phi_y\rangle\langle \phi_y|\phi_z\rangle \\
&= \sum_{x,y=0}^{d-1} c^{*}_xc_y\lambda_y\langle \phi_x|\phi_y\rangle\langle \phi_y|\phi_y\rangle \\
&= \sum_{y=0}^{d-1} c^{*}_yc_y\lambda_y\langle \phi_y|\phi_y\rangle = \sum_{y=0}^{d-1} |c_y|^{2}\lambda_y \geq 0 \\
\end{align}\tag{6}\label{6}
$$
From eq. $\eqref{4}$ and eq.$\eqref{6}$ we should have $\lambda_x \geq 0$ and $\sum_x\lambda_x = 1$, then we can consider $\lambda_x$ as some probability. 

