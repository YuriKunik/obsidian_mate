```tikz
\usepackage{tikz-cd}
\begin{document}
\begin{tikzcd}
A & B\\
X & B \cup_f X\\
&& Z
\arrow["f", from=1-1, to=1-2]
\arrow["\bar{f}", from=2-1, to=2-2]
\arrow["i", from=1-1, to=2-1]
\arrow["\bar{i}", from=1-2, to=2-2]
\arrow["g_X",bend right, from=2-1, to=3-3]
\arrow["g_Y",bend left, from=1-2, to=3-3]
\arrow["\exists! g", dotted, from=2-2, to=3-3]
\end{tikzcd}
\end{document}
```
