# Monoides

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

Sea \\( X \\) un conjunto. Una **lista** en \\( X\\) es un par \\( (n,f)\\) donde \\( n\in \N\\) (llamado la **longitud de la lista**) y \\( f: \underline{n} \rightarrow X \\) es una función. La lista \\( (n,f) \\) se denota por \\[ [ f(1) , \ldots, f(n)]. \\]
Se define la **lista vacía** como la *única* lista tal que \\( n=0 \\) y se denota por \\( [] \\). Dado \\(x  \in X \\), la **lista singleton en \\( x \\)** es la lista \\( [x] \\). Sea \\(L = (n,f) \\) una lista y \\( j \leq n\\), la **j-ésima entrada de \\(L\\)** es el elemento \\( f(j) \in \\). El conjunto de listas en \\( X \\) se denota por \\( List (X) \\)

Sean \\(L = (n,f) \\) y \\(L' = (n',f') \\) dos listas, se define la **concatenación de \\(L\\) y \\(L' \\)**, denotada por \\( L++L'\\), como la lista \\( (n+n',f++f')\\) , donde \\( f++f':\overline{n+n'} \rightarrow X \\) está dada por \\[ (f++f')(i) = \left \lbrace  { {f(i) \mbox{   si } i \leq n } \atop f'(i-n) \mbox{   i \geq n+1}  } \right. \\]

Como ejemplo podemos citar *la concatenación de cadenas (en Python, C y otros lenguajes de programación)*. Observar que en una lista (como ha sido definido) no puede variar de tamaño. Las listas ayudan a visualizar el concepto de suma formal.


### Monoides libre generado

Sea \\(X \\) un conjunto. El **monoide libre generado por \\( X \\)** es la terna \\( M:= ( List (X), [], ++)\\). Decimos que \\( X \\) es el **generador** del monoide \\( M \\).

Como ejemplo, \\( \Z\\) es el monoide generado por 1. Con esta notación, un número entero \\(n\\) se representa por \\([1,\ldots 1 ]\\).

## Monoide presentado
Sean \\(G \\) un conjunto finito y \\( n \in \N \\), para cada \\(1 \leq  i \leq n \\) escojamos \\(m_{i}, m_{i}' \in List(G)\\). El **monoide presentado por generadores en \\( G\\) y relaciones \\( \lbrace (m_{i}, m_{i}') \; / \; 1 \leq i \leq n  \rbrace \\)** es el monoide \\( \M = (M,e, \star)\\) definido de la siguiente manera: Sea \\( \sim \\) la relación de equivalencia generada por \\( \lbrace (xm_{i}y \sim xm_{i}' y ) \; / \, x,y \in List(G), \; 1 \leq i \leq n \rbrace \\); definimos \\(M = List (G) / \sim \\); \\(e := [] \\) y \\( \overline{f}  \star \overline {f'} = \overline{f++f'}  \\).

Habría que demostrar que la operación \\( \star \\) está bien definida, es decir, que el resultado de operar dos clases es el mismo sin importar las listas elegidas como representantes de las clases. Se deja esto como ejercicio (*cosa rutinaria para en Matemática*).

Cabe observar que todo monoide libre es presentado; bastaría tomar el conjunto de relaciones como vacío.

### Ejemplo

Supongamos que \\( G = \lbrace a,b,c,d \rbrace\\) son botones que al ser presionados en ciertos órdenes producen ciertos resultados. Luego, cada elementos de \\( List(G) \\) es una manera en la que se puede presionar los botones. Vamos a dar a \\(  G \\) la forma de monoide presentado. Supogamos que presionar \\([a,a,c]\\) siempre produce el mismo resultado que \\( [d,d] \\), *en cualquier ocasión*. Similarmente, supongamos que presionar \\([c,a,c,a] \\) es lo mismo que hacer nada.

Para este caso, consideramos \\(m_{1}= [a,a,c], \; m_{1}'= [d,d], \; m_{2}= [c,a,c,a] \\) y \\( m_{2}'=[] \\). Ahora hagamos un cálculo en \\( M= List(G) / \sima  \):

\\(  [b,c,d,d,a,c,a,a,c,d] = [ b,c,b,a,a,c,a,c,a,a,c,d ] = [ b,c,b,a,a,a,c,d ] = [ b,c,b,a,d,d,d ] \\)

Consíderese\\( K:= \{ BS , a b, \ldots , z \}  \\) Puede contruirse una estructura de monoide presentado, tal que \\(BS \\) puede verse como ``BackSpace`` (borrar letras).

## Monoides cíclicos

Un monoide es llamdado **cíclico** si tiene una presentación que involucra un solo generador.

Ya hemos visto que \\( \Z \\) es un monoide cíclico, generado por \\( 1\\).

### Ejemplo
Consideremos como ejemplo el monoide generado por \\( Q \\) y la relación \\( Q^7 =Q^4 \\). Este monoide podría representarse de la siguiente manera:



## [Acciones de un monoide sobre un conjunto](accionmonod.md)
Sea \\((M,e, \star) \\) un monoide y sea \\( S \\) un conjunto. Una **acción** (de \\((M,e, \star) \\) en \\(S \\)), es una función \\(\cdot : M \times S \rightarrow S \\) tal que, para todos \\( m,n  \in M \\) y \\(s \in S\\):
- \\( e \cdot s = s\\)
- \\( m \cdot (n \cdot s) = (m \star n) \cdot s \\).

Técnicamente, la definición anterior es la **acción izquierda** de \\( (M,e \star ) \\) en \\( S \\). También puede considerarse la noción de **acción izquierda** (solo debe considerarse la condición \\( m \cdot (n \cdot s) = (n \star m) \cdot s \\)) . Cuando el monoide es conmutativo.

### Ejemplo
- Sea \\( S= \{0,1,2, \ldots 11 \} \\). Consideremos la acción \\( \cdot \N _{0} \times S \rightarrow S  \\) tal que $n \cdot s $ es el residuo de dividir 12 entre \\(n+s\\). Esto define una acción.

- Sea
