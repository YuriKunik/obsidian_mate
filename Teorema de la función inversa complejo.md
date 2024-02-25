#complejo #diferenciación 
## Enunciado

Sean $f:U\to \mathbb{C}$ una [[Función holomorfa]] con $U$ abierto, $f = u + iv$ con $u, v \in C^1$, $z_{0} \in U$ tal que $f^\prime (z_{0})\neq 0$. Entonces existen $\tilde{U}, V$ entornos de $z_{0}, f(z_{0})$ correspondientemente, tales que $f:\tilde{U}\to V$ es biyectiva, $f^{-1}$ es holomorfa y vale
$$
(f^{-1})^\prime (f(z_{0})) = \frac{1}{f^{\prime} (z_{0})}.
$$

## Demostración

Tomamos la identificación de $f$ con $F:U\to \mathbb{R}^2$ y escribamos $z_{0}=x_{0}+iy_{0}$, $f^{\prime} (z_{0})=a+bi$, entonces por las [[Ecuaciones de Cauchy-Riemann]] sabemos que
$$
\det(DF(z_{0}))=a^{2}+b^{2}=\lvert f^{\prime} (z_{0}) \rvert ^{2}\neq 0
$$
Entonces $DF(z_{0})$ es inversible y, por lo tanto, $F$ tiene inversa local ([[Teorema de la función inversa multivariable]]). Además, usando la formula para la inversa en $\mathbb{R}^{2\times 2}$ tenemos que
$$
DF(z_{0})^{-1}= \frac{1}{\lvert z_{0} \rvert ^{2}}\begin{pmatrix}
a & b \\
-b & a
\end{pmatrix}
$$
lo que prueba que $f^{-1}$ también cumple las ecuaciones de C-R ya que $DF(z_{0})^{-1}$ es $DF^{-1}(f(z_{0}))$. Más aún, la forma de esta última matriz prueba que
$$
(f^{-1})^\prime(f(z_{0}))=\frac{a-b_{i} }{\lvert f^{\prime} (z_{0}) \rvert ^{2}}=\frac{\bar{f^{\prime} (z_{0})}}{\lvert f^{\prime} (z_{0}) \rvert ^{2}}=\frac{1}{f^{\prime} (z_{0})} .
$$
