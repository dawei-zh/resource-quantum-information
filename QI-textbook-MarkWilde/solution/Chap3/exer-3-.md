## Exercise 3.6.4

Suppose that Alice and Bob share the state
$$
|\Phi^{+}\rangle = \frac{1}{\sqrt{2}}(|00\rangle + |11\rangle) = \frac{1}{\sqrt{2}}(|++\rangle + |--\rangle)\tag{1}
$$
The rule of playing CHSH game is, the referee send Alice and Bob a bit $x$ and $y$, respectively, then Alice and Bob send back a bit $a$ and $b$ to the referee, Alice and Bob win the game if $x\and y = a\oplus b$, where $\oplus$ means exclusive OR. The strategy is that:

* If Alice get $0$ and Bob get $0$, Alice measure $|\Phi^{+}\rangle$ in $Z$ basis and send $a=0$ if measuring $+1$, and $a=1$ when measure $-1$. For Bob, he needs to measure $|\Phi^{+}\rangle$ in the $(X+Z)/\sqrt{2}$ basis and send $b=0$ if measuring $+1$, and $b=1$ when measure $-1$.
* If Alice get $0$ and Bob get $1$, Alice measure $|\Phi^{+}\rangle$ in $Z$ basis and send $a=0$ if measuring $+1$, and $a=1$ when measure $-1$. For Bob, he needs to measure $|\Phi^{+}\rangle$ in the $(Z-X)/\sqrt{2}$ basis and send $b=0$ if measuring $+1$, and $b=1$ when measure $-1$.
* If Alice get $1$ and Bob get $0$, Alice measure $|\Phi^{+}\rangle$ in $X$ basis and send $a=0$ if measuring $+1$, and $a=1$ when measure $-1$. For Bob, he needs to measure $|\Phi^{+}\rangle$ in the $(X+Z)/\sqrt{2}$ basis and send $b=0$ if measuring $+1$, and $b=1$ when measure $-1$.
* If Alice get $1$ and Bob get $1$, Alice measure $|\Phi^{+}\rangle$ in $X$ basis and send $a=0$ if measuring $+1$, and $a=1$ when measure $-1$. For Bob, he needs to measure $|\Phi^{+}\rangle$ in the $(Z-X)/\sqrt{2}$ basis and send $b=0$ if measuring $+1$, and $b=1$ when measure $-1$.

Here we will estimate the probability of winning the game for each case. Firstly, let's get the basis of $(X+Z)/\sqrt{2}$ and $(Z-X)/\sqrt{2}$. The eigenvalue of $(X+Z)/\sqrt{2}$ can be obtained by
$$
\left|\frac{X+Z}{\sqrt{2}} - \lambda I\right|= \begin{vmatrix}
1/\sqrt{2}-\lambda & 1/\sqrt{2} \\ 1/\sqrt{2} & -1/\sqrt{2}-\lambda 
\end{vmatrix} = \lambda^2 - 1  = 0 \iff \lambda = \pm 1\tag{2}
$$
The corresponding eigenvectors are given by
$$
\begin{align}
|v_1\rangle &= \cos\frac{\pi}{8}|0\rangle + \sin\frac{\pi}{8}|1\rangle \text{ for }\lambda = 1 \tag{3a}\label{3a}\\
|v_2\rangle &= \sin\frac{\pi}{8}|0\rangle - \cos\frac{\pi}{8}|1\rangle \text{ for }\lambda = -1 \tag{3b}\label{3b}
\end{align}
$$
The eigenvalue of $(Z-X)/\sqrt{2}$ can be obtained by
$$
\left|\frac{Z-X}{\sqrt{2}} - \lambda I\right|= \begin{vmatrix}
1/\sqrt{2}-\lambda & -1/\sqrt{2} \\ -1/\sqrt{2} & -1/\sqrt{2}-\lambda 
\end{vmatrix} = \lambda^2 - 1  = 0 \iff \lambda = \pm 1\tag{4}
$$
The corresponding eigenvectors are given by
$$
\begin{align}
|v_1\rangle &= -\cos\frac{\pi}{8}|0\rangle + \sin\frac{\pi}{8}|1\rangle \text{ for }\lambda = 1 \tag{5a}\label{5a}\\
|v_2\rangle &= \sin\frac{\pi}{8}|0\rangle + \cos\frac{\pi}{8}|1\rangle \text{ for }\lambda = -1 \tag{5b}\label{5b}
\end{align}
$$
In the appendix I will verify eq. $\eqref{3a}-\eqref{3b}$ and eq. $\eqref{5a}-\eqref{5b}$ are the eigenvectors for $(X+Z)/\sqrt{2}$ and $(Z-X)/\sqrt{2}$, respectively. 

