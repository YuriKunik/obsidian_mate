
## Enunciado

Dado $\mathcal{V}$ un [[Preorden monoidal simétrico cerrado]], podemos ver a $\mathcal{V}$ [[Categoría Enriquecida|enriquecida]] en si misma.

## Demostración
Necesitamos elegir un elemento $\mathcal{V}(x,y):=x\multimap y$. Veamos que esto satisface las condiciones para una categoría enriquecida

### $I\leq \mathcal{V}(x,x)$

Sabemos que $I\otimes x\leq x$ y por lo tanto, $I\leq ( x\multimap x)$ usando la definición del elemento $x \multimap x$.

### $\mathcal{V}(x,y)\otimes \mathcal{V}(y,z)\leq \mathcal{V}(x,z)$

esto sabemos que es cierto por 
![[Yoga de preordenes monoidales simétricos cerrados#$(u multimap v) otimes(v multimap w) leq (u multimap w)$|el siguiente resultado]].

