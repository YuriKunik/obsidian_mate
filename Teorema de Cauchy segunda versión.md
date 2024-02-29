
## Enunciado

Sea $U$ abierto y $f:U\to \mathbb{C}$ continua y una [[Función holomorfa]] en $U -\{ z_{0} \}$ para cierto $z_{0} \in U$. Si $R\subset U$ es un rectángulo cerrado, entonces
$$
\int_{\partial R}f(z) \, dz = 0
$$

### Demostración
si $z_{0} \notin R$, por [[Teorema de Cauchy Primera versión]], no tenemos que probar nada más. Si $z_{0} \in \mathbb{R}$, supongamos que está en interior.
Dado $\varepsilon > 0$ podemos dividir a $R$ en rectangulitos, con $z_{0} \in R_{0}$ uno de lados menores que $\varepsilon$.
![[Teorema de Cauchy segunda versión 2024-02-29 16.44.15.excalidraw]]
Entonces
$$
\int_{\partial R}f(z) \, dz = \sum_{j=0}^{8}\int_{\partial R_{j}}f(z) \, dz 
$$
pero para cada $j\neq {0}$ sabemos que es $0$ por la primera versión, por lo que nos queda
$$
\left\lvert  \int_{\partial R}f(z) \, dz   \right\rvert = \left\lvert  \int_{\partial R_{0}}f(z) \, dz   \right\rvert \leq 4 \varepsilon \lVert f|_{\partial R_{0}} \rVert _{\infty}
$$
que es claro que tiende a $0$ si tendemos el $\varepsilon$ a $0$.

## Corolarios

### Cauchy para funciones continuas y holomorfas salvo un punto en discos

Sea $D$ un disco y $f:D\to \mathbb{C}$ continua y holomorfa en $D-\{ z_{0} \}$. Entonces $f$ tiene primitiva en $D-\{ z_{0} \}$ y en particular, la integral de $f$ sobre cualquier curva cerrada contenida en $D-z_{0}$ es $0$.

### Un relajamiento de la versión anterior

Sea $D$ un disco y $f:D\to \mathbb{C}$  holomorfa en $D-\{ z_{0} \}$ tal que vale
$$
\lim_{ z \to z_{0} } (z-z_{0})f(z)=0.
$$
Entonces $f$ tiene primitiva en $D$ y en particular, la integral de $f$ sobre cualquier curva cerrada contenida en $D$ es $0$.