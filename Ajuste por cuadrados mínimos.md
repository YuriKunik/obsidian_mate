# Definición
Dado un espacio de funciones $f(x;\alpha_{1}, \dots, \alpha_{m})$ el ajuste por cuadrados mínimos es la función que minimiza el [[Error cuadrático medio]] de la tabla de valores:

| $x$ | $x_{1}$ | $x_{2}$ | $\dots$ | $x_{N}$ |
| --- | ------- | ------- | ------- | ------- |
| y   | $y_{1}$ | $y_{2}$ | $\dots$ | $y_{N}$        |

i.e. se busca minimizar
$$
S(\alpha_{1}, \dots, \alpha_{m}) = \frac{1}{2}\sum^N_{j=1}(y_{j}-f(x_{j};\alpha_{1}, \dots, \alpha_{m}))^2
$$

# Modelo lineal

Buscamos minimizar la función $S(\alpha_{1}, \dots, \alpha_{m})$ para funciones de la forma $f(x)=\alpha + \beta x$. Derivando y haciendo cuentas llegamos a que, para que ambas derivadas se anulen, necesitamos una solución del siguiente sistema:
$$
\begin{cases}
\sum_{j=1}^N y_{j}= \alpha N + \beta \sum_{j=1}^N x_{j}. \\
\sum_{j=1}^N y_{j}x_{j} = \alpha \sum_{j=1}^N x_{j} + \beta \sum_{j=1}^N x_{j}^2.
\end{cases}
$$
De forma matricial tenemos

$$
\begin{pmatrix}
n+1 & \sum^n_{i=0}x_{i} \\
\sum_{i=0} n x_{i} & \sum_{i=0}^n x_{i}^2  
\end{pmatrix}
\begin{pmatrix}
\alpha \\
\beta  
\end{pmatrix}
=
\begin{pmatrix}
\sum^n_{i=0} y_{i} \\
\sum^n_{i=0} y_{i}x_{i} 
\end{pmatrix}
$$
