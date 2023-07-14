#construcciones #definiciones #álgebra 
## Definición
### Objeto inicial
Dado un conjunto $A$, definimos la [[categoría]] $\text{Grp}^A$ que tiene como objetos tuplas  $(j, G)$, con $G$ un grupo y $j: A\to G$ una función de conjuntos. Como morfismos $(j_{1},G_{1})\to (j_{2},G_{2})$ diagramas conmutativos
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
G_1 & G_2\\
A &
\arrow["\phi", from=1-1, to=1-2]
\arrow["j_1", from=2-1, to=1-1]
\arrow["j_2", swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```

El [[Grupo]] libre $F(A)$ va a ser un objeto inicial en $\text{Grp}^A$.

## Intuición

Categóricamente F va a ser el [[Funtor Adjunto]] del [[Funtor]] olvido $U : \text{Grp} \to \text{Ens}$. Hagamos detalladamente esta construcción. Dado $A \in \text{Ens}$ tomamos las flechas 