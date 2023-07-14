Dada una tabla de datos:

| $x$ | $x_{1}$ | $x_{2}$ | $\dots$ | $x_{N}$ |
| --- | ------- | ------- | ------- | ------- |
| y   | $y_{1}$ | $y_{2}$ | $\dots$ | $y_{N}$ |

Si $z_{i} = h(y_{i})$, $t_{i}=g(x_{i})$ y $w_{i}=(\frac{1}{h^\prime(y_{i})})$, buscamos $\alpha$ y $\beta$ que minimicen:

$$

S_{G}(\alpha, \beta)= \sum_{i=0}^n w_{i}(z_{i}-(\alpha + \beta ti))

$$
dadas las matrices:

$$
W = 
\begin{pmatrix}
w_{0} & 0 & \dots & 0 \\
0  & w_{1} &  &  \\
\vdots &  &  \ddots &   &  \\
0  &  &  & w_{n}
\end{pmatrix},
A=
\begin{pmatrix}
1 & t_{0}\\
1 & t_{1}\\
\vdots & \vdots \\
1 & t_{n}
\end{pmatrix},
z= 
\begin{pmatrix}
z_{0} \\
z_{1} \\
\vdots \\
z_{n}
\end{pmatrix}
$$

las ecuaciones normales son, 
$$
A^T W A 
\begin{pmatrix}
\alpha \\
\beta
\end{pmatrix}
= A^T W_{z}
$$
