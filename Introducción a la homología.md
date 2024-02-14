
## Definiciones

Empecemos con un [[Complejo simplicial]] $X$ y trabajemos en el cuerpo $\mathbb{F}_{2}=\{ 0,1 \}$. Para arrancar le vamos a asignar a cada celda una tecla de luz metafórica.

1. Definimos las $k$-cadenas $C_{k}$ como el espacio vectorial sobre el cuerpo $\mathbb{F}_{2}$ con bases las $k$-celdas de $X$.
2. Consideramos los morfismos de borde: Transformaciones lineales $\partial_{k}:C_{k}\to C_{k-1}$ que manda una base de una $k$-celda a la suma abstracta de bases $(k-1)$-celdas que corresponden a caras.
Esto nos da una [[Cadena de Complejos]]

```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 \dots & C_{n+1} & C_n \dots & \dots C_1 & C_0 & 0
	\arrow["\partial_{n+1}", from=1-1, to=1-2]
	\arrow["\partial_{n}", from=1-2, to=1-3]
	\arrow["\partial_{0}", from=1-4, to=1-5]
	\arrow["", from=1-5, to=1-6]
\end{tikzcd}
\end{document}
```


## Ejemplos

Consideremos los casos bases:

## n-simplices

### n=1
En el caso en el que $n=1$ tenemos:

![[1-simplex.excalidraw]]

Donde el $C_{0}$ tiene dimensión 2 y $C_{1}$ dimensión 1. 

El morfismo de borde va a ser una transformación lineal de $C_{1}$ a $C_{2}$ que va a mandar $e_{1} \mapsto e_{1}+e_{2}$.

### n=2

Veamos que pasa cuando tenemos un 2-simplex

![[2-simplex.excalidraw]]

El $C_{2}$ va a tener dimensión 1, $C_{1}$ dimensión $3$ y $C_{0}$ también.

Los morfismos de borde son

$$
\partial:C_{2}\to C_{1}
$$
$$
e_{1} \mapsto e_{1} + e_{2} + e_{3}
$$

$$
\partial:C_{1}\to C_{0}
$$
$$
e_{1} \mapsto e_{1} + e_{2}
$$
$$
e_{2} \mapsto e_{2} + e_{3}
$$
$$
e_{3} \mapsto e_{1} + e_{3}
$$

El segundo como matriz es de la forma

$$
\begin{pmatrix}
1 & 1 & 0 \\
0 & 1 & 1 \\
1 & 0 & 1 
\end{pmatrix}
$$

## Lema 1

### Enunciado

La composición de dos bordes es la transformación lineal nula:

$$
\partial² = \partial_{k-1} \circ \partial_{k} = 0
$$

### Demostración

Sea $V={v_{j}}$ el conjunto de vertices. El mapa de caras $D_{i}$ actúa en un simplex removiendo el $i$-esimo vertice $v_{i}$ de la lista de simplices de estar presente. En el caso contrario no hace nada. Con esto un morfismo de borde es una suma de mapas de cara $\partial = \oplus_{i}D_{i}$. Alcanza verlo para cada $\sigma$ complejo de la base. 
$$
\partial²\sigma = \sum_{i\neq j}D_{j}D_{i}\sigma
$$
Cada $(k-2)$-cara es un $k$-simplice $\sigma$ es representado exactamente dos veces en la imagen de $D_{j}D_{i}$ sobre los $i\neq j$. Por esto los $\mathbb{F_{2}}$ nos dan que la suma es 0.
