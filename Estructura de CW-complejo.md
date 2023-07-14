#matemática #topoalg #definiciones #construcciones 

## Definición
Sea $X$ un espacio topológico. Una estructura de CW-complejo para X consiste en una filtración por subespacios:
$$
X^0\subset X^1\subset X^2\subset \dots \subset X
$$
donde:
1. $X^0$ es un subespacio discreto (llamamos a sus elementos 0-celdas).
2. Para todo $n,~X^n$ se obtiene de $X^{n-1}$ [[Adjunción de n-celdas|adjuntandole n-celdas]] (indexadas por cierto conjunto $J_n$)
3. $X = \bigcup_{n\leq 0} X^n$ con la topología final ($U \subset X$ es abierto si y solo si $U\cap X^n$ es abierto en $X^n$ para todo $n\leq0$)

A cada $X^n$ se le dice n-esqueleto de $X$