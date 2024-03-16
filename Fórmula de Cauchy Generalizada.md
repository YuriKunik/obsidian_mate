
## Enunciado

Sea $f:U\to \mathbb{C}$ una [[Función holomorfa]], y $\gamma$ [[Homotopía entre curvas complejas|homotópica]] a $0$ en $U$. Para $z \notin \text{im}(\gamma)$ vale
$$
f(z)I(\gamma, z)= \frac{1}{2\pi i}\int_{\gamma} \frac{f(w)}{w-z} \, dw 
$$

## Demostración

Tomemos la función $g(w):= \frac{f(w)-f(z)}{w-z}$ sabemos que se extiende de manera holomorfa a $U$ por ser $f$ holomorfa. De esta forma
$$
\int_{\gamma}g(z) \, dz =0
$$
por el [[Teorema de Cauchy generalizado]]. 
Es decir
$$
\int_{\gamma} \frac{f(w)}{w-z} \, dw = \int_{\gamma} \frac{f(z)}{w-z}\, dw = f(z) \int_{\gamma} \frac{1}{w-z} \, dw 
$$ que dividiendo ambos lados de la igualdad por $2\pi i$ tenemos lo que queríamos ya que surge la fórmula del [[Indice de una curva]].