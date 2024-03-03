
## Enunciado

Sea $z_{0}\in\mathbb{C}$, $r, R$ tales que $r<R$, $f:A:=\{ z: r< \lvert z-z_{0} \rvert<R \}\to \mathbb{C}$ una [[Función holomorfa]]. Entonces existen únicos, $a_{n} \in \mathbb{C}$ tales que
$$
f(z)=\sum_{n\in\mathbb{Z}}a_{n} (z-z_{0})^{n}, \quad z\in A
$$
Además, para todo $n \in\mathbb{Z}$ y para todo $\tilde{r} \in (r,R)$ vale

$$
a_{n} = \frac{1}{2\pi i} \int_{\partial D_{\tilde{r}}(z_0)} \frac{f(z)}{(z-z_{0})^{n+1}} \, dz 
$$

## Demostración

Dado $z\in A$, fijemos $\tilde{r}$ y $\tilde{R}$ taels que $r<\tilde{r}<\lvert z-z_{0} \rvert<\tilde{R}<R$ y una curva $\gamma$ de la siguiente forma

![[Series de Laurent 2024-03-02 22.50.59.excalidraw]]

Como $I(\gamma, z)=1$ y las integrales sobre el segmento se cancelan, la [[Fórmula generalizada de Cauchy]]  nos dice que

$$
f(z)=\frac{1}{2\pi i}\int_{\gamma} \frac{f(w)}{w-z} \, dw = \frac{1}{2\pi i} \left( \int_{\lvert w-z_{0} \rvert = R } \frac{f(z)}{w-z}\, dw  - \int_{\lvert w-z_{0} \rvert = r } \, \frac{f(w)}{w-z} dw \right)
$$

Veamos los dos términos de la resta por separado; para la primera integral, el hecho de que $\lvert z-z_{0} \rvert< \lvert w-z_{0} \rvert= \tilde{R}$ nos permite escribir
$$

$$