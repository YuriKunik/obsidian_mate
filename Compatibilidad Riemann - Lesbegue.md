
Sean $a\leq b$, $f:[a,b]\to \mathbb{R}$ una función Riemman-integrable. Entonces $f \in L_{1}([a,b])$ y 
$$
\int_{[a,b]}f = (R) \int_{a}^{b}f.
$$

## Claves:
1. Tomar particiones $\pi_{k}$ tales que $S_{\pi_{k}}(f)-s_{\pi_{k}}(f)< \frac{1}{k}$
2. Definir $g_{k}=\inf_{[x_{j}, x_{j+1}]} f(x)$ y $h_{k}=\sup_{[x_{j}, x_{j+1}]} f(x)$ en cada intervalo $[x_{j-1}, x_{j}]$.
3. $$
\int_{[a,b]}g_{k}=s_{\pi_{k}}(f)
$$ y análogo para $h_{k}$.
4. por ser monótonas y estar acotadas superior o inferiormente tenemos que convergen a $g, h$ respectivamente.
5. Por [[Segundo teorema de convergencia mayorada]]
