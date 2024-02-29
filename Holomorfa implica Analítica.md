#complejo #integracion #diferenciación 
## Enunciado

Sean $f:U\to \mathbb{C}$ una [[Función holomorfa]], $z_{0}\in U$. Si $\overline{D_{r}(z_{0})}\subset U$ entonces para $z \in D_{r}(z_{0})$ vale $f(z)=\sum_{n\geq 0}a_{n}(z-z_{0})^{n}$, donde 
$$
a_{n}  = \frac{1}{2\pi i} \int_{\partial D_{r}(z_{0})} \frac{f(w)}{(w-z_{0})^{n+1}} \, dw.
$$
Además el [[Radio de convergencia]] de la serie es mayor o igual que $r$.

### Demostración

Dado $z \in D_{r}(z_{0})$ fijo, por la [[Fórmula de Cauchy]] sabemos que
$$
f(z)=\frac{1}{2\pi i}\int_{\partial D_{r}(z_{0})} \frac{f(w)}{w-z} \, dw.
$$
Por otra parte, $w \in \partial D_{r}(z_{0})$ con lo que 
$$\left\lvert  \frac{z-z_{0}}{w-z_{0}}  \right\rvert =  \frac{\lvert z-z_{0}\rvert}{r} := C <1.$$
Trabajando con la fórmula de Cauchy, podemos hacer aparecer una serie geométrica ([[fórmula de la serie geométrica]]) ya que $\lvert\frac{z-z_{0}}{w-z_{0}}  \rvert <1$:
$$
\begin{align}
f(z) & =\frac{1}{2\pi i}\int_{\partial D_{r}(z_{0})} \frac{f(w)}{w-z_{0}-(z-z_{0})} \, dw  \\
	 & = \frac{1}{2\pi i}\int_{\partial D_{r}(z_{0})} \frac{f(w)}{(w-z_{0})} \frac{1}{\left( 1-\frac{z-z_{0}}{w-z_{0}} \right)}\, dw  \\
	 & =\frac{1}{2\pi i}\int_{\partial D_{r}(z_{0})} \frac{f(w)}{(w-z_{0})} \sum_{n\geq 0} \left(\frac{z-z_{0}}{w-z_{0}} \right)^{n}
\end{align}
$$
Además, como $C < 1$ la serie [[Convergencia Uniforme|converge uniformemente]] respecto de $w$. Por lo que podemos usar [[Yoga de integración compleja#Pase de sumatorias en integrales]]. 

$$
f(z)=\sum_{n>0} \frac{1}{2\pi i} \int_{\partial D_{r}(z_{0})} \frac{f(w)}{w-z_{0}} \left( \frac{z-z_{0}}{w-z_{0}} \right)^{n} \, dw = \sum a_{n}  (z-z_{0})^{n}
$$


