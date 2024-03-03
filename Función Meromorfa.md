
## Definición

Sea $U \subset \mathbb{C}$ abierto. Una función es **meromorfa** en $U$ si existe $S \subset U$ discreto tal que $f:U-S\to \mathbb{C}$ es una [[Función holomorfa]] y todos los elementos de $S$ son a lo sumo [[Singularidad|polos]] de $f$.

$f$ se dice **meromorfa en $\hat{\mathbb{C}}$** si existe $S \subset \mathbb{C}$ finito tal que $f:\mathbb{C}-S\to \mathbb{C}$ es holomorfa y todos los elementos de $S\cup \{ \infty \}$ son a lo sumo polos.

## Idea

### Función meromorfa con finitas singularidades.

Si el conjunto $S$ es finito y tenemos una función meromorfa en $U$, entonces, siendo $S=\{ z_{i} \}$ y $k_{i}$ el orden de cada polo de $f$. Entonces
$$
g(z):= f(z)\prod_{i=0}(z-z_{i} )^{k_{i} }
$$

es holomorfa, por lo que $f$ es, 
$$
f(z)=\frac{g(z)}{q(z)}
$$
con $q(z)$ un polinomio.

### Función meromorfa en $\hat{\mathbb{C}}$.

Tomando $g(z)$ igual que antes, nos queda que $g$ es una [[Función entera]]. Como $f\left( \frac{1}{z} \right)$ tiene límite finito para $z\to {0}$ ($\infty$ es una singularidad evitable), entonces, existen $C$, $R$ tales que $\lvert f(w) \rvert\leq C$ con $\lvert  w\rvert > R$. 
Con esto tenemos que
$$
\lvert g(w) \rvert \leq C \lvert q(w) \rvert 
$$
por lo que $g$ es un polinomio ([[Teorema de Louville generalizado]]).
Si $f$ tiene un polo en $\infty$ entonces
$$
g\left( \frac{1}{z} \right) = f\left( \frac{1}{z} \right) q\left( \frac{1}{z} \right) \to \infty
$$
con lo que $g$ también tenía un polo en $\infty$ con lo cual, al ser una función entera, es un polinomio. Así finalizamos en que
si $f$ es una función meromorfa en $\hat{\mathbb{C}}$ entonces es una función racional.
