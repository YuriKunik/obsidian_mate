
#calculonumerico

## Preparación
Notaremos a la integral de $f$ en $[a,b]$ $I(f)$ y al error cometido por una regla de cuadratura por $R(f)=I(f)-Q(f)$.

## Teorema

Dada una regla de cuadratura $Q(f)$ en el intervalo $[a,b]$ tal que
1. $Q$ es lineal.
2. $Q$ tiene [[Grado de exactitud de una cuadratura|grado de exactitud]] k.
3. $\lvert Q(f) \rvert\leq M(b-a)\lVert f \rVert_{\infty}$
Entonces, si $f \in C^{k+1}[a,b]$, se tiene
$$
\lvert R(f) \rvert \leq \frac{(1+M)(b-a)^{k+2}}{(k+1)!} \rVert f^{k+1}\lVert_{\infty} 
$$
### Demostración
Empecemos trabajando con $\lvert R(f)  \rvert$. Tomemos el polinomio de taylor de grado $k$, $p_{k}$ centrado en algún punto del intervalo. Entonces
$$
\begin{align}
\lvert R(f) \rvert  & = \lvert Q(f)-I(f) \rvert  \\
     & = \lvert Q(f)-I(f)  \rvert  \\
     & = \lvert Q(f)-Q(p_{k})+Q(p_{k}) - I(f) \rvert  \\
     & \leq \lvert Q(f-p_{k}) \rvert  + \lvert I(p_{k}-f) \rvert  \\
     & \leq M(b-a)\lVert f-p_{k}\rVert_{\infty} + (b-a) \lVert f-p_{k}\rVert_{\infty} \\
     & \leq (M+1) \frac{(b-a)^{k+2}}{(k+1)!} \lVert f^{k+1} \rVert_{\infty}
\end{align}
$$
Donde usamos todas las propiedades de $Q$ además de una cota del error del polinomio interpolador de taylor.


