Then we need to calculate the probability of winning the game for each case. 

* If $x=0$ and $y=0$, $x\and y = 0$

  *  If Alice get $|0\rangle$ and $a=0$, then Bob should measure $|0\rangle$ in $(X+Z)\sqrt{2}$ basis. From eq. $\eqref{3a}-\eqref{3b}$, we could solve the equation and get
    $$
    |0\rangle = \cos\frac{\pi}{8} |v_1\rangle + \sin\frac{\pi}{8}|v_2\rangle\tag{6}\label{6}
    $$
    To make sure $a\oplus b = 0$, we need to measure $|v_1\rangle$ with $\lambda=1$ then $b=0$ to win the game; so the probability of getting $|v_1\rangle$ and winning the game is $\cos^2(\pi/8)$.

  * If Alice get $|1\rangle$ and $a=1$, then Bob should measure $|1\rangle$ in $(X+Z)\sqrt{2}$ basis. From eq. $\eqref{3a}-\eqref{3b}$, we could solve the equation and get
    $$
    |1\rangle = \sin\frac{\pi}{8} |v_1\rangle - \cos\frac{\pi}{8}|v_2\rangle\tag{7}\label{7}
    $$
    To make sure $a\oplus b = 0$, we need to measure $|v_2\rangle$ with $\lambda=-1$ then $b=1$ to win the game; so the probability of getting $|v_2\rangle$ and winning the game is $\cos^2(\pi/8)$.

* If $x=0$ and $y=1$, $x\and y = 0$

  *  If Alice get $|0\rangle$ and $a=0$, then Bob should measure $|0\rangle$ in $(Z-X)\sqrt{2}$ basis. From eq. $\eqref{5a}-\eqref{5b}$, we could solve the equation and get
    $$
    |0\rangle = -\cos\frac{\pi}{8} |v_1\rangle + \sin\frac{\pi}{8}|v_2\rangle\tag{8}\label{8}
    $$
    To make sure $a\oplus b = 0$, we need to measure $|v_1\rangle$ with $\lambda=1$ then $b=0$ to win the game; so the probability of getting $|v_1\rangle$ and winning the game is $\cos^2(\pi/8)$.

  * If Alice get $|1\rangle$ and $a=1$, then Bob should measure $|1\rangle$ in $(Z-X)\sqrt{2}$ basis. From eq. $\eqref{5a}-\eqref{5b}$, we could solve the equation and get
    $$
    |1\rangle = \sin\frac{\pi}{8} |v_1\rangle + \cos\frac{\pi}{8}|v_2\rangle\tag{9}\label{9}
    $$
    To make sure $a\oplus b = 0$, we need to measure $|v_2\rangle$ with $\lambda=-1$ then $b=1$ to win the game; so the probability of getting $|v_2\rangle$ and winning the game is $\cos^2(\pi/8)$.

