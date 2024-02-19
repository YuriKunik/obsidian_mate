#calculonumerico #integracion 

## Enunciado

Dada $f\in C[a,b]$ y dado $n \in  \mathbb{N}$ notamos por
$$
I(f)=\int_{a}^{b} f(x)w(x) \, dx \quad \text{ y definimos } Q_{n}(f)=\sum_{j=0}^{n}  A^{n}_{j}f(x_{j}^{(n)})
$$
donde
$$
A_{j}^{(n)} = \int_{a}^{b} l^{n}_{j}(x)w(x) \, dx.
$$
Con esto, si existe una constante $K$ tal que
$$
\sum_{j=0}^{n}  \lvert A^{(n)}_{j} \rvert \leq K \quad \forall n
$$

entonces
$$
\lim_{ n \to \infty } Q_{n}(f)=I(f).
$$

### Demostración
Por el [[Teorema de Weiestrass]], dado $\varepsilon>0$ existe un polinomio $q_{N} \in \mathcal{P}_{N}$ ($N$ dependiendo de $\varepsilon$) tal que
$$
\lVert f-q_{N} \rVert_{\infty}\leq\varepsilon.
$$
Como $Q_{n}$ es exacta para todo polinomio de grado menor o igual que $n$ sabemos que a partir de un momento $Q_{n}(q_{N})=I(q_{N})$. Tenemos que 
$$
\begin{align}
\lvert I(f)-Q_{n}(f) \rvert  & = \lvert I(f)-I(q_{N})+Q_{n}(q_{N})-Q_{n}(f) \rvert  \\
     & \leq \lvert I(f-q_{N}) \rvert + \lvert Q_{n}(q_{N}-f) \rvert .
\end{align}
$$

Anotando por comodidad $c=\int_{a}^{b} w(x) \, dx$, se tiene
$$
\begin{align}
\lvert I(f)-I(q_{N}) \rvert &= \left\lvert  \int_{a}^{b} w(x)(f(x)-q_{N}(x)) \, dx   \right\rvert  \\
&\leq \lVert f-q_{N} \rVert _{\infty} c \\
     & \leq c \varepsilon
\end{align}
$$
En el otro término tenemos
$$
\begin{align}
\lvert Q_{n}(q_{N})-Q_{n}(f) \rvert &= \left\lvert  \sum_{j=0}^n A_{j}^{(n)}(q_{N}(x_{j}^{(n)})-f(x_{j}^{(n)}))  \right\rvert  \\
 &\leq \lVert f-q_{n} \rVert _{\infty} \sum_{j=0}^n A_{j}(n) \\
 &  \leq K\varepsilon 
\end{align}
$$

Con esto dado $\varepsilon > 0$  existe $N$ tal que si $n>N$
$$
\lvert I(f)-Q_{n}(f) \rvert \leq (c+K){\varepsilon}
$$
$\square$