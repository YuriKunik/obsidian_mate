# Objetivo

Encontrar un polinomio que interpole a la función en distintos puntos y también en las derivadas de algunos de esos puntos
# Teorema

Dada una función $f$, puntos $x_{0},\dots,x_{k}$ y $m_{0},\dots, m_{k} \in \mathbb{N}_{0}$ tales que $\sum m_{k}=n+1$, existe un único polinomio $p \in \mathcal{P}_{n}$ que satisface

$$
\begin{cases}
p(x_{0})=f(x_{0}), \quad p^\prime(x_{0})=f^\prime (x_{0}) ,\quad \dots p^{(m_{0}-1)}(x_{0})=f^{(m_{0}-1)}(x_{0}) \\
p(x_{1})=f(x_{1}), \quad p^\prime(x_{1})=f^\prime (x_{1}), \quad \dots p^{(m_{1}-1)}(x_{1})=f^{(m_{1}-1)}(x_{1}) \\
\vdots \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \vdots \quad\quad\quad\quad\quad\quad\quad\quad\quad\quad \quad \vdots  \\
p(x_{k})=f(x_{k}), \quad p^\prime(x_{k})=f^\prime (x_{k}) ,\quad \dots p^{(m_{k}-1)}(x_{k})=f^{(m_{k}-1)}(x_{k}) \\
\end{cases}
$$

# Construcción

La construcción va a ser similar a el método de newton pero, al pedir condiciones sobre la derivada vamos a repetir puntos en las diferencias divididas. Para esto vamos a definir
$$
f[x,x]= f^\prime (x).
$$
En el caso en el que tengamos varias condiciones sobre un mismo punto agregamos a la diferencia divida el mismo.



