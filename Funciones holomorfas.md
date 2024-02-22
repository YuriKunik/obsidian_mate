
## Definición

Sean $U \subset \mathbb{C}$ abierto, $z_{0}\in U$. Una función $f:U\to \mathbb{C}$ se dice derivable en $z_{0}$ si existe
$$
\lim_{ z \to z_{0} } \frac{f(z)-f(z_{0})}{z-z_{0}}
$$
En tal caso dicho límite se llama derivada de $f$ en $z_{0}$ y se denota $f^{\prime} (z_{0})$.
Si $f$ es diferenciable en un entorno de $z_{0}$ entonces se dice que es **holomorfa** en $z_{0}$. 

## Equivalencia

La función $f$ es derivable en $z_{0}$ si y solo si existe $\alpha \in \mathbb{C}$ y $R:U\to \mathbb{C}$ tales que
$$
f(z)=f(z_{0})+\alpha(z-z_{0})+R(z).
$$
con
$$
\lim_{ z \to z_{0} } \frac{R(z)}{z-z_{0}} = 0
$$
### Demostración

#### $1 \implies 2$

Tomemos $\alpha = f^{\prime} (z_{0})$ y $R(z)=f(z)-f(z_{0})-\alpha(z-z_{0})$. Es claro que $f(z)$ cumple la igualdad, veamos que el límite tiende a 0.
$$
\begin{align}
\lim_{ z \to z_{0} } \frac{f(z)-f(z_{0})-\alpha(z-z_{0})}{z-z_{0}} &= \lim_{ z \to z_{0} } \frac{f(z)-f(z_{0})}{z-z_{0}} - f^{\prime} (z_{0}) \\
     & = 0
\end{align}
$$
#### $2 \implies 1$

Para la vuelta, observemos que
$$
\begin{align}
0  &  = \lim_{ z \to z_{0} } \frac{R(z)}{z-z_{0}}  \\
     & = \lim_{ z \to z_{0} }  \frac{f(z)-f(z_{0})+\alpha(z-z_{0})}{z-z_{0}} \\
     & = \lim_{ z \to z_{0} } \frac{f(z)-f(z_{0})}{z-z_{0}} - \alpha
\end{align}
$$
Con lo cual, existe el cociente incremental y es igual a $\alpha$.
$\square$

## Propiedades extras

Valen

1. La regla de la suma, el producto y de la cadena.
2. Si $f$ es derivable en $z_{0}$ entonces es continua en $z_{0}$
3. Si $f$ y $g$ son derivables en $z_{0}$ y $g^\prime (z_{0})\neq 0$ entonces 
$$
\lim_{ z \to z_{0} } \frac{f(z_{0})}{g(z_{0})}= \frac{f^\prime(z_{0})}{g^\prime (z_{0})}
$$

