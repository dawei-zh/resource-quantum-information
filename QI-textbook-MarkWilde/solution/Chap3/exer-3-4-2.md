## Exercise 3.4.2

In quantum mechanics, the measurement result is the eigenvalues of the observable. Suppose we have an arbitrary state $|\psi\rangle =\alpha |0\rangle+\beta|1\rangle$​, and 
$$
\alpha = a + ib,\, \beta = c+id \;\;\; \alpha, \beta\in\mathbb{C}\tag{1}\label{1}
$$
we can check the expectation value of measuring $X$​ and $Y$​. 

* For observable $X$, the eigenvalues are $+1$ and $-1$, and the corresponding eigenvectors are $|+\rangle$ and $|-\rangle$. Note that
  $$
  \begin{align}
  |0\rangle &= \begin{pmatrix}
  1 \\ 0
  \end{pmatrix} = \frac{1}{\sqrt{2}}\left[ \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ 1
  \end{pmatrix} +  \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ -1
  \end{pmatrix}\right] = \frac{|+\rangle+|-\rangle}{\sqrt{2}}\tag{2a} \\
  |1\rangle &= \begin{pmatrix}
  0 \\ 1
  \end{pmatrix} = \frac{1}{\sqrt{2}}\left[ \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ 1
  \end{pmatrix} -  \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ -1
  \end{pmatrix}\right] = \frac{|+\rangle-|-\rangle}{\sqrt{2}}\tag{2b}
  \end{align}
  $$
  We can re-write the quantum state as
  $$
  |\psi\rangle =\alpha |0\rangle+\beta|1\rangle = \alpha \frac{|+\rangle+|-\rangle}{\sqrt{2}}+\beta\frac{|+\rangle-|-\rangle}{\sqrt{2}} = \frac{(\alpha+\beta)|+\rangle + (\alpha-\beta)|-\rangle}{\sqrt{2}}\tag{3}
  $$
  Thus, the probability of getting $|+\rangle$ is $|\alpha+\beta|^2/2$,  the probability of getting $|-\rangle$ is $|\alpha-\beta|^2/2$, and the expectation value of measuring $X$ is given by
  $$
  \mathbb{E}(X) =\frac{|\alpha+\beta|^2}{2}\times 1 +  \frac{|\alpha-\beta|^2}{2}\times (-1) = \frac{|\alpha+\beta|^2 - |\alpha-\beta|^2}{2}\tag{4}\label{4}
  $$
  According to eq. $\eqref{1}$, we can re-write eq. $\eqref{4}$ as
  $$
  \begin{align}
  \mathbb{E}(X) &= \frac{|\alpha+\beta|^2 - |\alpha-\beta|^2}{2} \\
  &= \frac{|a+ib+c+id|^2 - |a+ib-c-id|^2}{2} \\
  &= \frac{|(a+c)+i(b+d)|^2 - |(a-c)+i(b-d)|^2}{2} \\
  &= \frac{(a+c)^2+(b+d)^2 - (a-c)^2-(b-d)^2}{2} \\
  &= 2(ac+bd)
  \end{align}\tag{5}\label{5}
  $$
  Meanwhile, the $\langle \psi|X|\psi\rangle$ is given by
  $$
  \begin{align}
  \langle \psi|X|\psi\rangle = \begin{pmatrix}
  \alpha^{*} & \beta^{*}
  \end{pmatrix}\begin{pmatrix}
  0 & 1 \\ 1 & 0
  \end{pmatrix}\begin{pmatrix}
  \alpha \\ \beta
  \end{pmatrix}  = \begin{pmatrix}
  \beta^{*} & \alpha^*
  \end{pmatrix}\begin{pmatrix}
  \alpha \\ \beta
  \end{pmatrix} = \alpha\beta^* + \alpha^*\beta
  \end{align}\tag{6}\label{6}
  $$
  According to eq. $\eqref{1}$​, we can re-write eq. $\eqref{6}$​ as
  $$
  \langle \psi|X|\psi\rangle = \alpha\beta^* + \alpha^*\beta =(a+ib)(c-id) + (a-ib)(c+id) = 2(ac+bd)\tag{7}\label{7}
  $$
  From eq. $\eqref{5}$ and eq. $\eqref{7}$, we have $\mathbb{E}(X) = \langle \psi|X|\psi\rangle$

