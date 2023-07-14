
## Enunciado

### 1.
Sea $M$ un $A$-[[Módulo]], $M^{\prime}\subset M$ [[Sub-módulo]] $f:M\to N$ [[Morfismo de módulos]], tal que $f(M^{\prime})=\{0\}$ entonces $\exists!\bar{f}:M / M^{\prime} \to N$ morfismo tal que 

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
M & N\\
M/M^{\prime}
\arrow["f", from=1-1, to=1-2]
\arrow["\pi",swap, from=1-1, to=2-1]
\arrow["\exists \bar{f}",swap, from=2-1, to=1-2]
\end{tikzcd}
\end{document}
```

### 2.
Sea $f:M\to N$ morfismo de $A$-módulos. $M^{\prime}\subset M, N^{\prime}\subset N$ sub-módulos tal que $f(M^{\prime})\subset N^{\prime}$.
Entonces $\exists!\bar{f}:M / M^{\prime} \to N / N^{\prime}$ morfismo de $A$-Módulos tal que conmuta

```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
M & N\\
M/M^{\prime} & N/N^{\prime}
\arrow["f", from=1-1, to=1-2]
\arrow["\pi_1",swap, from=1-1, to=2-1]
\arrow["\pi_2",swap, from=1-2, to=2-2]
\arrow["\exists \bar{f}",swap, from=2-1, to=2-2]
\end{tikzcd}
\end{document}
```

### 3.
Sea $f:M\to N$ morfismo de $A$-Módulos. Entonces $\bar{f}:M / \text{ker}(f)\to N$ establece un isomorfismo de $A$-módulos.

### 4.
Sea $M$ un $A$-módulos, $M_{1}\subset M_{2}\subset M_{3}$ sub-módulos. Entonces
$$
\frac{M / M_{1}}{M_{2} / M_{1}} \equiv M / M_{2}
$$
### 5.
Sea $M$ un $A$-módulos, $M_{1}\subset M,M_{2}\subset M$ existe un isomorfismo
$$
\frac{M_{1}}{M_{1}\cap M_{2}} \to \frac{M_{1}+M_{2}}{M_{2}}
$$

## Observaciones

En  [[#1.]] y [[#2.]] la demostración es chequear que $\bar{f}$ está bien definida. Para [[#1]] la definimos como $\bar{f}([a])=f(a)$ y para [[#2.]] $\bar{f}([a])=[f(a)]$. La condición que imponemos sobre la función nos va a determinar que estos estén bien definidos y sean morfismos de $A$-módulos.

El enunciado [[#3.]] es directo de definiciones. Para [[#4.]] y [[#5.]] Hay que trabajar más.