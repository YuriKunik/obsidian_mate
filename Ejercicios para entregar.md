Maria Dorda
Yuri Kunik
# Ejercicio 18:

## Enunciado:
Dada una familia de grupos abelianos $\{G_{n}\}_{n\geq 2}$, construir un CW-complejo simplemente conexo $X$ tal que $H_{n}(X)=G_{n}$ $\forall n \geq 2$.

## Demostración

Por el teorema de estructura, sabemos que todo grupo abeliano finitamente generado, $G$, es de la forma

$$
G = \mathbb{Z}^n \bigoplus_{i=1}^t \mathbb{Z}_{q_{i}},
$$
con $q_{i}$ una potencia de algún primo. Si podemos un CW-complejo que tenga como homología cada uno de los sumandos, podemos conseguir un espacio que tenga al grupo $G$ como $H_{n}$ tomando la wedge sum.
Vamos a dividir el problema en 2 casos:
1. CW-complejo con $H_{n}= \mathbb{Z}_{m}$:  
Tomamos $S^n$ como CW-complejo y le adjuntamos una $n+1$-celda $e^{n+1}$ mediante la función de adjunción $\varphi : S^n \to S^n$ con grado $m$. Llamando a este espacio $X_{m}$ el complejo de cadenas celular $C_{*}(X_{m})$ es:
```tikz
\usepackage{amsfonts}
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
	 \dots & \mathbb{Z} & \mathbb{Z} & 0\dots & 0 & \mathbb{Z} & 0
	\arrow["d_{n+2}", from=1-1, to=1-2]
	\arrow["d_{n+1}", from=1-2, to=1-3]
	\arrow["d_{n}", from=1-3, to=1-4]
	\arrow["", from=1-4, to=1-5]
	\arrow["", from=1-5, to=1-6]
	\arrow["", from=1-6, to=1-7]
\end{tikzcd}
\end{document}
```
Por la fórmula para el morfismo de borde, sabemos que :
$$
 d_{n+1}(e^{n+1})= deg(\varphi) e^n = m e^n.
$$
Tomando homología tenemos:
$$
H_n(X_{m}) = \frac{ker(d_{n})}{Im(d_{n+1})} = \frac{\mathbb{Z}}{\mathbb{Z}_m}
$$
$$
	H_{k}(X_{m}) = 0 \forall k\geq 2, k \neq n 
$$
2. CW-comlpejo con $H_{n}=\mathbb{Z}$: 
Tomamos $S^n$ como CW-complejo y sin adjuntar nada más tenemos que:
$$
H_{k}(S^n) = 
\begin{cases}
0 & \text{si } k \neq n \text{ y } k \geq 2  \\  
\mathbb{Z} & k = n
\end{cases}
$$

Ahora, dado un grupo $G$ abeliano finitamente generado y un $k\in \mathbb{N}$,  tenemos
$$
\begin{align}
 G &= \mathbb{Z}^n \bigoplus_{i=1}^t \mathbb{Z}_{q_{i}} \\
 &= H_k(S^k)^n \bigoplus_{i}^t H_{k}(X_{q_{i}}) \\ 
 &= H_{k}(\vee_{i=1}^n S^k \bigvee_{i}^t X_{q_{i}}) \\ \\
 &= H_{k}(X_{G}) 
\end{align}.
$$
Para finalizar, en el caso de tener una cadena de grupos abelianos finitamente generados, $\{ G_{n} \}_{n \geq 2}$, tomamos $X= \vee_{n=2} X_{G_{n}}$.  
																								$\square$

# Ejercicio 19:
## Enunciado:
Sea $n \in \mathbb{Z}$. Probar que existe una única función $\phi$ que le asigna a cada CW-complejo finito un entero tal que
1. $\phi(X)$ = $\phi(Y)$ si $X$ e $Y$ son homeomorfos.
2. $\phi(X)=\phi(A)+\phi(X/A)$ si $A$ es subcomplejo de X.
3. $\phi(S^0)=n$
Probar además que tal función debe cumplir que $\phi(X)=\phi(Y)$ si $X \simeq Y$.

## Demostración

### Existencia
$$
	\phi(X) =n ( \chi (X) - 1)
