#análisis #series #complejo 

## Enunciado

Sean $f_{n}:U\to \mathbb{C}$ una sucesión de funciones tales que existen $A_{n}$ con $\lvert f_{n}(z) \rvert\leq A_{n}$ para todo $z\in U$. Si $\sum_{n}A_{n}< \infty$ entonces $\{ f_{n} \}$ [[Convergencia Uniforme|converge uniformemente]] y [[Convergencia Absoluta|absolutamente]].

## Demostración

Que converge absolutamente es directo por el [[Criterio de comparación]]. Para ver que converge uniformemente usamos que $S_{M}(z)$ es una [[Serie uniformemente de Cauchy]]: Dado $\varepsilon > 0$ fijamos $N_{0}$ tal que para $M > N >N_{0}$ valga $\sum_{n=N+1}^M A_{n} < \varepsilon$. Entonces 
$$
    \lvert S_{N}(z)-S_{M}(z) \rvert = \left\lvert  \sum_{n=N+1}^M f_{n}(z)  \right\rvert \leq \sum_{n=N+1}^M A_{n} < \varepsilon
$$