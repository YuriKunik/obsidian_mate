[    
    // Math mode
    {trigger: "jk", replacement: "$$0$", options: "tA"},
    {trigger: "dm", replacement: "$$\n$0\n$$", options: "tAw"},
    {trigger: "beg", replacement: "\\begin{$0}\n$1\n\\end{$0}", options: "mA"},


    // Dashes
    // {trigger: "--", replacement: "–", options: "tA"},
    // {trigger: "–-", replacement: "—", options: "tA"},
    // {trigger: "—-", replacement: "---", options: "tA"},


    // Greek letters
    {trigger: "@a", replacement: "\\alpha", options: "mA"},
    {trigger: "@A", replacement: "\\alpha", options: "mA"},
    {trigger: "@b", replacement: "\\beta", options: "mA"},
    {trigger: "@B", replacement: "\\beta", options: "mA"},
    {trigger: "@c", replacement: "\\chi", options: "mA"},
    {trigger: "@C", replacement: "\\chi", options: "mA"},
    {trigger: "@g", replacement: "\\gamma", options: "mA"},
    {trigger: "@G", replacement: "\\Gamma", options: "mA"},
    {trigger: "@d", replacement: "\\delta", options: "mA"},
    {trigger: "@D", replacement: "\\Delta", options: "mA"},
    {trigger: "@e", replacement: "\\epsilon", options: "mA"},
    {trigger: "@E", replacement: "\\epsilon", options: "mA"},
    {trigger: ":e", replacement: "\\varepsilon", options: "mA"},
    {trigger: ":E", replacement: "\\varepsilon", options: "mA"},
    {trigger: "@z", replacement: "\\zeta", options: "mA"},
    {trigger: "@Z", replacement: "\\zeta", options: "mA"},
    {trigger: "@t", replacement: "\\theta", options: "mA"},
    {trigger: "@T", replacement: "\\Theta", options: "mA"},
    {trigger: "@k", replacement: "\\kappa", options: "mA"},
    {trigger: "@K", replacement: "\\kappa", options: "mA"},
    {trigger: "@l", replacement: "\\lambda", options: "mA"},
    {trigger: "@L", replacement: "\\Lambda", options: "mA"},
    {trigger: "@m", replacement: "\\mu", options: "mA"},
    {trigger: "@M", replacement: "\\mu", options: "mA"},
    {trigger: "@r", replacement: "\\rho", options: "mA"},
    {trigger: "@R", replacement: "\\rho", options: "mA"},
    {trigger: "@s", replacement: "\\sigma", options: "mA"},
    {trigger: "@S", replacement: "\\Sigma", options: "mA"},
    {trigger: "ome", replacement: "\\omega", options: "mA"},
    {trigger: "@o", replacement: "\\omega", options: "mA"},
    {trigger: "@O", replacement: "\\Omega", options: "mA"},
    {trigger: "([^\\\\])(${GREEK}|${SYMBOL})", replacement: "[[0]]\\[[1]]", options: "rmA", description: "Add backslash before greek letters and symbols"},


    // Insert space after greek letters and symbols, etc
    {trigger: "\\\\(${GREEK}|${SYMBOL}|${SHORT_SYMBOL})([A-Za-z])", replacement: "\\[[0]] [[1]]", options: "rmA"},
    
    {trigger: "\\\\(${GREEK}|${SYMBOL}) sr", replacement: "\\[[0]]^{2}", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) cb", replacement: "\\[[0]]^{3}", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) rd", replacement: "\\[[0]]^{$0}$1", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) hat", replacement: "\\hat{\\[[0]]}", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) dot", replacement: "\\dot{\\[[0]]}", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) bar", replacement: "\\bar{\\[[0]]}", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) vec", replacement: "\\vec{\\[[0]]}", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) tilde", replacement: "\\tilde{\\[[0]]}", options: "rmA"},
    {trigger: "\\\\(${GREEK}|${SYMBOL}) und", replacement: "\\underline{\\[[0]]}", options: "rmA"},
    {trigger: "\\\\(${GREEK}),\\.", replacement: "\\boldsymbol{\\[[0]]}", options: "rmA"},
    {trigger: "\\\\(${GREEK})\\.,", replacement: "\\boldsymbol{\\[[0]]}", options: "rmA"},


    // Operations
    {trigger: "te", replacement: "\\text{$0}", options: "m"},
    {trigger: "text", replacement: "\\text{$0}", options: "mA"},
    {trigger: "ker", replacement: "\\text{ker}($0)$1", options: "mA"},
    {trigger: "im", replacement: "\\text{im}($0)$1", options: "mA"},
    {trigger: "bf", replacement: "\\mathbf{$0}", options: "mA"},
    {trigger: "sr", replacement: "^{2}", options: "mA"},
    {trigger: "cb", replacement: "^{3}", options: "mA"},
    {trigger: "_", replacement: "_{$0}$1", options: "mA"},
    {trigger: "^", replacement: "^{$0}$1", options: "mA"},
    {trigger: "sts", replacement: "_\\text{$0}", options: "rmA"},
    {trigger: "sq", replacement: "\\sqrt{ $0 }$1", options: "mA"},
    {trigger: "//", replacement: "\\frac{$0}{$1}$2", options: "mA"},
    {trigger: "func", replacement: "$0:$1\\to $2", options: "mA"},
    {trigger: "ee", replacement: "e^{ $0 }$1", options: "mA"},
    {trigger: "rm", replacement: "\\mathrm{$0}$1", options: "mA"},
    {trigger: "conj", replacement: "^{*}", options: "mA"},
    {trigger: "trace", replacement: "\\mathrm{Tr}", options: "mA"},
    {trigger: "det", replacement: "\\det", options: "mA"},

    {trigger: "([a-zA-Z]),\\.", replacement: "\\mathbf{[[0]]}", options: "rmA"},
    {trigger: "([a-zA-Z])\\.,", replacement: "\\mathbf{[[0]]}", options: "rmA"},
    {trigger: "([A-Za-z])(\\d)", replacement: "[[0]]_{[[1]]}", options: "rmA", description: "Auto letter subscript", priority: -1},
    {trigger: "([A-Za-z])_(\\d\\d)", replacement: "[[0]]_{[[1]]}", options: "rmA"},
    {trigger: "\\hat{([A-Za-z])}(\\d)", replacement: "hat{[[0]]}_{[[1]]}", options: "rmA"},
    {trigger: "\\\\mathbf{([A-Za-z])}(\\d)", replacement: "\\mathbf{[[0]]}_{[[1]]}", options: "rmA"},
    {trigger: "\\\\vec{([A-Za-z])}(\\d)", replacement: "\\vec{[[0]]}_{[[1]]}", options: "rmA"},
    {trigger: "([a-zA-Z])bar", replacement: "\\bar{[[0]]}", options: "rmA"},
    {trigger: "([a-zA-Z])hat", replacement: "\\hat{[[0]]}", options: "rmA"},

    {trigger: "([a-zA-Z])vec", replacement: "\\vec{[[0]]}", options: "rmA"},
    {trigger: "([a-zA-Z])ovec", replacement: "\\overrightarrow{[[0]]}", options: "rmA"},
    {trigger: "([a-zA-Z])tilde", replacement: "\\tilde{[[0]]}", options: "rmA"},
    {trigger: "([a-zA-Z])und", replacement: "\\underline{[[0]]}", options: "rmA"},
    {trigger: "bar", replacement: "\\bar{$0}$1", options: "mA"},
    {trigger: "hat", replacement: "\\hat{$0}$1", options: "mA"},
    {trigger: "vec", replacement: "\\vec{$0}$1", options: "mA"},
    {trigger: "tilde", replacement: "\\tilde{$0}$1", options: "mA"},
    {trigger: "und", replacement: "\\underline{$0}$1", options: "mA"},

    {trigger: "([^\\\\])(arcsin|arccos|arctan|arccot|arccsc|arcsec|sin|cos|tan|cot|csc)", replacement: "[[0]]\\[[1]]", options: "rmA"},
    {trigger: "\\\\(arcsin|arccos|arctan|arccot|arccsc|arcsec|sin|cos|tan|cot|csc)([A-Za-gi-z])", replacement: "\\[[0]] [[1]]", options: "rmA"}, // Insert space after trig funcs. Skips letter "h" to allow sinh, cosh, etc.
    {trigger: "\\\\(arcsinh|arccosh|arctanh|arccoth|arcsch|arcsech|sinh|cosh|tanh|coth|csch)([A-Za-z])", replacement: "\\[[0]] [[1]]", options: "rmA"}, // Insert space after trig funcs
    {trigger: "\\\\(neq|geq|leq|gg|ll|sim)([0-9]+)", replacement: "\\[[0]] [[1]]", options: "rmA"}, // Insert space after inequality symbols



    // Symbols
    {trigger: "ooo", replacement: "\\infty", options: "mA"},
    {trigger: "sm", replacement: "\\sum", options: "mA"},
    {trigger: "prod", replacement: "\\prod", options: "mA"},
    {trigger: "bigo", replacement: "\\bigoplus_{$0}^{$1} $2", options: "mA"},
    {trigger: "lim", replacement: "\\lim_{ ${0:n} \\to ${1:\\infty} } $2", options: "mA"},
    {trigger: "([^\\\\])pm", replacement: "[[0]]\\pm", options: "rm"},
    {trigger: "([^\\\\])mp", replacement: "[[0]]\\mp", options: "rm"},
    {trigger: "+-", replacement: "\\pm", options: "mA"},
    {trigger: "-+", replacement: "\\mp", options: "mA"},
    {trigger: "...", replacement: "\\dots", options: "mA"},
    {trigger: "<->", replacement: "\\leftrightarrow ", options: "mA"},
    {trigger: "->", replacement: "\\to", options: "mA"},
    {trigger: "!>", replacement: "\\mapsto", options: "mA"},
    {trigger: "invs", replacement: "^{-1}", options: "mA"},
    {trigger: "\\\\\\", replacement: "\\setminus", options: "mA"},
    {trigger: "||", replacement: "\\mid", options: "mA"},
    {trigger: "and", replacement: "\\cap", options: "mA"},
    {trigger: "orr", replacement: "\\cup", options: "mA"},
    {trigger: "inn", replacement: "\\in $0", options: "mA"},
    {trigger: "sub", replacement: "\\subset", options: "mA"},
    {trigger: "\\subset eq", replacement: "\\subseteq", options: "mA"},
    {trigger: "\\subset ne", replacement: "\\subsetneq", options: "mA"},
    {trigger: "set", replacement: "\\{ $0 \\}$1", options: "mA"},
    {trigger: "=>", replacement: "\\implies", options: "mA"},
    {trigger: "=<", replacement: "\\impliedby", options: "mA"},
    {trigger: "iff", replacement: "\\iff", options: "mA"},
    {trigger: "e\\xi sts", replacement: "\\exists", options: "mA", priority: 1},
    {trigger: "===", replacement: "\\equiv", options: "mA"},
    {trigger: "fora", replacement: "\\forall", options: "mA"},
    {trigger: "Sq", replacement: "\\square", options: "mA"},
    {trigger: "!=", replacement: "\\neq", options: "mA"},
    {trigger: ">=", replacement: "\\geq", options: "mA"},
    {trigger: "<=", replacement: "\\leq", options: "mA"},
    {trigger: ">>", replacement: "\\gg", options: "mA"},
    {trigger: "<<", replacement: "\\ll", options: "mA"},
    {trigger: "~~", replacement: "\\sim", options: "mA"},
    {trigger: "\\sim ~", replacement: "\\approx", options: "mA"},
    {trigger: "prop", replacement: "\\propto", options: "mA"},
    {trigger: "nabl", replacement: "\\nabla", options: "mA"},
    {trigger: "del", replacement: "\\nabla", options: "mA"},
    {trigger: "xx", replacement: "\\times", options: "mA"},
    {trigger: "**", replacement: "\\cdot", options: "mA"},
    {trigger: "para", replacement: "\\parallel", options: "mA"},


    {trigger: "xnn", replacement: "x_{n}", options: "mA"},
    {trigger: "xii", replacement: "x_{i}", options: "mA"},
    {trigger: "xjj", replacement: "x_{j}", options: "mA"},
    {trigger: "xp1", replacement: "x_{n+1}", options: "mA"},
    {trigger: "ynn", replacement: "y_{n}", options: "mA"},
    {trigger: "yii", replacement: "y_{i}", options: "mA"},
    {trigger: "yjj", replacement: "y_{j}", options: "mA"},


    {trigger: "mcal", replacement: "\\mathcal{$0}$1", options: "mA"},
    {trigger: "mbb", replacement: "\\mathbb{$0}$1", options: "mA"},
    {trigger: "ell", replacement: "\\ell", options: "mA"},
    {trigger: "lll", replacement: "\\ell", options: "mA"},
    {trigger: "LL", replacement: "\\mathcal{L}", options: "mA"},
    {trigger: "HH", replacement: "\\mathcal{H}", options: "mA"},
    {trigger: "CC", replacement: "\\mathbb{C}", options: "mA"},
    {trigger: "RR", replacement: "\\mathbb{R}", options: "mA"},
    {trigger: "ZZ", replacement: "\\mathbb{Z}", options: "mA"},
    {trigger: "NN", replacement: "\\mathbb{N}", options: "mA"},
    {trigger: "II", replacement: "\\mathbb{1}", options: "mA"},
    {trigger: "\\mathbb{1}I", replacement: "\\hat{\\mathbb{1}}", options: "mA"},
    {trigger: "AA", replacement: "\\mathcal{A}", options: "mA"},
    {trigger: "BB", replacement: "\\mathbf{B}", options: "mA"},
    {trigger: "EE", replacement: "\\mathbf{E}", options: "mA"},
    {trigger: "AB", replacement: "\\overrightarrow{AB}", options: "mA"},    
    {trigger: "BC", replacement: "\\overrightarrow{BC}", options: "mA"},
    {trigger: "AC", replacement: "\\overrightarrow{AC}", options: "mA"},
    {trigger: "BD", replacement: "\\overrightarrow{BD}", options: "mA"},
    {trigger: "CD", replacement: "\\overrightarrow{CD}", options: "mA"},



    // Unit vectors
    {trigger: ":i", replacement: "\\mathbf{i}", options: "mA"},
    {trigger: ":j", replacement: "\\mathbf{j}", options: "mA"},
    {trigger: ":k", replacement: "\\mathbf{k}", options: "mA"},
    {trigger: ":x", replacement: "\\hat{\\mathbf{x}}", options: "mA"},
    {trigger: ":y", replacement: "\\hat{\\mathbf{y}}", options: "mA"},
    {trigger: ":z", replacement: "\\hat{\\mathbf{z}}", options: "mA"},



    // Integrals
    {trigger: "oinf", replacement: "\\int_{0}^{\\infty} $0 \\, d${1:x} $2", options: "mA"},
    {trigger: "infi", replacement: "\\int_{-\\infty}^{\\infty} $0 \\, d${1:x} $2", options: "mA"},
    {trigger: "dint", replacement: "\\int_{${0:0}}^{${1:\\infty}} $2 \\, d${3:x} $4", options: "mA"},
    {trigger: "oint", replacement: "\\oint", options: "mA"},
    {trigger: "iiint", replacement: "\\iiint", options: "mA"},
    {trigger: "iint", replacement: "\\iint", options: "mA"},
    {trigger: "int", replacement: "\\int $0 \\, d${1:x} $2", options: "mA"},

    // Environments
    {trigger: "pmat", replacement: "\\begin{pmatrix}\n$0\n\\end{pmatrix}", options: "mA"},
    {trigger: "bmat", replacement: "\\begin{bmatrix}\n$0\n\\end{bmatrix}", options: "mA"},
    {trigger: "Bmat", replacement: "\\begin{Bmatrix}\n$0\n\\end{Bmatrix}", options: "mA"},
    {trigger: "vmat", replacement: "\\begin{vmatrix}\n$0\n\\end{vmatrix}", options: "mA"},
    {trigger: "Vmat", replacement: "\\begin{Vmatrix}\n$0\n\\end{Vmatrix}", options: "mA"},
    {trigger: "case", replacement: "\\begin{cases}\n$0\n\\end{cases}", options: "mA"},
    {trigger: "align", replacement: "\\begin{align}\n$0\n\\end{align}", options: "mA"},
    {trigger: "array", replacement: "\\begin{array}\n$0\n\\end{array}", options: "mA"},
    {trigger: "matrix", replacement: "\\begin{matrix}\n$0\n\\end{matrix}", options: "mA"},



    // Brackets
    {trigger: "avg", replacement: "\\langle $0 \\rangle $1", options: "mA"},
    {trigger: "norm", replacement: "\\lvert $0 \\rvert $1", options: "mA", priority: 1},
    {trigger: "mod", replacement: "|$0|$1", options: "mA"},
    {trigger: "(", replacement: "(${VISUAL})", options: "mA"},
    {trigger: "[", replacement: "[${VISUAL}]", options: "mA"},
    {trigger: "{", replacement: "{${VISUAL}}", options: "mA"},
    {trigger: "(", replacement: "($0)$1", options: "mA"},
    {trigger: "{", replacement: "{$0}$1", options: "mA"},
    {trigger: "[", replacement: "[$0]$1", options: "mA"},
    {trigger: "lr(", replacement: "\\left( $0 \\right) $1", options: "mA"},
    {trigger: "lr|", replacement: "\\left| $0 \\right| $1", options: "mA"},
    {trigger: "lr{", replacement: "\\left\\{ $0 \\right\\} $1", options: "mA"},
    {trigger: "lr[", replacement: "\\left[ $0 \\right] $1", options: "mA"},
    {trigger: "lra", replacement: "\\left< $0 \\right> $1", options: "mA"},
    {trigger: "cad", replacement: "$0,~ $0,~ \\dots ,~$0 $1", options:"mA"},

    {trigger: "\\to>", replacement: "\\twoheadrightarrow", options:"mA"},
    {trigger: "pri", replacement: "\\prime $0", options: "mA"},
    {trigger: "fpr", replacement: "f^{\\prime} $0", options: "mA"},
    {trigger: "nvec", replacement: "\\lVert $0 \\rVert $1", options: "mA"},
    {trigger: "ninft", replacement: "\\lVert $0 \\rVert_\\infty $1", options: "mA"},
    
]