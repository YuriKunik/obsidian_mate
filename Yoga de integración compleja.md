#complejo #integracion #análisis 

# Propiedades

## Integración de funciones continuas con primitiva

Sea $f:U\to \mathbb{C}$ una función continua. Si $f$ tiene primitiva en $U$, entonces $\int_{\gamma} f(z)  \, dz = 0$ para toda $\gamma$ [[Camino]] cerrado.

### Demostración

Sea $F$ una [[Función holomorfa]] tal que $F^{\prime }\equiv f$ en $U$. Usando que vale el [[Teorema fundamental del cálculo]] para funciones complejas, obtenemos
$$
\begin{align}
\int_{a}^{b} f(\gamma(t))\gamma^{\prime }(t) \, dt &= \int_{a}^{b} (F \circ \gamma)^{\prime }(t) \, dt \\
	 & = F(\gamma(b))-F(\gamma(a)) \\
	 & = 0.
\end{align}
$$


## Desigualdad integral
Dada $f$ continua sobre la imagen de un camino $\gamma$, vale
$$
\left\lvert  \int _{\gamma}f \, dz   \right\rvert \leq \lVert f \circ \gamma \rVert_{\infty} \text{Long}(\gamma).
$$
Con 
$$
\text{Long}(\gamma)=\sum_{j=0}^{N-1}\int_{t_{j} }^{t_{j+1} } \lvert \gamma^{\prime }(t) \rvert   \, dx.
$$

## Pase del límite a la integral


Dadas $\{ f_{n}  \}$ y $f$ su [[Convergencia Uniforme|límite uniforme]] sobre subconjuntos compactos de $U$, entonces
$$
\int _{\gamma}f_{n} (z) \, dz \to \int _{\gamma}f(z) \, dz. 
$$
para todo camino en $U$.

## Pase de sumatorias en integrales.

Si la serie $\sum_{n}f_{n}$ [[Convergencia Uniforme|converge uniformemente]] sobre subconjuntos compactos de $U$ etnoces
$$
\int _{\gamma} \sum_{n\geq 0}f_{n} (z)dz = \sum_{n\geq 0}\int_{\gamma} f_{n} (z)  \, dz.
$$

## Condición suficiente para tener primitiva

Sea $f:U\to \mathbb{C}$ una función continua, con $U$ abierto. Si, para todo [[Camino]] cerrado $\gamma$ en $U$ vale que $\int_\gamma f(z) \, dz = 0$, entonces existe $F:U\to \mathbb{C}$ una [[Función holomorfa]] tal que $F^{\prime }(z)=f(z)$ en todo $z \in U$.

### Demostración

Para demostrar esto asumimos que $U$ es conexo y, al ser además abierto, arcoconexo. 

Tomando $z_{0} \in U$ definimos
$$
F(z):= \int _{\gamma}f(w) \, dw \quad \text{ con } \gamma \text{ un camino que une } z_{0} \text{ y } z.
$$
Verifiquemos que $F$ está bien definida. Sean $\gamma, \alpha$ caminos que unen $z_{0}$ con $z$, el camino $\gamma-\alpha$ es cerrado, por lo que $\int_{\gamma-\alpha} f(z)\, dz = 0$. Y usando propiedades de [[Integración de funciones complejas]] y [[Camino|caminos]]:
$$
\int _{\gamma}f(z) \, dz = \int _{\alpha}f(z) \, dx  
$$
Observemos, además, que podemos definir esto para cualquier par de puntos por ser $U$ arcoconexo. Abusando de notación, podemos decir que
$$
F(z):=\int_{z_{0}}^{z} f(z) \, dz.
$$
Así queremos ver que $F$ es holomorfa. Dado $h \in \mathbb{C}$, podemos tomarlo tal que $z+h$ esté en $U$. Veamos el cociente incremental
$$
\frac{F(z+h)-F(z)}{h} = \frac{1}{h}\int_{z}^{z+h} f(w) \, dw 
$$
que si el $h$ es todavía más chico, podemos suponer que el segmento que une $z$ con $z+h$ está contenido en $U$. Si lo parametrizamos con $\gamma(t)=z+th$ obtenemos
$$
\int _{\gamma}f(z) \, dw= hf(z) 
$$

entonces

$$
\begin{align}
\left\lvert  \frac{F(z+h)-F(z)}{h} - f(z)  \right\rvert  & = \left\lvert  \frac{F(z+h)-F(z)-hf(z)}{h}  \right\rvert  \\
	 & = \left\lvert  \frac{1}{h} \int_{z}^{z+h} [f(w)-f(z)] \, dw   \right\rvert  \\ 
	 & \leq \text{máx}_{t\in[0,1]} \lvert f(z+th)-f(z) \rvert \to 0
\end{align}
$$
por la continuidad de $f$.

## Condición suficiente para tener primitiva versión poligonales

Sean $U \subset \mathbb{C}$ abierto y $f:U\to \mathbb{C}$ continua. Supongamos que para toda poligonal cerrada simple $\gamma$ en $U$ con lados paralelos a los ejes vale $\int_\gamma f(z) \, dz=0$ entonces $f$ tiene primitiva $F$ definida en $U$.

### Idea

Podemos armar curvas que unen dos puntos solo por estas poligonales como lo ilustra el siguiente dibujo.

![[Yoga de integración compleja 2024-02-28 20.38.58.excalidraw]]

ponele.

$$

$$
