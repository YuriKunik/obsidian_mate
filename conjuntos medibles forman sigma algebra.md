#análisisreal 
## Enunciado

La familia de [[Conjunto Medible|conjuntos medibles]] forman una [[sigma algebra]]. 

## Demostración

### $\emptyset$ es medible.

Directo al tener medida nula
### Unión numerable de medibles es medible

Dado un $\varepsilon>0$ tenemos que para cada $A_{j}$ existe un abierto $U_{j}$ donde $|U_{j} - A_{j}|_{e}< \frac{\varepsilon}{2^{j}}$. Así:
$$
|U-A|_{e}\leq |\bigcup_{j}U_{j}-A_{j}|_{e} \leq \sum_{j} |U_{j}-A_{j}| \leq \varepsilon
$$
### Complemento de medible es medible

#### Todo conjunto compacto es medible

De la definición de [[medida exterior de lesbegue]] vemos que podemos obtener un conjunto abierto $U$ con $K\subset U$ tal que $|U|_{e} -|K|_{e} < \varepsilon$. Por [[Escritura de abiertos como cajas]] tenemos que $U-K = \cup B_{j}$ y que $|U-K|=\sum |B_{j}|$. Ahora cada conjunto $E_{N} =  \cup_{j=1}^{N}B_{j}$ es compacto con $d(E_{N}, K)>0$, esto implica que $|E_{N} \cup K|_{e}=|E_{N}|_{e} + |K|_{e}$. Así:
$$|K|_{e} + \varepsilon \geq |U|_{e} \geq |E_{N}\cup K|_{e}= |E_{N}|_{e}+|K|_{e}
$$
con lo que $|E_{N}|_{e} \leq \varepsilon$.
Esto nos permite concluir dado que:
$$
|U-K|_{e} \leq \sum |B_{j}|_{e} = \lim_{ N \to \infty } \sum |B_{j}|_{e} = \lim_{ N \to \infty } |E_{N}| \leq \varepsilon
$$


#### Todo conjunto cerrado es medible

Para esto intersecamos a nuestro conjunto cerrado $F$ con bolas de radio $k$ centradas en el origen y escribimos a $F$ como unión numerable de conjuntos medibles. Así obtenemos que es medible

#### Caso general

Sea $A$ un conjunto medible, tenemos que para cada $k$ podemos encontrar un abierto $U_{k}$ tal que $A \subset U_{k}$ con $|U_{k}-A|< \varepsilon$. Escribamos a $F_{k} = U_{k}^{c}$ y $F = \cup F_{k}$. Sabemos que $F$ es medible y:

$$
|A^{c}-F|_{e} = |F^{c}-A|_{e} \leq |F_{k}^{c} - A|_{e} = |U_{k}-A|_{e} < \frac{1}{k}
$$

Al ser $k$ arbitrario concluimos que $|A^{c}-F|_{e} = 0$ y puesto que $A^{c} = A^{c}-F \cup F$  $A^{c}$ es medible.

## Trucos

![[conjuntos medibles forman sigma algebra 2025-01-28 15.03.49.excalidraw]]