* If $x=1$ and $y=0$, $x\and y = 0$

  *  If Alice get $|+\rangle$ and $a=0$, then Bob should measure $|+\rangle$ in $(Z-X)\sqrt{2}$ basis. From eq. $\eqref{3a}-\eqref{3b}$, eq. $\eqref{6}-\eqref{7}$ and eq. $\eqref{a2}$, we could get
    $$
    \begin{align}
    |+\rangle &= \frac{1}{\sqrt{2}}\left[\cos\frac{\pi}{8}+\sin\frac{\pi}{8}\right] |v_1\rangle + \frac{1}{\sqrt{2}}\left[\sin\frac{\pi}{8} - \cos\frac{\pi}{8}\right]|v_2\rangle  \\
    &= \cos\frac{\pi}{8}|v_1\rangle - \sin\frac{\pi}{8}|v_2\rangle
    \end{align}\tag{10}
    $$
    To make sure $a\oplus b = 0$, we need to measure $|v_1\rangle$ with $\lambda=1$ then $b=0$ to win the game; so the probability of getting $|v_1\rangle$ and winning the game is $\cos^2(\pi/8)$.

  * If Alice get $|-\rangle$ and $a=1$, then Bob should measure $|-\rangle$ in $(Z-X)\sqrt{2}$ basis. From eq. $\eqref{3a}-\eqref{3b}$, eq. $\eqref{6}-\eqref{7}$ and eq. $\eqref{a2}$, we could get
    $$
    \begin{align}
    |-\rangle &= \frac{1}{\sqrt{2}}\left[\cos\frac{\pi}{8}-\sin\frac{\pi}{8}\right] |v_1\rangle + \frac{1}{\sqrt{2}}\left[\sin\frac{\pi}{8} + \cos\frac{\pi}{8}\right]|v_2\rangle  \\
    &= \sin\frac{\pi}{8}|v_1\rangle + \cos\frac{\pi}{8}|v_2\rangle
    \end{align} \tag{11}
    $$
    To make sure $a\oplus b = 0$, we need to measure $|v_2\rangle$ with $\lambda=-1$ then $b=1$ to win the game; so the probability of getting $|v_2\rangle$ and winning the game is $\cos^2(\pi/8)$.

* If $x=1$ and $y=1$, $x\and y = 1$

  *  If Alice get $|+\rangle$ and $a=0$, then Bob should measure $|+\rangle$ in $(Z-X)\sqrt{2}$ basis. From eq. $\eqref{5a}-\eqref{5b}$, eq. $\eqref{8}-\eqref{9}$ and eq. $\eqref{a2}$, we could get
    $$
    \begin{align}
    |+\rangle &= \frac{1}{\sqrt{2}}\left[-\cos\frac{\pi}{8}+\sin\frac{\pi}{8}\right] |v_1\rangle + \frac{1}{\sqrt{2}}\left[\sin\frac{\pi}{8} + \cos\frac{\pi}{8}\right]|v_2\rangle  \\
    &= -\sin\frac{\pi}{8}|v_1\rangle + \cos\frac{\pi}{8}|v_2\rangle
    \end{align}\tag{12}
    $$
    To make sure $a\oplus b = 1$, we need to measure $|v_2\rangle$ with $\lambda=-1$ then $b=1$ to win the game; so the probability of getting $|v_2\rangle$ and winning the game is $\cos^2(\pi/8)$.

  * If Alice get $|-\rangle$ and $a=1$, then Bob should measure $|-\rangle$ in $(Z-X)\sqrt{2}$ basis. From eq. $\eqref{5a}-\eqref{5b}$, eq. $\eqref{8}-\eqref{9}$ and eq. $\eqref{a2}$, we could get
    $$
    \begin{align}
    |+\rangle &= \frac{1}{\sqrt{2}}\left[-\cos\frac{\pi}{8}-\sin\frac{\pi}{8}\right] |v_1\rangle + \frac{1}{\sqrt{2}}\left[\sin\frac{\pi}{8} - \cos\frac{\pi}{8}\right]|v_2\rangle  \\
    &= -\cos\frac{\pi}{8}|v_1\rangle - \sin\frac{\pi}{8}|v_2\rangle
    \end{align}\tag{13}
    $$
    To make sure $a\oplus b = 1$, we need to measure $|v_1\rangle$ with $\lambda=1$ then $b=0$ to win the game; so the probability of getting $|v_1\rangle$ and winning the game is $\cos^2(\pi/8)$.

Therefore, the probability of winning the game is $\cos^2(\pi/8)$.

#### Appendix

To verify eq. $\eqref{3a}$, we have
$$
\begin{align}
\frac{X+Z}{\sqrt{2}}|v_1\rangle &=\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} \begin{pmatrix}\cos\pi/8 \\ \sin\pi/8\end{pmatrix}=  \frac{1}{\sqrt{2}}\begin{pmatrix}\cos\pi/8 + \sin\pi/8\\ \cos\pi/8 - \sin\pi/8\end{pmatrix}
\end{align}\tag{A1}\label{a1}
$$
Note that 
$$
\begin{align}
\frac{1}{\sqrt{2}}\left(\cos\frac{\pi}{8} + \sin\frac{\pi}{8}\right) = \left(\cos\frac{\pi}{4}\cos\frac{\pi}{8} + \sin\frac{\pi}{4}\sin\frac{\pi}{8}\right) = \cos\left(\frac{\pi}{4} - \frac{\pi}8\right) = \cos\left(\frac{\pi}8\right) \\

