# Clase Fourier
15/06/11 Matemática II (biología)
---
# Señales
## Definición

Una señal es una cantidad que varía a lo largo del tiempo.  Matematicamente vamos a tener una función

$f:\mathbb{R}\to \mathbb{R}^n$

$$
f(t) = (x_{1}, \dots, x_{n})
$$

---
## Señales periódicas

Una señal para la cual existe un $T$ con

$$
f(t+T) = f(t)~ ~\forall t \in \mathbb{R}
$$

se le dice periodica.

Al $T$ mínimo que cumple esto lo llamamos periodo de la función $f$.

---
## Ejemplos
- Tamaño de una población a lo largo del tiempo (según el 1er parcial)
<split>
![[Solucionperiodica.png|400]] ![[output.png|400]]
</split>
---
- Osciladores
<split even>
Péndulos, resortes, corriente alterna
</split>
- Olas (waves)
	Sonidos, Olas de verdad, Luz
---
## Señales armónicas simples

$$
f(t) = \hat{x}sen(2\pi /T + \varphi)
$$
con:
- $\hat{x}$ la amplitud máxima
- $T$ el periodo
- $\varphi$ la fase

---
<iframe src="https://editor.p5js.org/YuriK/full/YadA6dwc2"
		width=800
		height=600></iframe>
---
Grafiquemos algunas señales en python.

---

# Curvas Lissajous
<iframe width="560" height="315" src="https://www.youtube.com/embed/SaadsrHBygc?clip=Ugkxgf0ZerW7loz-F6ST-dSp-XQ9aPDbhMoA&amp;clipt=EOneJxiB1Cg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
---
### ¿Cuál es la importancia de las señales armónicas simples?

Si bien su comportamiento queda determinado por unos pocos parámetros, estas son suficientes para "explicar" todas las señales periódicas mediante el análisis de Fourier.

---
## Transformada de fourier

¿Qué vamos a hacer?

---

## Transformada de fourier

¿Qué vamos a hacer?

Una combinación entre PCA y cuadrados mínimos pero aplicado a señales arbitrarias.
---
## Transformada de fourier


¿Qué vamos a hacer?

Una combinación entre PCA y cuadrados mínimos pero aplicado a señales arbitrarias.

- Dada una cantidad suficiente de puntos, vamos a representar nuestra señal como una combinación lineal de señales armónicas simples, donde cada coeficiente nos va a indicar la incidencia de la frecuencia del termino correspondiente.
---

Para esto vamos a utilizar polinomios trigonométricos
$$$
x(t) = a_{0}+ \sum_{k=1}^n(a_{k}\cos(2\pi kt / T)+b_{k}sen(s\pi kt / T))
$$$

---

Definiendo nuevos coeficientes


$$$
c_{k}= 
\begin{cases}
\frac{a_{k}-ib_{k}}{2} si, k>0 \\ \\
\frac{a_{-k}+ib_{-k}}{2} si, k < 0
\end{cases}
$$$
también los podemos escribir como

$$$
x(t) = \sum^n_{k=-n} c_{k} e^{2\pi i k t/ T}
$$$

---
## Coeficientes
Si tenemos una señal que queremos escribir como una serie de polinomios, podemos averiguar los coeficientes como vimos en la teórica

![[coeficientes_matriz.png]]

---
Podemos ganar un poco de intuición para esto si vemos a la matriz de la izquierda como una matriz de cambio de base, con los vectores que forman parte de la base estando como columnas y siendo evaluados en $t_{i}$
---
## Transformada de fourier
La transformada de Fourier va a aparecer ya que nos va a permitir calcular los coeficientes de una forma más directa
---
![[Formula Fourier.png]]

Después de unas cuentitas, llegamos a que si el grado de nuestro polinomio es $n$ y el numero de samples $N$ verifica que $N \geq 2n+1$ entonces $\hat{x}_k = c_k$

---

### Calculemos unos ejemplos

---
## Uso principal

La clave de Fourier es que nos permite pasar de un espacio temporal a otro de frecuencias. Este cambio nos da información que no teníamos a simple vista sobre nuestra señal. El ejemplo más claro de esto lo encontramos al aplicar Fourier a señales de sonido.

---
## Ballena de 52 Hz
La ballena de 52 hertz es el único individuo que canta en esta frecuencia. El resto de las ballenas de la misma zona tienen otras frecuencias, por esto se piensa que la ballena 52 es la ballena más solitaria del mundo. Escuchemos un fragmento de su canto en x10 de velocidad y veamos la frecuencia principal.
[Wikipedia](https://en.wikipedia.org/wiki/52-hertz_whale)

---
### Aplicaciones de Fourier dentro de la biología

Análisis de cantos de ballenas
- [Clicks de cachalotes](https://pubmed.ncbi.nlm.nih.gov/7560502/)
- [Detección de ballenas francas con el espectro](https://www.kaggle.com/c/whale-detection-challenge/data)
- [Más cachalotes](https://drive.google.com/file/d/1f2kKZO5mz-iX_rh-ZVvpwIT6nIUg6U8A/view?usp=sharing)

Este tiene un dataset de un montón de ballenas recopilados para un concurso.

---

  Biología molecular
- [Introducción al tema + ejemplos](https://www.stemside.co.uk/post/the-fourier-transform-and-its-application-in-structural-biology-part-one)

Otros animales
- [Algo sobre perros y +](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC1367946/pdf/biophysj00631-0066.pdf)
