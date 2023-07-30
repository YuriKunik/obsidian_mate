
## Enunciados

Sea $M$ un $A$-[[Módulo Noetheriano]], entonces

1. Todo submódulo $S \subset M$ es Noetheriano
2. $\forall f:M\to N$ epimorfa $\implies$ $N$ es Noetheriano.
3. $A$ Noetheriano, $I \subset A$ un [[Ideal]] $\implies$ $A / I$ es Noetheriano
4. Sea $f:M\to N$ un morfismo de $A$-módulos, $M$ es Noetheriano $\iff$ $\text{ker}(f)$ e $\text{im}(f)$ son Noetherianos.
5. Dada una [[Sucesión exacta corta]]
```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
0 & M_1 & M_2 & M_3 & 0 \\
\arrow["", from=1-1, to=1-2]
\arrow["", from=1-2, to=1-3]
\arrow["", from=1-3, to=1-4]
\arrow["", from=1-4, to=1-5]
\end{tikzcd}
\end{document}
```
$M_{2}$ es Noeth $\iff$ $M_{1}$ y $M_{3}$ lo son.

Esto vale idénticamente para [[Módulo artiniano|módulos artinianos]]

## Demostraciones

1. Directa ya que toda cadena de [[Sub-módulo|submódulos]] de $S$ es una cadena de submódulos de $M$.
2. Dada una cadena de submódulos de $N$, $C$, entonces $f^{-1}(C)$ es una cadena en $M$  que se estaciona, por lo tanto existe $n$ tal que $f^{-1}(N_{n}) = f^{-1}(N_{n+1})$. Aplicando $f$ a ambos lados tenemos que $N_{n}= N_{n+1}$ ya que $f$ es epi.
3. Directo ya que $\pi$ es epi.
4. La ida vale por 1. y 2. Para la vuelta tomemos una cadena $C$ en $M$ y veamos que se estaciona. Sabemos que se estacionan $C\cap \text{ker}(f)$ y $f(C)$, con lo cual, existe $n \in \mathbb{N}$ tal que $N_{m}\cap \text{ker}(f) = N_{m+1}\cap \text{ker}(f)$ y $f(N_{m})=f(N_{m+1})$, $\forall m \geq n$. Dado $x \in S_{n+1}$ $f(x)\in f(S_{n+1})=f(S_{n})$, entonces $\exists x' \in S_{n}$ tal que $f(x)=f(x')$. Restando la ecuación previa tenemos que $x-x' \in S_{n+1}\cap \text{ker}(f)=S_{n}\cap \text{ker}(f)$, por lo tanto $x-x'\in S_{n}$, lo que implica, restando $x'$ que $x$ también está en $S_{n}$ por lo que $S_{n}=S_{n+1}$ .
5. Directo de lo anterior.



