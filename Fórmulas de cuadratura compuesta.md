
## Idea
Partimos el intervalo $[a,b]$ en subintervalos eligiendo puntos $a=x_{0} < x_{1},\dots x_{n}=b$.
Sabemos que
$$
\int_{a}^b f(x) \, dx = \sum_{i=0}^{n-1} \int _{x_{i}}^{x_{i+1}} f(x)\, dx .
$$
Con lo que, para cada $I_{i}(f)$ aplicamos una fórmula de cuadratura $Q_{i}(f)$ con su respectivo error $R_{j}(f)$. Obtenemos
$$
\int _{a}^b f(x) \, dx \sim \sum^{n-1}_{i=0}Q_{i}(f) \quad \text{con error} \quad R(f)=\sum^{n-1}_{i=0}R_{i}(f).
$$
## Estimación general del error.
Si cada cuadratura cumple las hipótesis del [[Error de cuadraturas|Teorema de error de cuadratura]]. Entonces, si $f \in C^{k+1}[a,b]$ y $h=máx_{j}{x_{j+1}-x_{j}}$ se tiene que 
$$
\lvert R(f) \rvert \leq \frac{(1+M)(b-a)}{(k+1)!}h^{k+1}\lVert f^{k+1} \rVert_{\infty}
$$