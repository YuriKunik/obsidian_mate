## Definición
Dado un conjunto $A$. El [[grupo]] simétrico de A, denotado $S_{A}$ es el grupo $\text{Aut}_{\text{Ens}}(A)$. El grupo de permutaciones de $\{ 1, \dots, n \}$ es notado $S_{n}$.

## Ejemplos

### $S_{2}$
El grupo $S_{2}$ consiste de dos permutaciones:
$$
\begin{cases}
1 \mapsto 1 \\
2 \mapsto 2
\end{cases}
\quad
\text{   y   }
\quad
\begin{cases}
1 \mapsto 2 \\
2 \mapsto 1
\end{cases}
$$
Llamandolas $e$ y $f$ respectivamente nos dan las siguientes ecuaciones:
$$
ee=ff=e, \quad ef = fe = f.
$$
De forma matricial las podemos notar
$$
e=
\begin{pmatrix}
1 & 2  \\
1 & 2 \\
\end{pmatrix}
,\quad
f=
\begin{pmatrix}
1 & 2  \\
2 & 1 \\
\end{pmatrix}
$$
### $S_{3}$
El [[grupo]] $S_{3}$ está formado por

$$
\left \{
\begin{pmatrix}
1 & 2 & 3 \\
1 & 2 & 3 \\
\end{pmatrix}
,
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 3 \\
\end{pmatrix}
,
\begin{pmatrix}
1 & 2 & 3 \\
3 & 2 & 1 \\
\end{pmatrix}
,
\begin{pmatrix}
1 & 2 & 3 \\
1 & 3 & 2 \\
\end{pmatrix}
,
\begin{pmatrix}
1 & 2 & 3 \\
3 & 1 & 2 \\
\end{pmatrix}
,
\begin{pmatrix}
1 & 2 & 3 \\
2 & 3 & 1 \\
\end{pmatrix}
\right \}
$$

multiplicando dos de estas de la forma
$$
1 
\begin{pmatrix}
1 & 2 & 3 \\
3 & 1 & 2 \\
\end{pmatrix}

\begin{pmatrix}
1 & 2 & 3 \\
2 & 3 & 1 \\
\end{pmatrix}
= 
3
\begin{pmatrix}
1 & 2 & 3 \\
2 & 3 & 1 \\
\end{pmatrix}
=1
$$
podemos ver que nos queda:

$$ 
\begin{pmatrix}
1 & 2 & 3 \\
3 & 1 & 2 \\
\end{pmatrix}

\begin{pmatrix}
1 & 2 & 3 \\
2 & 3 & 1 \\
\end{pmatrix}
= 
\begin{pmatrix}
1 & 2 & 3 \\
1 & 2 & 3 \\
\end{pmatrix}
$$
Este grupo ya deja de ser conmutativo y ningún grupo simétrico vuelve a serlo para $n\geq 3$. Lo que si se dan son otras relaciones interesantes. En este caso
$$
x = 
\begin{pmatrix}
1 & 2 & 3 \\
2 & 1 & 3
\end{pmatrix}
\quad
\text{cumple}
\quad
x^2 = e
$$
y
$$
y = 
\begin{pmatrix}
1 & 2 & 3 \\
3 & 1 & 2
\end{pmatrix}
\quad
\text{cumple}
\quad
y^3 = e
$$
(x es de [[orden en grupos|orden]] 2 e y es de orden 3).

Por último, vale que $yx=xy^2$. Con estas relaciones todo producto se puede reducir a un producto de la forma $x^iy^j$ con $0\leq i\leq 1,~ 0\leq j\leq 2$.
Como esto nos da 6 elementos distintos y el grupo tiene justamente $3!$, vemos que está generado por $x, y$ con las relaciones $x^2=e, y^3=e, yx=xy^2$.