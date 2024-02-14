## Objetivo

Minimizar el error
$$
E_{n}=\frac{f^{(n+1)}(\xi)}{(n+1)!}W_{n+1}(x)
$$
Esto lo vamos a lograr minimizando el valor de $W_{n+1}$ mediante una elección correcta de puntos.


## Definición

Los polinomios de Tchebychev se definen como
$$
T_{k}(x) = \cos(k \cos^{-1} (x))
$$
### Formula recursiva

Primero observemos que $T_{0}(x)=1$ y $T_{1}(x) =x$
Usando la identidad trigonométrica 
$$
\cos(\alpha+\beta)+\cos(\alpha-\beta)=2\cos(\alpha)\cos(\beta)
$$
y tomando $x = \cos(\theta )$ tenemos que
$$
T_{k+1}(x)=\cos((k+1) \theta) = 2\cos(\theta)\cos(k\theta)-\cos((k-1)\theta)
$$

Es decir, volviendo a reemplazar la x
$$
T_{k+1}(x) = 2xT_{k}(x)-T_{k-1}(x)
$$

## Propiedades

Sea $T_{k}$ el polinomio de Tchebychev de grado $k$

1. El coeficiente principal de $T_{k}$ es $2^{k-1}$.
2. Las raíces de $T_{k}$ son de la forma
$$
x_{i}=\cos\left( \frac{(2i+1)\pi}{2k} \right)
$$
3. $\lVert T_{k} \rVert_{\infty} = 1$

#### Demostración
1. Sale de la forma recursiva.
2. Necesitamos que el argumento de $T_{k}(x)=\cos(k\cos^{-1}(x))=0$ y eso pasa sii $k\cos ^{-1}(x) = (2i+1) \frac{\pi}{2}$. Despejando obtenemos la formula deseada y moviendo $i = 0, \dots, k-1$ tenemos todas.
3. por la formula es claro y además alcanza los valores en $y_{i}=\cos\left( \frac{i\pi}{k} \right)$,

## Teorema: Tchebychev minimiza la norma

Entre todos los polinomios mónicos de grado $n+1$,
$$
W_{n+1}(x)=\frac{1}{2^n}T_{n+1}(x)
$$
minimiza la norma $\lVert . \rVert_{\infty}$ en el $[-1,1]$.

### Demostración:

Asumamos que existe un polinomio mónico de grado $n+1$ tal que 
$$
\lVert P \rVert_{\infty} <\lVert W_{n+1} \rVert_{\infty}
$$
Por las propiedades vistas anteriormente sabemos que $\lvert W_{n+1} \rvert$ alcanza su máximo en los $n+2$ puntos $y_{i}=\cos\left( \frac{i\pi}{n+1} \right)$. De esto, si restringimos $W_{n+1}$ a $[y_{i}, y_{i+1}]$, en cada uno de estos intervalos alcanza la norma infinito. Entonces tenemos la relación

$$
\lVert P \rVert_{\infty[y_{i}, y_{i+1}]} < \frac{1}{2^n} = \lVert W_{n+1} \rVert_{\infty[y_{i}, y_{i+1}]}.
$$
Además, $W_{n+1}(y_{i})=-W_{n+1}(y_{i+1})$. Si suponemos que $W_{n+1}(y_{i})>0$, la desigualdad nos dice que
$$
P(y_{i})<W_{n+1}(y_{i})\quad\text{y}\quad P(y_{i+1})>W_{n+1}(y_{i+1}).
$$
De donde tenemos que el polinomio $Q(x)=P(x)-W_{n+1}(x)$ tiene al menos un 0 en el intervalo $(y_{i},y_{i+1})$. Como tenemos $n+2$ valores de $y$ $Q$ tiene al menos $n+1$ ceros. Pero $Q$ es a lo sumo de grado $n$ por ser una resta de dos polinomios mónicos de grado $n+1$ con lo cual es el polinomio nulo y $P = W_{n+1}$.

## Formula del error tomando ceros de Tcheby

Sea $f\in C^{n+1}[-1,1]$. Si $p_{n}$ es el polinomio que interpola a $f$ en las raíces de $T_{n+1}$ entonces,

$$
\lVert f-p_{n} \rVert_{\infty} \leq  \frac{\lVert f^{(n+1)} \rVert_{\infty}}{2^n(n+1)!}
$$
Esto se deduce directamente de la formula del resto y notando que $W_{n+1}= T_{n+1}$.

## Traslación a intervalos generales

Remplazando $t = \frac{2(x-a)}{b-a}-1$ obtenemos polinomios con propiedades análogas al Tcheby clásico.
TODO.
















