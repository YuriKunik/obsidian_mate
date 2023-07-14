#matemática #definiciones #álgebra 
## Definición
### Concreta
Sea $G$ un conjunto no vacío, dotado de una operación binaria
$$
	\cdot: G \times G \rightarrow G
$$
que cumplen:
1. Existe un elemento $e \in G$ tal que $g \cdot e = e\cdot g = g$
2. La operación es asociativa
3. Todo elemento tiene inverso

### Categórica

La [[Categoría]] $\text{Grp}$ tiene:
- Objetos $(G,\cdot)$ con $G\in \text{Ens}$, $\cdot : G \times G \to G$ cumpliendo los puntos de la definición anterior (Se puede expresar categóricamente pero lo dejo para después).
- Morfismos $\varphi: G \to H$ tal que, como función de conjuntos, conmuta
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
G \times G & H \times H \\
G & H\\
\arrow["\varphi \times \varphi", from=1-1, to=1-2]
\arrow["m_G", from=1-1, to=2-1]
\arrow["m_H", from=1-2, to=2-2]
\arrow["\varphi", swap, from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```
#### Observación
No es necesario especificar donde va a parar la identidad ya que esto se deduce del diagrama previo.

