## Setup

Si $x(t)$ es solución de la ecuación
$$
\begin{cases}
x^{\prime }(t)= f(t,x(t)) \\
x(t_{0})=x_{0}
\end{cases}
$$
en $[t_{0},T]$, el estudio del error global nos va a permitir estimar que tan bueno es un método para predecir el valor $x(T)$.

## Teorema

Dados $n \in \mathbb{N}$ y $h=\frac{T-t_{0}}{n}$ y un método
$$
x_{i+1}=x_{i}+h\phi(t_{i},x_{i},h)
$$
de forma tal que $\phi$ sea una [[Función Lipschitz]] en la segunda variable:
$$
\exists K / \lvert \phi(t,x, h)- \phi (t, y, h) \rvert \leq K \lvert x-y \rvert 
$$
Entonces para todo $x,y \in \mathbb{R}$ y $t \in [t_{0},T]$ se tiene que
$$
\lvert x(T)-x_{n} \rvert \leq \frac{\tau_{máx}}{K}(e^{K(T-t_{0})}-1)
$$
### Demostración

Sea $e_{i}=x(t_{i})-x_{i}$ el error que se comete en el $i$-ésimo paso del método. Tenemos que
$$
x(t_{i}+h)=x(t_{i})+h\phi(t_{i},x(t_{i}),h)+h\tau
$$
y
$$
x_{i+1}=x_{i}+h\phi(t_{i},x_{i},h).
$$
Restando ambos obtenemos una expresión para $e$
$$
e_{i+1}=x_{i}-x(t_{i})-h(\phi(t_{i},x_{i},h)-\phi(t,x(t_{i}),h))+h\tau_{i}.
$$
Tomando norma obtenemos
$$
\begin{align}
\lvert e_{i+1} \rvert  & \leq \lvert e_{i} \rvert  + h\lvert \phi(t_{i},x _{i}, h)- \phi(t,x(t_{i}),h)\rvert + h\tau_{i} \\
     & \leq \lvert e_{i} \rvert + Kh\lvert x_{i}-x(t_{i}) \rvert + \tau h \\
     & \leq \lvert e_{i} \rvert + Kh \lvert e_{i} \rvert + h \tau_{máx} \\
     & = \lvert e_{i} \rvert (1+Kh)+h \tau_{máx} \\
     & =  \lvert e_{i} \rvert A+ h\tau_{máx}.
\end{align}
$$

Esto nos da una forma recursiva para el error
$$
\begin{align}
\lvert e_{0}\rvert &=0 \\
\lvert e_{1}\rvert &\leq h\tau_{max} \\
\lvert e_{2}\rvert &\leq h\tau_{max}A+h\tau_{max}  \\
                   & = (A+1)h\tau_{max}  \\ \\
\lvert e_{3}\rvert & \leq (A^{2}+A+1)h\tau_{max}  \\ \\
                   & \vdots \\
\lvert e_{n}\rvert & \leq \sum_{j=0}^{n}  A^{j} h \tau_{max}
\end{align}
$$
Ahora, usando la fórmula de suma de potencias, nos queda
$$
\begin{align}
\lvert e_{n} \rvert  & \leq \frac{A^n-1}{A-1}h\tau_{max} \\
     &  = \frac{(1+Kh)^{n}-1}{K}\tau_{max} \\
     & \leq \frac{e^{Knh}-1}{k}\tau_{max}  \\
     & = \frac{e^{K(T-t_{0})}-1}{k}\tau_{max} 
\end{align}
$$
Donde la última desigualdad es
$$
(1+\alpha)^n \leq e^{\alpha n}
$$
con $\alpha>0$.