
## Definición

Sea $\mathcal{V}$ un [[Quantale]], y $\mathcal{X}$, $\mathcal{Y}$ $\mathcal{V}-$[[Categoría Enriquecida|categorías]]. Un $\mathcal{V}-$profuntor $\phi :\mathcal{X}\twoheadrightarrow \mathcal{Y}$ es un $\mathcal{V}$-[[Funtor Enriquecido|funtor]] $\phi:\mathcal{X}^{op} \times \mathcal{Y}\to \mathcal{V}$

## Observación

Estamos viendo al $\mathcal{V}-$funtor cayendo en $\mathcal{V}$ [[Categoría enriquecida en si misma|enriquecida en si mismo]].

## Definición equivalente
Ejercicio 4.9 7Sketches

Sabemos que $\phi$ es una función $\phi : ob(\mathcal{X}^{op} \times \mathcal{Y}) \to V$. Donde los objetos de $\mathcal{X} \times \mathcal{Y}$ son $ob(\mathcal{X})\times ob(\mathcal{Y})$. La condición que cumple, por otra parte, nos dice que
$$
(\mathcal{X}^{op}\times \mathcal{Y})((x,y), (x^{\prime}, y^{\prime })) \leq \mathcal{V}(\phi(x,y), \phi(x^{\prime }, y^{\prime }))
$$
Donde $\mathcal{V}(\phi(x,y), \phi(x^{\prime }, y^{\prime }))= \phi(x,y) \multimap\phi(x^{\prime}, y^{\prime})$  y $(\mathcal{X^{op}\times \mathcal{Y}})((x,y), (x^{\prime}, y^{\prime })) = \mathcal{X}(x^{\prime},x) \otimes \mathcal{Y}(y,y^{\prime})$ 

con lo cual la condición anterior es equivalente a 

$$
\mathcal{X}(x^{\prime },x) \otimes \mathcal{Y}(y,y^{\prime}) \leq\phi(x,y) \multimap\phi(x^{\prime}, y^{\prime})
$$

entonces, por [[Preorden monoidal simétrico cerrado|definición de elemento hom]], terminamos las equivalencias con

$$
\mathcal{X}(x^{\prime},x) \otimes \phi(x,y) \otimes \mathcal{Y}(y,y^{\prime}) \leq \phi(x^{\prime}, y^{\prime})
$$
## Coincidencia con la definición de [[Relación de factibilidad]]

Supongamos que $\mathcal{X}$ e $\mathcal{Y}$ son [[preorden|preordenes]], es decir $\text{Bool}-$categorías, si tomamos un $\text{Bool}$-profuntor $\phi$ de $\mathcal{X}$ a $\mathcal{Y}$, tenemos un $\text{Bool}$-[[Funtor Enriquecido|funtor]] $\phi:\mathcal{X}^{op}\times Y\to \text{Bool}$ que sabemos que coincide con una función monótona cuando los vemos como preordenes, con lo cual la definición coincide.