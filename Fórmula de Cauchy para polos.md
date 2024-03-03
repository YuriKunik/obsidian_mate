
## Construcción

Sea $f$ con un [[Singularidad|polo de orden k]] entonces, $f(z)=(z-z_{0})^{k}h(z)$ con $h(z)$ holomorfa en todo $U$.  Esto nos dice que $h(z)$ tiene escritura como serie de potencias en $D_{r}(z_0)$.
$$
h(z)=\sum b_{n}(z-z_{0})^{n} 
$$
y 
$$
\begin{align}
b_{n} &= \frac{1}{2\pi i} \int_{\partial D_{\varepsilon}(z_0)} \frac{h(z)}{(z-z_{0})^{n}} \, dz  \\
	 & =  \frac{1}{2\pi i} \int_{\partial D_{\varepsilon}(z_0)} \frac{f(z)}{(z-z_{0})^{n+k}} \, dz  \\
	  &  = a_{n+k} 

\end{align}
$$

Entonces $(z-z_{0})^{k}b_{n}=b_{n-k}=a_{n}$
