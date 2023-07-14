#matemática #definiciones #numerico
## Definición
Dada la tabla de datos
|     | x1  | ... | xj  | ... | xp  |
| --- | --- | --- | --- | --- | --- |
| m1  | x11 | ... | x1j | ... | x1p |
| ... | ..  | ..  | ..  | ..  | ..  |
| mn  | xn1 | ..  | xnj | ... | xnp |
Sea $X^*$ la matriz de datos normalizada. La matriz de covarianza viene dada por la formula
$$
\Sigma = \frac{(X^*)^TX^*}{n} \in \mathbb{R}^{p\times p}
$$

## observaciones
1. $\Sigma$ es simétrica.
2. es diagonalizable y todos sus autovalores son reales
3. Los autovectores correspondientes a autovalores distintos son ortogonales
4. Hay una base ortogonal formada de $\mathbb{R}^p$ formada por autovectores de $\Sigma$
	1. Si $U$ es la matriz con columnas los autovectores de $\Sigma$ y $D$ es diagonal con los autovalores de $\Sigma$: $\Sigma=UDU^T$