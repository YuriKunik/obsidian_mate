
## Enunciado

Sea $\rho$ el [[Radio de convergencia]] de la serie de potencias dada por $\{ a_{n} \}$ entonces:
1. Si $0 \leq r < \rho$ entonces $a_{n}z^n$ converge [[Convergencia Uniforme|uniformemente]] y [[Convergencia Absoluta|absolutamente]] en $\overline{D_{r}}$.
2. Si $r>\rho$ entonces la serie no converge para $\lvert z \rvert=r$

## Demostración

Dado $r < \rho$ podemos tomar $r < \tilde{r} <\rho$ con lo que
$$
a_{n} r^n = a_{n} \tilde{r}^n \frac{r^n}{\tilde{r}^n} 
$$
Los términos de la expresión cumplen que $a_{n} \tilde{r}^n$ es una sucesión acotada y que $\frac{r}{ \tilde{r}}<1$. Por lo que $\sum \lvert a_{n} \rvert r^n$ converge lo cual implica que $a_{n} z^n$ converge en $\overline{D_{r}}$ por [[Criterio suficiente para un radio de convergencia]].