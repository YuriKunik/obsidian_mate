
## Enunciado

Si $A \subset \mathbb{R}^{n}$ es un [[conjunto elemental]], entonces $| A| = | A |_{e}$ ([[medida exterior de lesbegue]]).

## Demostración

Dado $A$, un conjunto elemental,  es claro que $|A| \leq |A|_{e}$ ya que $\cup_{i=1}^{n}B_{i} = A$ es un cubrimiento por cajas valido. Para la otra desigualdad dividamos por casos

### $A$ conjunto cerrado:

Al ser $A$ un conjunto elemental cerrado obtenemos directamente que es [[compacto]]. Por definición de la medida exterior podemos encontrar para todo $\varepsilon > 0$ un cubrimiento de cajas $(B_{j})_{j=1}^{\infty}$ tal que $A \subset \cup B_{j}$, $|A|_{e} + \varepsilon > \sum_{j}|B_{j}|$. Ademas, podemos agarrar cajas abiertas $B_{j}^{\prime}$ que difieran en medida de $B_{j}$ por $\frac{\varepsilon}{2^{j}}$, y que las contengan. Así tenemos que ha de existir una colección finita de cajas $B^{i}$ que cubran a $A$, de donde
$$
|A| \leq \sum_{i=1}^{n} |B^{i}| \leq \sum_{i=1}^{\infty} |B_{i}^{\prime }| \leq \sum_{i=1}^{\infty} |B_{i}| + \frac{\varepsilon}{2^{i}} \leq |A|_{e} + 2\varepsilon.
$$

### A conjunto arbitrario:

Supongamos que $A = B_{1} \cup \dots \cup B_{r}$ siendo esta su descomposición en cajas disjuntas. Tomando $B_{i}^{\prime} \subset B_{i}$, cajas cerradas con $|B_{i}| - \frac{\varepsilon}{r}<|B_{i}^{\prime}|$ su unión, $E = \cup B_{i}^{\prime}$, es cerrada por lo que vale el enunciado. Juntando todo tenemos:
$$
|A| = \sum |B_{i}| \leq \sum |B^{\prime }_{i}| + \varepsilon \leq |E| + \varepsilon \leq |A|_{e} + \varepsilon
$$

## Enunciado para sigma elementales

El resultado mas general se obtiene tomando límite y notando que todas las sumas parciales cumplen la desigualdad.