
## Deducción

Dada $f:U\to \mathbb{C}$ una función, podemos escribir a $f$ según su parte real y su parte imaginaria:
$$
f(x+yi)=u(x,y)+iv(x,y)
$$
con $u,v:U\to \mathbb{R}$ con $U \subset \mathbb{R}^{2}$ una identificación del $U\subset \mathbb{C}$ del dominio de $f$. Siguiendo está identificación, podemos definir 
$$
F(x,y)=(u(x,y),v(x,y))
$$
Ahora, cuál es la relación entre estas formas:

## Enunciado

Teniendo definidas, $f$ y $F$. Vale que $f$ es derivable en $z_{0}=x_{0}+iy_{0}$ sii $F$ es diferenciable en $(x_{0},y_{0})$ y además $DF(x_{0},y_{0})$ es [[C linealidad|C lineal]].

### Demostración

#### $1\implies 2$
Escribamos explicitamente cada número complejo como vector en la condición de derivabilidad. Tenemos $z_{0}=x_{0}+iy_{0}$, $f^{\prime }(z_{0})=a+bi$ y $h=h_{1}+ih_{2}$. Con esto sabemos que se cumple la igualdad
$$
\begin{align}
f(z_{0}+h)-f(z_{0})&=(a+bi)(h_{1}+h_{2}i)+R(z_{0}+h) \\
     & = ah_{1}-bh_{2} + (ah_{2} + bh_{1})i + R(z)
\end{align}
$$

Reemplazando, obtenemos
$$
F(x_{0}+h_{1}, y_{0}+h_{2})- f(x_{0},y_{0}) = \begin{pmatrix}
a & -b \\
b & a
\end{pmatrix}
\begin{pmatrix}
h_{1} \\
h_{2}
\end{pmatrix}
+R(x_{0}+h_{1}, y_{0}+h_{2}).
$$

Donde $R$ verifica que
$$
\frac{\lVert \tilde{R}(x_{0}+h_{1},y_{0}+h_{2}) \rVert}{\lVert (h_{1},h_{2}) \rVert } \to 0
$$
Esto Prueba que $F$ es diferenciable, y además $DF_{(x_{0},y_{0})}$ cumple que 
$$

$$
#### $2\implies 1$









