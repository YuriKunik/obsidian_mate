
## Enunciado

Sean $f:U\to \mathbb{C}$ una [[Función holomorfa]], $r > 0$ y $z_{0} \in\mathbb{C}$ tal que $\overline{D_{r}(z_{0})}\subset U$. Entonces, para todo $z \in D_{r}(z_{0})$
$$
f(z)= \frac{1}{2\pi i}\int_{\partial D_{r}(z_{0})} \frac{f(w)}{w-z} \, dw .
$$
### Demostración

Dado $z \in D_{r}(z_{0})$, consideremos un disco $D$ que contenga a $D_{r}(z_{0})$ la función
$$
g(w):=
\begin{cases}
\frac{f(w)-f(z)}{w-z}  & \text{si } w\neq z \\
f^{\prime} (w)  & \text{si } w=z
\end{cases}
$$
es claro que es continua en $D$ y holomorfa en $D-\{ z \}$. Entonces, por [[Teorema de Cauchy segunda versión#Cauchy para funciones continuas y holomorfas salvo un punto en discos]], vale que 
$$
\int_{\partial D_{r}(z_{0})}g(w) \, dw =0
$$
Es decir
$$
\int_{\partial D_{r}(z_{0})} \frac{f(w)}{w-z} \, dw = \int_{\partial D_{r}(z_{0})} \frac{f(z)}{w-z} dw = f(z)\int_{\partial D_{r}(z_{0})} \frac{1}{w-z}dw.
$$
de donde obtenemos la igualdad por el resultado [[Integral compleja de la función inversa]].