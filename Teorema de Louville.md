
## Enunciado

Dada una [[Función entera]] $f:\mathbb{C}\to \mathbb{C}$ tal que existe $M$ que cumple
$$
\lvert f(z) \rvert \leq M
$$

implica que $f \equiv c$.

## Demostración

Al ser entera, sabemos que es [[Función analítica]] con [[Radio de convergencia]] infinito. Entonces se escribe como $f(z) = \sum a_{n}z^{n}$.
Por la [[Desigualdad de Cauchy]], para cada $n\geq 1$
$$
\lvert a_{n}  \rvert \leq \frac{M}{r^{n}} \to 0 \quad \text{cuando }\quad r\to \infty.
$$

Cosa que podemos hacer ya que $f$ es entera. Entonces $f(z)=a_{0}$.