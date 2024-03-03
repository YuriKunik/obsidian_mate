#integracion #complejo 
## Enunciado

Sean $f:U\to \mathbb{C}$ una función continua, $\gamma :[a,b]\to \mathbb{C}$ una curva $C^{1}$ a trozos. Entonces si $F$ es una [[Primitivas a lo largo de curvas|primitiva a lo largo]] de $\gamma$ entonces
$$
\int_{\gamma}f(z) \, dz = F(b)-F(a).
$$

## Demostración

Podemos suponer que $\gamma$ es de clase $C^{1}$. Entonces tenemos el cubrimiento por abiertos $\{ J_{t} \}_{t\in[a,b]}$ y los conjuntos correspondientes $\{ V_{t} \}$ junto con $g_{t}$. Entonces por el [[número de Lesbegue]] para el cubrimiento $J$ de $[a,b]$ existe un $\delta$ tal que, si tenemos $[t_{j}, t_{j+1}]$ de largo menor que $\delta$, entonces existe un $J_{t}$ tal que $[t_{j}, t_{j+1}] \subset J_{t}$. Así, tomamos $n$ de forma tal que $\frac{b-a}{n}< \delta$ y $t_{j}=a+\frac{j(b-a)}{n}$. Con esto, cada intervalo $[t_{j},t_{j+1}]$ está contenido en algún $J_{t}$ y le asignamos $V_{t}$ y $g_{t}$. Así, en limpio, nos quedan $\{ [t_{j},t_{j+1}] \}_{j=0}^{n-1}$, ${V_{j}}$ y $g_{j}$ las correspondientes a cada intervalo. Con esto

$$
	\int_{\gamma|[t_{j} , t_{j+1} ]} f(z) \, dz = g_{j}(\gamma (t_{j+1})) - g_{j}(\gamma(t_{j}))
$$
que, en la integral entera, nos da
$$
\int_{\gamma} f(z)\, dz = \sum_{j=0}^{n-1} [F(t_{j+1})-F(t_{j})]=F(b)-F(a).
$$

## Corolario: Dos Primitivas difieren en una constante

### Curva $C^{1}$ a trozos

En éste caso es directo ya que de tener dos primitivas, $F, \tilde{F}$. Tomamos
$$
F(t)-F(a)= \int_{\gamma|[a,t]} f(z) \, dz = \tilde{F}(t)- \tilde{F}(a)
$$
con lo que difieren para todo $t$, en $F(a)-\tilde{F}(a)$.

### Curva continua.

Siendo $F_{1}, F_{2}$ las primitivas a lo largo de $\gamma$, $J_{t}^{k},V_{t}^{k},g_{t}^{k}$ como en la definición, con $k=1,2$. Entonces $F_{1}(t)-F_{2}(t)=g_{t}^{1}(\gamma(t))-g^{2}_{t}(\gamma(t))$ es constante en $J^{1}_{t}\cap J^{2}_{t}$. Como es localmente constante, es constante por ser continua.
