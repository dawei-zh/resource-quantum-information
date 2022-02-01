## Exercise 3.6.1

Consider the composite quantum state $|\Phi^{+}\rangle_{AB}$,
$$
|\Phi^{+}\rangle_{AB} = \frac{1}{\sqrt{2}}(|0\rangle_{A}|0\rangle_{B} + |1\rangle_{A}|1\rangle_{B})\tag{1}\label{1}
$$
The $|+\rangle$ and $|-\rangle$ states are given by
$$
|+\rangle = \frac{1}{\sqrt{2}}(|0\rangle + |1\rangle), |-\rangle = \frac{1}{\sqrt{2}}(|0\rangle - |1\rangle)\\ \iff |0\rangle = \frac{1}{\sqrt{2}}(|+\rangle + |-\rangle), |1\rangle = \frac{1}{\sqrt{2}}(|+\rangle - |-\rangle)\tag{2}\label{2}
$$
Substitute eq. $\eqref{2}$ into eq. $\eqref{1}$, we have
$$
\begin{align}
|\Phi^{+}\rangle_{AB} =& \frac{1}{\sqrt{2}}\left[\frac{1}{\sqrt{2}}(|+\rangle_{A} + |-\rangle_{A})\otimes \frac{1}{\sqrt{2}}(|+\rangle_{B} + |-\rangle_{B}) \right.\\
&+ \left.\frac{1}{\sqrt{2}}(|+\rangle_{A} - |-\rangle_{A})\otimes \frac{1}{\sqrt{2}}(|+\rangle_{B} - |-\rangle_{B}) \right]\\
=& \frac{1}{2\sqrt{2}}\left(|+\rangle_{A}|+\rangle_{B} + |+\rangle_{A}|-\rangle_{B} + |-\rangle_{A}|+\rangle_{B} + |-\rangle_{A}|-\rangle_{B} \right. \\
&+ |+\rangle_{A}|+\rangle_{B} - |+\rangle_{A}|-\rangle_{B} - |-\rangle_{A}|+\rangle_{B} + |-\rangle_{A}|-\rangle_{B}) \\
=& \frac{1}{2\sqrt{2}}(2|+\rangle_{A}|+\rangle_{B} + 2|-\rangle_{A}|-\rangle_{B}) \\
=& \frac{1}{\sqrt{2}}(|+\rangle_{A}|+\rangle_{B} + |-\rangle_{A}|-\rangle_{B}) 
\end{align}\tag{3}
$$
