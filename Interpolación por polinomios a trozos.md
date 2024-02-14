
## Interpolación por poligonales

Se toman $n$ puntos equiespaciados y los conectamos con segmentos (polinomios de grado 1).
El error de esto lo podemos medir como
$$
\lVert f-q_{n} \rVert _{\infty} \leq \frac{\lVert f^{\prime \prime }\rVert_{\infty}}{2} \frac{h^2}{4} = \frac{\lVert f^{\prime \prime }\rVert_{\infty}}{8} \frac{(b-a)^2}{n^2}
$$