$$
Es claro que cumple a) y c). Para b), sea $X$ un CW-complejo y $A$ un subcomplejo de $X$. $X/A$ tiene estructura de CW-complejo con $n$-celdas pegadas por $q\circ \varphi_\alpha$ y $(X/A)^{(0)} = X^{(0)}/A^{(0)}$. De esta construcción se ve que la cantidad de n-celdas de $X/A$ es la cantidad de n-celdas de $X$ menos las de $A$ salvo en $n=0$ donde tenemos una extra que corresponde a la clase de equivalencia de $[A]$.  Con esto 
$$
\begin{align}
	\phi(X/A) &= n ( \chi(X/A) - 1) \\
             & = n\left(  \sum_{m} \# \text{m-celdas de X/A} -1 \right)  \\ \\
	 & = n\left( \sum_{m} \#\text{m-celdas de }X - \#\text{m-celdas de }A + 1 - 1 \right)  \\
&= n \left(  \sum_{m} \# \text{m-celdas de }X - 1 \right) - n\left(  \sum_{m} \# \text{m-celdas de } A - 1 \right) \\
& = \phi(X) - \phi(A).
\end{align}
$$

### Unicidad

Sea $\varphi$ una función que cumpla los items del enunciado. Veamos que $\varphi$ tiene que separar los wedges finitos en sumas:
$$
\begin{align}
	\varphi(A\vee B) &= \varphi(A) + \varphi((A \vee B) / A) \\
	 & = \varphi(A) + \varphi(B).
\end{align}
$$
En la última igualdad usamos que $\varphi$ se preserva por homeomorfismos. Vamos a ver que la $\varphi$ coincide con $\phi$ en las esferas (los CW-complejos más simples). Entonces $\varphi(S^0) = n$, para $\varphi(S^1) = \varphi(S^0) + \varphi(S^1 / S^0) = n + \varphi(S^1 \vee S^1) = n + 2\varphi(S^1)$. Con esto podemos concluir que, $\varphi(S^1) = -n$. Inductivamente, usando que $\varphi(S^n/S^{n-1}) = \varphi(S^n \vee S^n)$, obtenemos
$$
\varphi(S^k)=
\begin{cases}
	n & \text{k es par} \\
-n & \text{k es impar}
\end{cases}
$$
![[Drawing 2023-06-03 15.18.13.excalidraw]]

Tomando un CW-complejo arbitrario. Si las $0$-celdas son $\{ x_{i} \}_{i=1}^m$ entonces
$$
\begin{align}
\varphi(\{ x_{i} \}_{i\geq 1}) &= \varphi(S^0) + \varphi(\{ x_{i} \}_{i\geq 1} / S^0)  \\
& = n + \varphi(\{ x_{i} \}_{i\geq 2})  \\
	 & = n + \varphi(S^0) + \varphi(\{ x_{i} \}_{i\geq 2} / S^0) \\
	 & = 2n + \varphi(\{ x_{i} \}_{i\geq 3}) \\
   & = \vdots  \\
   & = (m-1)n.
\end{align}
$$
Si $X^{(l)}=X$, 
$$
\begin{align}
\varphi(X^{(l)}) &= \varphi(X^{(l)} / X^{(l-1)}) + \varphi(X^{(l-1)}) \\
	 & =\varphi(\bigvee_{m\leq \# l-\text{celdas}} S^l ) + \varphi(X^{(l-1)})  \\
& = (-1)^l \# \{ l\text{-celdas} \} n + \varphi(X^{(l-1)} / X^{(l-2)}) + \varphi(X^{(l-2)}) \\
&= (-1)^l \# \{ l\text{-celdas} \} n + (-1)^{l-1} \# \{ l-1\text{-celdas} \}n + \varphi(X^{(l-2)})  \\
& = \sum_{i=1}^l (-1)^i \# \{l\text{-celdas}\}n + \varphi(X^0)  \\
& = \sum_{i=1}^l (-1)^i \# \{l\text{-celdas}\}n +  (\# \{0\text{-celdas}\} - 1 )n \\
& = \phi(X).
\end{align}
$$
Que la $\phi$ sea preservada por equivalencias homotópicas viene de que $\chi$ cumple esto.

# Ejercicio 21:

## Enunciado:
Probar que toda función continua $f : S^n \to S^n$ es homotópica a una que tiene algún punto fijo.

## Demostración:
Supongamos que $f$ no tiene puntos fijos (caso contrario ya estamos). En la teórica vimos que si dos funciones $f,~ g$ no coinciden en ningún punto, entonces $f \approx A \circ g$. Tomando a $g$ como la identidad, al f no tener puntos fijos, $f(x) \neq id(x) ~ \forall x$ entonces $f\approx A \circ id = A$. Basta ver que tenemos una función $g$ con algún punto fijo, homotópica a $A$.  Llamemos a la rotación por un ángulo $\theta$, 
$$
r(\theta) =
\begin{pmatrix}
\cos(\theta) & - \sin(\theta) & 0 & \dots & 0 \\
-\sin (\theta) & \cos(\theta) & 0  & \dots & 0 \\
0 &0&1  && 0 \\
\vdots &&&\ddots&\vdots\\
0 & \dots &\dots&&1
\end{pmatrix}.
$$
 Moviendo el ángulo entre $0$ y $\pi$ obtenemos una homotopía para las funciones $A$ y $r(\pi)\circ A$. Con esto ya estamos dado que $r(\pi)\circ A (1,0 \dots, 0) = r(\pi)(-1,0,\dots, 0)= (1, 0, \dots, 0)$.
																								$\square$