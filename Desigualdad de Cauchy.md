
## Enunciado

Dada $f:U\to \mathbb{C}$ una [[Función holomorfa]], $r>0$ y $z_{0} \in \mathbb{C}$ tal que $D_{r}(z_{0})\subset U$. Entonces
$$
\lvert a_{n}  \rvert = \left\lvert  \frac{1}{2 \pi i} \int_{\partial D_{r}(z_{0})} \frac{f(w)}{(w-z_{0})^{n+1}} \, dw   \right\rvert \leq \frac{M_{r}}{r^{n}}
$$

donde
$$
M_{r}:= \text{máx}_{z\in\partial D_{r}(z_{0})}\lvert f(z) \rvert .
$$

## Demostración

Usando la [[Fórmula de Cauchy]]:

$$
\begin{align}
\lvert a_{n}  \rvert  & \leq \frac{1}{2\pi } \frac{M_{r}}{r^{n+1}}  2\pi r\\
	 & = \frac{M_{r}}{r^{n}}
\end{align}
$$

Donde en la primera desigualdad usamos que $\lvert w-z_{0} \rvert = r$ para todo $w \in \partial D_{r}(z_{0})$ y la [[Yoga de integración compleja#Desigualdad integral]]. 
