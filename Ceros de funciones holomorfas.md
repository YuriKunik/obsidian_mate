
# Propiedades

## El conjunto de ceros tiene interior no vacío

Sea $U$ un conjunto abierto y conexo, $f:U\to \mathbb{C}$ una [[función holomorfa]]. Si $Z:=\{ z\in U : f(z)=0 \}$ tiene interior no vacío, entonces $f\equiv 0$ en $U$.

### Demostración

Sea $E:=\{ z \in U : f^{(n)}(z)=0 \quad \forall z \in U\}$. Veamos que $E$ es no vacío. Si $z_{0} \in Z^{\circ}$ entonces $f(z_{0})=0$. Ahora $f$ tiene desarrollo de potencias en $z_{0}$ por lo que vale, para cierto $r>0$ que
$$
f(z)=\sum_{n\geq 0}a_{n} (z-z_{0})^{n}
$$
con 
$$
a_{n} = \frac{1}{2\pi i}\int_{\partial D_{r}(z_{0})} \frac{f(w)}{(w-z_{0})^{n+1}} \, dw,
$$
por la [[Fórmula de Cauchy]]. La clave está en que, podemos tomar $r$ de forma tal que $\overline{D_{r}(z_{0})}\subset Z^{\circ}$, con lo que
$$
a_{n} = 0 \quad \forall n\in \mathbb{N}_{0}
$$
debido a que se anula la integral. Ahora que sabemos que $E$ es no vacío, tomemos un nuevo $z_{0}\in E$, entonces, en un radio $r$ $f$ tiene un desarrollo como serie de potencias
$$
f(z)=\sum_{n\geq 0} \frac{f^{(n)}(z_{0})}{n!} (z-z_{0})^{n} = 0.
$$
con lo cual $f$ es nula en todo $D_{r}(z_{0})$ que ya vimos que implica $D_{r}(z_{0})\subset Z^{\circ} \subset E$. Por otro lado es claro que $E$ es cerrado por ser
$$
E = \bigcap_{n\geq 0} (f^{(n)})^{-1}(0).
$$
donde cada intersecando es cerrado. Con esto tenemos que $E = U$ por ser $U$ conexo, y por lo tanto $f\equiv 0$.


### Corolario

Con $f:U\to \mathbb{C}$ una función holomorfa en $U$ abierto y conexo, si $f^{(n)}(z_{0})=0$ para algún $z_{0}\in U$, entonces $f\equiv 0$.


## Ceros son puntos aislados

Sea $f$ una función holomorfa en $U$ abierto y conexo que no es identicamente nula. Entonces sus ceros son puntos aislados.

### Demostración:

Sea $z_{0}$ un cero de $f$, entonces existe un $r>0$ tal que

$$
f(z)=\sum_{n\geq n_{0}} \frac{f^{(n)}(z_{0})}{n!}(z-z_{0})^{n}.
$$

con $f^{(n_{0})}(z_{0})\neq 0$. Así podemos separar a $f$ en
$$
\begin{align}
f(z) & = \frac{f^{(n_{0})}(z_{0})}{n_{0}!}(z-z_{0})^{n_{0}}+ \sum_{n\geq n_{0}+1} \frac{f^{(n)}(z_{0})}{n!}(z-z_{0})^{n} \\
	 & = (z-z_{0})^{n_{0}}\left(  \frac{f^{n_{0}}(z_{0})}{n_{0}!}+ \sum_{n\geq n_{0}+1} \frac{f^{(n)}(z_{0})}{n!} (z-z_{0})^{n-n_{0}}\right) \\
	
	 & = (z-z_{0})^{n_{0}}\left(  \frac{f^{n_{0}}(z_{0})}{n_{0}!}+ h(z) \right)
\end{align}
$$
con $n_{0}$ mínimo de forma que $f^{(n_{0})}(z_{0})\neq 0$. Así $h(z_{0})= 0$ y es holomorfa en $z_{0}$. Por continuidad, podemos conseguir un $\delta$ tal que para todo $z \in D_{\delta}(z_{0})$ 
$$
\lvert g(z) \rvert < \left\lvert  \frac{f^{(n_{0})}(z_{0})}{2 n_{0}!}  \right\rvert 
$$

no funciona la demo esta mintiendo.