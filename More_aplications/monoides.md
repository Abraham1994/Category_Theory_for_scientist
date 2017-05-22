# Más aplicaciones

<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"> </script>

\\(
  \newcommand{\noin}{\in \!\!\!\!\! / }
  \newcommand{\ds}{\displaystyle}
  \newcommand{\R}{\mathbb{R}}
  \newcommand{\Rd}{\R^{d}}
  \newcommand{\Sr}{\mathcal{S}(\mathbb{R}^{d})}
  \newcommand{\Rt}{\R^{3}}
  \newcommand{\vp}{\varphi}
  \newcommand{\M}{\mathcal{M}}
  \newcommand{\F}{\mathcal{F}}
  \newcommand{\Q}{\mathbb{Q}}
  \newcommand{\C}{\mathscr{C}}
  \newcommand{\D}{\mathscr{D}}
  \newcommand{\V}{\mathbf{V}}
  \newcommand{\pro}{\mathbf{P}}
  \newcommand{\A}{\mathscr{A}}
  \newcommand{\B}{\mathscr{B}}
  \newcommand{\Po}{\mathcal{P}(\Omega)}
  \newcommand{\N}{\mathbb{N}}
  \newcommand{\Rn}{\mathbb{\R}^{n}}
  \newcommand{\Rna}{(\R^{n})^{*}}
\\)

## Monoides libres

### Listas

Sea \\( X \\) un conjunto. Una **lista** en \\( X\\) es un par \\( (n,f)\\) donde \\( n\in \N\\) (llamado la **longitud de la lista**) y \\( f: \underline{n} \rightarrow X \\) es una función. La lista \\( (n,f) \\) se denota por \\[ [ f(1) , \ldots, f(n)] \\]
La **lista vacía** es la *única* lista tal que \\( n=0 \\) y se denota por \\( [] \\). Dado \\(x  \in X \\), la **lista singleton en \\( x \\)** es la lista \\( [x] \\). Sea \\(L = (n,f) \\) una lista y \\( j \leq n\\), la **j-ésima entrada de \\(L\\)** es el elemento \\( f(j) \in \\). El conjunto de listas en \\( X \\) se denota por \\( List (X) \\)

Sean \\(L = (n,f) \\) y \\(L' = (n',f') \\) dos listas, se define la **concatenación de \\(L\\) y \\(L' \\)**, denotada por \\( L++L'\\), como la lista \\( (n+n',f++f')\\) , donde \\( f++f':\overline{n+n'} \rightarrow X \\) está dada por \\[f(x)= \left\lbrace \begin{array}{rcl}
x^2+1 & \mbox{si} & x\geq 0\\
\ln|x| & \mbox{si} & x< 0\\
\end{array}
\right. \\]

Como ejemplo podemos citar *la concatenación de cadenas (en Python, C y otros lenguajes de programación)*.


### Monoides libre generado

Sea \\(X \\) un conjunto. El **monoide libre generado por \\( X \\)** es la secuencia \\( M:= ( List (X), [], ++). Decimos que \\( X \\) es el **generador** del monoide \\( M \\).



## Monoide presentado
Sean \\(G \\) un conjunto finito y \\( n \in \N \\), para cada \\(1 \leq  i \leq n \\) escojamos \\(m_{i}, m_{i}' \in List(G)\\). El **monoide presentado por el generador \\( G\\) y relaciones \\( \lbrace (m_{i}, m_{i}') \; / \; 1 \leq i \leq n  \rbrace \\)** es el monoide \\( \M = (M,e, \star)\\) definido de la siguiente manera: Sea \\( \sim \\) la relación de equivalencia generada por \\( \lbrace (xm_{i}y \sim xm_{i}' y ) \; / \, x,y \in List(G), \; 1 \leq i \leq n \rbrace \\); definimos \\(M = List (G) / \sim \\); \\(e := [] \\) y \\( \overline{f}  \star \overline {f'} = \overline{f++f'}  \\).

Habría que demostrar que la operación \\( \star \\) está bien definida, es decir, que el resultado de operar dos clases sea el mismo sin importar las listas elegidas como representantes de las clases. Se deja esto como ejercicio (*cosa rutinaria para un matemático*).

Cabe observar que todo monoide libre es presentado; bastaría tomar el conjunto de relaciones como vacío.
