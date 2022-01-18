## Exercise 3.2.1

A general single qubit state $|\psi\rangle$ corresponds one point on the Bloch sphere with parameter $(\theta, \varphi)$, and the relation is given by
$$
|\psi\rangle = \cos\frac{\theta}{2} |0\rangle + \sin\frac{\theta}{2}e^{i\varphi}|1\rangle\tag{1}
$$
We can use the relation to find the $(\theta,\varphi)$ for a single qubit state. 

* For $|+\rangle$, we have
  $$
  |+\rangle = \frac{1}{\sqrt{2}}|0\rangle + \frac{1}{\sqrt{2}}|1\rangle = \cos\left(\frac{1}{2}\cdot\frac{\pi}{2}\right)|0\rangle + \sin\left(\frac{1}{2}\cdot\frac{\pi}{2}\right)e^{i0}|1\rangle \tag{2}
  $$
  Thus, the corresponding parameter for $|+\rangle$ is $(\pi/2, 0)$.

* For $|-\rangle$, we have
  $$
  |-\rangle = \frac{1}{\sqrt{2}}|0\rangle - \frac{1}{\sqrt{2}}|1\rangle = \cos\left(\frac{1}{2}\cdot\frac{\pi}{2}\right)|0\rangle + \sin\left(\frac{1}{2}\cdot\frac{\pi}{2}\right)e^{i\pi}|1\rangle \tag{3}
  $$
  where $e^{i\pi}+1 = 0$. Thus, the corresponding parameter for $|-\rangle$ is $(\pi/2, \pi)$.