\frac{1}{\sqrt{2}}\left(\cos\frac{\pi}{8} - \sin\frac{\pi}{8}\right) = \left(\cos\frac{\pi}{4}\cos\frac{\pi}{8} - \sin\frac{\pi}{4}\sin\frac{\pi}{8}\right) = \cos\left(\frac{\pi}{4} + \frac{\pi}8\right) = \sin\left(\frac{\pi}8\right) 
\end{align}\tag{A2}\label{a2}
$$
So eq. $\eqref{a1}$​ becomes 
$$
\frac{X+Z}{\sqrt{2}}|v_1\rangle =\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} \begin{pmatrix}\cos\pi/8 \\ \sin\pi/8\end{pmatrix}=  \begin{pmatrix}\cos\pi/8 \\ \sin\pi/8\end{pmatrix}\tag{A3}
$$
and thus we verify eq. $\eqref{3a}$.

To verify eq. $\eqref{3b}$, we have
$$
\begin{align}
\frac{X+Z}{\sqrt{2}}|v_2\rangle &=\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} \begin{pmatrix}\sin\pi/8 \\ -\cos\pi/8\end{pmatrix}=  \frac{1}{\sqrt{2}}\begin{pmatrix}\sin\pi/8- \cos\pi/8 \\ \cos\pi/8 + \sin\pi/8\end{pmatrix}
\end{align}\tag{A4}\label{a4}
$$
From eq. $\eqref{a2}$, eq. $\eqref{a4}$​ becomes 
$$
\frac{X+Z}{\sqrt{2}}|v_2\rangle =\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & 1 \\ 1 & -1
\end{pmatrix} \begin{pmatrix}\sin\pi/8 \\ -\cos\pi/8\end{pmatrix}=  \begin{pmatrix}-\sin\pi/8 \\ \cos\pi/8\end{pmatrix}\tag{A5}
$$
and thus we verify eq. $\eqref{3b}$.

To verify eq. $\eqref{5a}$, we have
$$
\begin{align}
\frac{Z-X}{\sqrt{2}}|v_1\rangle &=\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & -1 \\ -1 & -1
\end{pmatrix} \begin{pmatrix}-\cos\pi/8 \\\sin\pi/8 \end{pmatrix}=  \frac{1}{\sqrt{2}}\begin{pmatrix}-\sin\pi/8- \cos\pi/8 \\ \cos\pi/8 - \sin\pi/8\end{pmatrix}
\end{align}\tag{A6}\label{a6}
$$
From eq. $\eqref{a2}$, eq. $\eqref{a6}$​ becomes 
$$
\frac{Z-X}{\sqrt{2}}|v_1\rangle =\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & -1 \\ -1 & -1
\end{pmatrix} \begin{pmatrix}-\cos\pi/8 \\ \sin\pi/8\end{pmatrix}=  \begin{pmatrix}-\cos\pi/8 \\ \sin\pi/8\end{pmatrix}\tag{A7}
$$
and thus we verify eq. $\eqref{5a}$.

To verify eq. $\eqref{5b}$, we have
$$
\begin{align}
\frac{Z-X}{\sqrt{2}}|v_2\rangle &=\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & -1 \\ -1 & -1
\end{pmatrix} \begin{pmatrix}\sin\pi/8 \\\cos\pi/8 \end{pmatrix}=  \frac{1}{\sqrt{2}}\begin{pmatrix}\sin\pi/8- \cos\pi/8 \\ -\cos\pi/8 - \sin\pi/8\end{pmatrix}
\end{align}\tag{A8}\label{a8}
$$
From eq. $\eqref{a2}$, eq. $\eqref{a8}$​ becomes 
$$
\frac{Z-X}{\sqrt{2}}|v_2\rangle &=\frac{1}{\sqrt{2}}
\begin{pmatrix}
1 & -1 \\ -1 & -1
\end{pmatrix} \begin{pmatrix}\sin\pi/8 \\\cos\pi/8 \end{pmatrix}=  \begin{pmatrix}-\sin\pi/8 \\ -\cos\pi/8\end{pmatrix}\tag{A9}
$$
and thus we verify eq. $\eqref{5b}$.
