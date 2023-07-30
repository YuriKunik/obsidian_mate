
## Definiciones

### Permutación de filas (resp. Columnas)
Para $\sigma \in \mathbb{S}_{n}$, $\alpha_{\sigma}$ definida por 

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\bar{r} \times \bar{r} & \bar{r} \times \bar{r} & A \\
\arrow["\sigma \times id", from=1-1, to=1-2]
\arrow["\alpha", from=1-2, to=1-3]
\end{tikzcd}
\end{document}
```
para filas.

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\bar{r} \times \bar{r} & \bar{r} \times \bar{r} & A \\
\arrow["id \times \sigma", from=1-1, to=1-2]
\arrow["\alpha", from=1-2, to=1-3]
\end{tikzcd}
\end{document}
```
para columnas.

#### Observaciones

1. Si notamos $p_{ij} = (I_{r})_{ij}=$ Matriz obtenida de $I_{r}$ transponiendo las filas i y j. Entonces el signo de la permutación es $-1$ por lo que el [[Determinante en anillos|determinante]] es $\det(p_{ij}) = -1$ con lo cual $p_{ij}\in (A^{r\times r})^{*}$.

2. $\alpha_{\sigma}$ se obtiene multiplicando a $\alpha$ por una sucesión finita de $p_{ij}$, ya que $\sigma$ es producto de transposiciones.

### Permutar por una unidad

Sea una [[Grupo de unidades|unidad]] $\lambda\in A^{*}$ hacemos

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
\bar{r} \times \bar{r} & A & A \\
\arrow["\alpha", from=1-1, to=1-2]
\arrow["\lambda .", from=1-2, to=1-3]
\end{tikzcd}
\end{document}
```
o equivale a multiplicar por izquierda a $\text{diag}(1,\dots,1,\lambda,1,\dots,1) \in (A^{r\times r})^{*}$

### Sumar a una fila otra por un elemento de $A$

Corresponde a multiplicar a la izquierda por

$$
t^{ij}(u)=I_{r}+ue^{ij} \quad (i\neq j)
$$