* For observable $Y$​, the eigenvalues are $+1$​ and $-1$​, and the corresponding eigenvectors are 
  $$
  |v_1\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ i
  \end{pmatrix}, |v_2\rangle = \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ -i
  \end{pmatrix}\tag{8}
  $$
  Note that
  $$
  \begin{align}
  |0\rangle &= \begin{pmatrix}
  1 \\ 0
  \end{pmatrix} = \frac{1}{\sqrt{2}}\left[ \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ i
  \end{pmatrix} +  \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ -i
  \end{pmatrix}\right] = \frac{|v_1\rangle+|v_2\rangle}{\sqrt{2}}\tag{9a} \\
  |1\rangle &= \begin{pmatrix}
  0 \\ 1
  \end{pmatrix} = \frac{1}{\sqrt{2}}\left[ \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ i
  \end{pmatrix} -  \frac{1}{\sqrt{2}}\begin{pmatrix}
  1 \\ -i
  \end{pmatrix}\right] = \frac{-i(|v_1\rangle-|v_2\rangle)}{\sqrt{2}}\tag{9b}
  \end{align}
  $$
  We can re-write the quantum state as
  $$
  |\psi\rangle =\alpha |0\rangle+\beta|1\rangle = \alpha \frac{|v_1\rangle+|v_2\rangle}{\sqrt{2}}-i\beta\frac{|v_1\rangle-|v_2\rangle}{\sqrt{2}} = \frac{(\alpha-i\beta)|v_1\rangle + (\alpha+i\beta)|v_2\rangle}{\sqrt{2}}\tag{10}
  $$
  Thus, the probability of getting $|v_1\rangle$ is $|\alpha-i\beta|^2/2$,  the probability of getting $|v_2\rangle$ is $|\alpha+i\beta|^2/2$, and the expectation value of measuring $Y$ is given by
  $$
  \mathbb{E}(Y) =\frac{|\alpha-i\beta|^2}{2}\times 1 +  \frac{|\alpha+i\beta|^2}{2}\times (-1) = \frac{|\alpha-i\beta|^2 - |\alpha+i\beta|^2}{2}\tag{11}\label{11}
  $$
  According to eq. $\eqref{1}$, we can re-write eq. $\eqref{11}$ as
  $$
  \begin{align}
  \mathbb{E}(Y) &= \frac{|\alpha-i\beta|^2 - |\alpha+i\beta|^2}{2} \\
  &= \frac{|a+ib-ic+d|^2 - |a+ib+ic-d|^2}{2} \\
  &= \frac{|(a+d)+i(b-c)|^2 - |(a-d)+i(b+c)|^2}{2} \\
  &= \frac{(a+d)^2+(b-c)^2 - (a-d)^2-(b+c)^2}{2} \\
  &= 2(ad-bc)
  \end{align}\tag{12}\label{12}
  $$
  Meanwhile, the $\langle \psi|Y|\psi\rangle$ is given by
  $$
  \begin{align}
  \langle \psi|Y|\psi\rangle = \begin{pmatrix}
  \alpha^{*} & \beta^{*}
  \end{pmatrix}\begin{pmatrix}
  0 & -i \\ i & 0
  \end{pmatrix}\begin{pmatrix}
  \alpha \\ \beta
  \end{pmatrix}  = \begin{pmatrix}
  i\beta^{*} & -i\alpha^*
  \end{pmatrix}\begin{pmatrix}
  \alpha \\ \beta
  \end{pmatrix} = i\alpha\beta^* - i\alpha^*\beta
  \end{align}\tag{13}\label{13}
  $$
  According to eq. $\eqref{1}$​, we can re-write eq. $\eqref{13}$​ as
  $$
  \langle \psi|Y|\psi\rangle =i\alpha\beta^* - i\alpha^*\beta =i(a+ib)(c-id) - i(a-ib)(c+id) = 2(ad-bc)\tag{14}\label{14}
  $$
  From eq. $\eqref{12}$ and eq. $\eqref{14}$, we have $\mathbb{E}(Y) = \langle \psi|Y|\psi\rangle$
