#complejo #integracion #análisis 
## Definición

Dada una función continua $f:U\to \mathbb{C}$ y  $\gamma :[a,b]\to U$ de clase $C^1$, se define
$$
\int _{\gamma}f(z) \, dz = \int _{a}^b f(\gamma(z))\gamma \prime (z) \, dz. 
$$

si $\gamma$ es un [[Camino]], entonces 
$$
\int _{\gamma}f(z) \, dz = \sum_{j=0}^{N-1}\int _{a}^b f(\gamma_{j}(z))\gamma \prime_{j} (z) \, dz. 
$$

En cada uno de los casos anteriores

$$
\int_{a}^{b} F(t) \, dt = \int_{a}^{b} \Re(F(t)) \, dt + i \int_{a}^{b} \Im(F(t))\, dt.   
$$