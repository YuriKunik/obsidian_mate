
## Módulo de fracciones
### Construcción

Sea $A$ un [[Anillo]] conmutativo, $S \subset A$ un [[Subconjunto multiplicativo]], $M$ un A-[[Módulo]], construyamos un nuevo $A$-módulo que contenga a todos los elementos de $M$ pero además cosas de la forma $\frac{m}{s}$. Para eso definamos una relación de equivalencia en el producto $M\times S$ de forma tal que:
$$
(m,s)\sim(m^{\prime},s^{\prime}) \iff \exists s^{\prime\prime} /  s^{\prime\prime} (s^{\prime}m - s m^{\prime}) = 0
$$
Con esto nos queda el morfismo cociente, $\pi: M\times S\to M\times S / \sim$
$$
\pi(m,s)= \frac{m}{s}
$$

Al conjunto $M\times S /\sim$ lo notamos $S^{-1}M$. Nos falta ver que esto es, en efecto, un $A$-módulos con
1. $\frac{m}{s}+\frac{m^{\prime}}{s^{\prime}}=\frac{s^{\prime}m+s m^{\prime}}{s^{\prime}s}$
2. $a\frac{m}{s}=\frac{am}{s}$

## Anillo de fracciones
En el caso de que $M$ sea un anillo llamamos a esto un anillo de fracciones