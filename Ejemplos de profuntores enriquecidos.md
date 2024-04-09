
## $\text{Bool}-$profuntores y puentes entre ciudades

Teniendo $\mathcal{V}=\text{Bool}$, un $\text{Bool}-$[[Profuntor enriquecido|profuntor]] $\phi :X\twoheadrightarrow Y$, con $X$ e $Y$ [[Preorden|preordenes]]. Sabemos que los preordenes se pueden representar como [[Diagrama de Hasse]]. Vamos a pensar a los preordenes como ciudades con cada elemento siendo un punto de interés. Así, una flecha de un punto a otro representa que hay una forma de llegar de $a$ a $b$. Un profuntor, en este caso, es una función
$$
\phi :\mathcal{X}^{op} \times \mathcal{Y}\to Bool.
$$
monotona (una [[Relación de factibilidad]]). Esto se traduce a tener, dados $(x,y),$ una flecha si $\phi(x,y)= \text{True}$. En términos de nuestro ejemplo de la ciudad, a poder ir de $x$ a $y$ por más que estén en ciudades distintas.

![[Ejemplos de profuntores enriquecidos 2024-03-17 22.53.51.excalidraw]]
La cuestión de que $\phi$ salga de $X^{op}$ se ve en que, con $S\to E$, $b\to a$, entonces $\phi(E,b) \leq \phi(S,a)$, lo cual es cierto ya que ambos son $\text{True}$. Poniendo un recuadro más grande obtenemos un nuevo preorden que viene del nuevo diagrama de Hasse obtenido. A este lo llamaremos [[collage de preordenes]].

En forma matricial, expresamos 

| $\phi$ | a    | b     | c    | d     | e    |
| ------ | ---- | ----- | ---- | ----- | ---- |
| N      | true | false | true | false | true |
| E      | true | true  | true | true  | true |
| W      | true | false | true | false | true |
| S      | true | true  | true | true  | true |

a esto se le llama la matriz de factibilidad de $\phi$.

## **Costo**-profuntores y puentes.

Haciendo algo parecido al diagrama anterior, volvemos a usar diagramas para representar a las **Costo**-categorías pero está vez vamos a necesitar grafos pesados. En este caso, las flechas van a indicar la distancia entre distintos puntos.

![[Ejemplos de profuntores enriquecidos 2024-03-17 23.14.55.excalidraw]]

En este caso [[Funtor Enriquecido|funtores enriquecidos]] entre preordenes son más que funciones monótonas. Tenemos $\phi :X^{op}\times Y\to \text{Costo}$. Que sea un funtor enriquecido nos dice que;
$$
\begin{align}
	(X^{op}\times Y)((x,y),(w,z))  & = X(w, x) + Y(y,z)  \\
	 & \leq \text{Cost}(\phi(x,y), \phi(w,z))  \\
	 & = \phi(x,y) \multimap \phi(w,z)  \\
	 & = max(0, \phi(w,z)-\phi(x,y))
\end{align}
$$

Esta conclusión no se ve muy alentadora pero tratemos de inducir el significado del profuntor desde un hecho que sabemos, un $Costo$-funtor $F:X\to Y$ es una función que no incrementa distancias. ¿Qué es la distancia en $X^{op}\times Y$? es la suma de las distancias entre los pares correspondientes de puntos. Sabiendo que las distancias son los caminos más cortos.