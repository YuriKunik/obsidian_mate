#definiciones #topoalg #matemática
## Definición
Un $n$ simplex es el menor conjunto convexo en $\mathbb{R}^m$ conteniendo $n+1$ puntos $v_0, v_1, ..., v_n$ que no están en el mismo hiperplano de dimensión menor que $n$. A cada simplex lo vamos a notar $[v_0, v_1, ..., v_n]$. 
Para la homología es importante el orden de los vertices, por esto tomamos un orden inducido por los sub indices. 

Existe un homeomorfismo lineal desde el n-simplex estándar  a un n-simplex $[v_0, ..., v_n]$ dado por:
$$
(t_0, ..., t_1) \mapsto \sum_i t_i v_i
$$
Los coeficientes son las coordenadas baricéntricas del punto $\sum_i t_i v_i$ en $[v_0,  ..., v_n]$.

## Caras
Una Cara de un simplex $[v_0, ..., v_n]$ es un subsimplice con sus vertices siendo cualquier subconjunto no vacío de vertices del original.