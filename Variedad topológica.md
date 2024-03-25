
## Definición

### Definición del Lee
Un [[espacio topológico]] $M$ es una **variedad topológica** de dimensión $n$ si:

1. $M$ es un [[Espacio de Hausdorff]].
2. $M$ tiene una [[base topológica]] contable.
3. $M$ es localmente euclídeo de dimensión $n$. Es decir, para todo $p \in M$, podemos encontrar un entorno $U$ de $p$ una función $\phi :U\to \mathbb{R}^{n}$ y un entorno $V$ de $\phi(p)$ de forma tal que $\phi :U\to V$ es un [[homeomorfismo]].

### Definición de Larry
Un espacio topológico Hausdorff $M$ y un cubrimiento por abiertos $\{ U_{i} \}_{i \in I}$ con $\varphi :U_{i}\to \varphi_{i}(U_{i})\subset \mathbb{R}^{n}$ homeomorfismo con la imagen tal que, para $U_{j}\cap U_{i}\neq \emptyset$
$$
\varphi _{j} \circ \varphi _{i} ^{-1}|_{\varphi _{i} (U_{i} \cap U_{j} )}:\varphi_{i}(U_{i} \cap U_{j} )\to \varphi_{j}(U_{i} \cap U_{j} )
$$
sea homeomorfo.

![[Variedad topológica 2024-03-20 20.32.18.excalidraw]]

## En criollo

La definición de Larry explicita el hecho de que los mapas tienen que ser compatibles. En el caso continuo nos queda inmediatamente ya que pedimos que sean homeomorfismos con la imagen.