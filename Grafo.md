
## Definición

Un **grafo** es una $4$-upla $(V,A,s,t)$ con
1. $V$ un conjunto llamado conjunto de vértices
2. $A$ un conjunto llamado conjunto de aristas (o flechas)
3. $s:A\to V$ una función llamada origen (source).
4. $t:A\to V$ una función llamada destino (target).

Un **camino** es una sucesión de flechas $\{ a_{j} \}_{i=0}^{n}$ con $t(a_{j})=s(a_{j+1})$.
## Idea

La idea de esta definición es que las funciones $s$ y $t$ nos sirven para saber de donde a donde va cada una de la flechas del grafo. A modo de ejemplo podemos ver

![[Grafo 2024-03-07 02.08.11.excalidraw]]

En este caso,
$$
\begin{cases}
A = s(f)=s(h) \\
B = s(g)=t(f)  \\
C =t(g)=t(h)
\end{cases}
$$