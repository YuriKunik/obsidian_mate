
# Primera versión (rectángulos)

## Enunciado

Sea $U$ abierto y $f:U\to \mathbb{C}$ holomorfa. Si $R\subset U$ es un rectángulo cerrado, entonces
$$
\int _{\partial R}f(z) \, dz =0 
$$
### Demostración

Dividamos el rectángulo $R$ en cuatro partes iguales de manera que:
$$
\int_{\partial R}f(z) \, dz = \sum_{j=1}^{4} \int_{\partial R_{j}}f(z) \, dz 
$$
![[Teorema de Cauchy 2024-02-28 21.20.14.excalidraw]]
Con esto, para el $j$ tal que la integración en módulo es mayor, se verifica
$$
\left\lvert  \int_{\partial R_{j} } f(z)\, dz   \right\rvert \geq \frac{1}{4} \left\lvert  \int_{\partial R} f(z) \, dz   \right\rvert 
$$

repitiendo este procedimiento para el $j$ donde pasaba esto, obtenemos una sucesión decreciente de rectángulos
$$
\dots \subset R^{2} \subset R^{1} \subset R. 
$$
tal que
$$
\text{Long}(\partial R^{k}) = \frac{1}{2^{k}}\text{Long}(\partial R).
$$
y

$$
\text{Diag}(\partial R^{k}) = \frac{1}{2^{k}}\text{Diag}(\partial R).
$$
Como $\mathbb{C}$ es completo y la familia $\{  R^{j} \}$ tiene la [[Propiedad de intersecciones finitas]], existe 
$$
\bigcap_{k\geq 1}R^{k}={z_{0}}
$$

Por ser $f$ holomorfa, dado $\varepsilon>0$ existe $\delta>0$ tal que, si $\lvert z-z_{0} \rvert<\delta$ entonces:
$$
\lvert f(z)-f(z_{0})-f^{\prime} (z_{0})(z-z_{0}) \rvert \leq \varepsilon \lvert z-z_{0} \rvert.
$$
Luego, podemos fijar $k_{0}$ tal que $D_{\delta}(z_{0})\subset R^{k_{0}}$. Como la función $g(z):= f^{\prime}(z_{0})(z-z_{0})+f(z_{0})$ tiene primitiva (es un polinomio de grado 1) entonces ([[Yoga de integración compleja#Integración de funciones continuas con primitiva|primitiva implica integra 0]])
$$
\begin{align}
\left\lvert  \int_{\partial R^{k}}f(z) \, dz   \right\rvert  &  = \left\lvert   \int_{\partial R^{k}} [f(z)-f(z_{0})-f^{\prime} (z_{0})(z-z_{0})] \, dz  \right\rvert  \\
 & \leq \varepsilon \text{máx}_{z \in \partial R^{k}} \lvert z-z_{0}  \rvert \text{Long}(\partial R^{k})  \\
	 & \leq \varepsilon \text{Diag}(\partial R^{k})\text{Long}(\partial R^{k}).
\end{align}
$$
para $k \geq k_{0}$.

Usando las desigualdades que fuimos consiguiendo nos queda,

$$
\begin{align}
\left\lvert  \int_{\partial R}f(z) \, dz   \right\rvert  &\leq 4^{k} \left\lvert  \int_{\partial R^{k}} f(z)\, dz   \right\rvert  \\
&\leq 4^{k}  \varepsilon \text{Diag}(\partial R^{k})\text{Long}(\partial R^{k})  \\
	 & \leq \frac{\varepsilon 4^{k}}{4^{k}} \text{Diag}(\partial R)\text{Long}(\partial R)  \\ \\
	 & \to 0
\end{align}
$$

## Corolarios

### Primitiva de holomorfas en un disco

Sean $D$ un disco abierto, $f:U\to \mathbb{C}$ una [[Función holomorfa]]. Entonces $f$ tiene primitiva en $D$.

#### Demostración

Por el siguiente [[Yoga de integración compleja#Condición suficiente para tener primitiva versión poligonales|resultado]], nos alcanza ver que toda integral sobre una curva poligonal cerrada contenida en $D$ es nula. Para esto, notemos que todo interior de una curva poligonal cerrada simple, se puede escribir como una unión de rectángulos $\{ R_{i} \}$ de forma tal que queden bien orientadas las curvas al hacerlo. Ilustramos esto con el siguiente gráfico
![[Teorema de Cauchy 2024-02-29 01.34.35.excalidraw]]

Así, tenemos
$$
\int_{\gamma}f(z) \, dz = \sum_{i=0}^n \int_{\partial R_{i}}f(z) \, dx  = 0
$$
por el teorema de Cauchy. Con esto sabemos que $f$ tiene primitiva en todo $D$.

### Caminos cerrados en discos de funciones holomorfas

Sean $D$ un disco abierto, $f:D\to \mathbb{C}$ una [[Función holomorfa]]. Entonces la integral sobre cualquier camino cerrado contenido en $D$ es nula.

#### Demostración

Por el resultado [[Teorema de Cauchy Primera versión#Primitiva de holomorfas en un disco|sobre las primitivas de holomorfas en un disco]] sabemos que $f$ tiene primitiva en $D$. Pero por [[Yoga de integración compleja#Integración de funciones continuas con primitiva]] tenemos el resultado.
