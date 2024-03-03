
## Enunciado

Sea $f:U-\{ z_{0} \}\to \mathbb{C}$ una [[Función holomorfa]] con una [[Singularidad]] esencial en $z_{0}$. Entonces, para todo $\varepsilon >0$ tal que $D_{\varepsilon}(z_{0})\subset U$, $f(D_{\varepsilon}(z_{0})-\{ z_{0} \})$  es denso en $\mathbb{C}$.

## Demostración

Supongamos que existe $\varepsilon$ tal que la imagen de $D_{\varepsilon}(z_{0})-\{  z_{0}\}$ no es densa. Esto implicaría que exista una bola $D_{r}(w)$ que no interseque a la imagen de $D_{\varepsilon}(z_{0})-\{ z_{0} \}$. Así podemos definir $g(z)= \frac{1}{f(z)-w}$ que es holomorfa en $D_{\varepsilon}(z_{0})-\{ z_{0} \}$. Además $\lvert f(z)-w \rvert \geq r$ por lo que $\lvert g(z) \rvert\leq \frac{1}{r}$. Esto implica que 
$$
\lim_{ z \to z_{0} } (z-z_{0})g(z)=0
$$
por lo que tiene una singularidad evitable en $z_{0}$, lo cual nos dice que es holomorfa en $D_{\varepsilon}(z_0)$. Como $g$ no es constante (ya que entonces $z_{0}$ no sería una singularidad esencial de $f$), podemos escribir $g(z)=(z-z_{0})^{k}h(z)$ con $h(z_{0})\neq 0$. Entonces 
$$
f(z)=g(z)+w= \frac{1}{(z-z_{0})^{k}h(z)} + w
$$
que implica tener
$$
\lim_{ z \to z_{0} } (z-z_{0})^{k+1}f(z)=0
$$
lo cual es absurdo ya que $z_{0}$ no era un polo de orden $k$.

## Corolario

Sea $z_{0}$ una singularidad esencial de $f$ y $w \in \hat{\mathbb{C}}$, entonces existe una sucesión ${z_{n}}$ tal que $f(z_{n}) \to w$.

### Demostración

Si $w\neq \infty$ tomamos $z_{n} \in D_{\frac{1}{n}}(z_0)-\{ z_{0} \}$ tal que $f(z_{n})\in D_{\frac{1}{n}}(w)$. Si $w =\infty$ tomamos $z_{n}$ del mismo lugar pero tal que $f(z_{n})\in D_{1}(n)$.



