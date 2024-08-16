
# Enunciado

Todo [[Morfismo de grupos de Lie]] $F:G\to K$ tiene rango constante.

## Demostración

Para ver esto hay que usar que
$$
\begin{align}
    F(gh)&=F(L_{g}(h)) \\
	 & = F(g)F(h) \\
	 & = L_{F(g)}(F((h))
\end{align}
$$
Con esto, $F\circ L_{g} = L_{F(g)}\circ F$, que diferenciando en $1$ nos da:
$$
\begin{align}
dF_{g}\circ d(L_{g})_{1}  & = d(L_{F(g)})_{1} \circ dF_{1}
\end{align}
$$
Que al ser $L_{g}$ un [[difeomorfismo]], tenemos que el rango de $F$ solo depende del rango en el tangente en $1$.