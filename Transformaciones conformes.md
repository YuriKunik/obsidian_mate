
#complejo 

## Idea

La idea es demostrar que las funciones holomorfas preservan ángulos. Para esto tomamos dos curvas regulares $\gamma, \delta: (-\varepsilon,\varepsilon) \to \mathbb{C}$ tales que $\gamma(0)=\delta(0)=z_{0}$. La definición del ángulo en un punto $z_{0}$ del plano, venía dada por un $\theta$ tal que
$$
\cos(\theta)= \frac{\langle \gamma^\prime (0), \delta^\prime (0) \rangle}{\lVert \gamma^\prime (0) \rVert \lVert \delta^\prime (0) \rVert }.
$$


En el caso complejo, observamos que hacer $x_{0}x_{1} + y_{0}y_{1} = \Re( z\bar{w})$ por lo que la ecuación anterior nos queda,
$$
\cos(\theta)=\frac{\Re(\gamma^\prime (0) \overline{\delta^\prime (0)}) }{\lvert \gamma^\prime (0) \rvert \lvert \delta^\prime (0) \rvert }
$$

Escribiendo $\gamma^\prime (0)= \lvert \gamma^\prime (0) \rvert e^{i\alpha}$ y $\delta^\prime (0)=\lvert \delta^\prime(0) \rvert e^{i\beta}$. Haciendo $\frac{\gamma^\prime(0)}{\delta^\prime(0)}$ y despejando obtenemos la igualdad simplificada:
$$
\cos(\theta)=\Re(e^{i(\alpha-\beta)})
$$


## Definición

Una función $f$ se dice conforme en un punto $z_{0}$ si preserva ángulos orientados.

## Holomorfa implica conforme

Sea $f$ una [[Función holomorfa]] en $z_{0}$ entonces, si $f^{\prime}(z_{0})\neq 0$, escribimos $f^{\prime}(z_{0})=re^{i\theta}$. Entonces, teniendo $\gamma$ regular con $\gamma(0)=z_{0}$
$$
(f \circ \gamma)^\prime (0)= re^{i\theta} \gamma^\prime (0).
$$
Teniendo lo mismo para una $\delta$ que cumpla las condiciones anteriores y escribiendo las derivadas de las curvas en $0$ como $\lvert \gamma^\prime (0) \rvert e^{i\alpha}$ y $\lvert \delta^\prime (0) \rvert e^{i\beta}$ nos queda
$$
\begin{align}
\Re(e^i(\alpha+\theta-\beta-\theta))  & = \Re(e^{\alpha-\beta})
\end{align}.
$$
De donde vemos que preserva ángulos. La cuenta funciona ya que estamos aplicando una rotación y un cambio de escala a la derivada de la curva, pero estos dos son lo mismo para cualquier curva que pase por el punto.


## Conforme implica holomorfa

Sean $U \in \mathbb{C}$ un abierto y $f:U\to \mathbb{C}$ conforme en $z_{0}$. Entonces $f$ es derivable en $z_{0}$, con $f^{\prime}(z_{0})\neq 0$.

### Demostración

Como $f$ es conforme, dadas dos curvas regulares $\gamma$, $\delta$ con $\delta(0)=\gamma(0)=z_{0}$, se tiene que
$$
\frac{(f\circ\gamma)^\prime}{(f\circ\delta)^\prime}(0) = c \frac{\gamma^\prime (0)}{\delta^\prime (0)}
$$