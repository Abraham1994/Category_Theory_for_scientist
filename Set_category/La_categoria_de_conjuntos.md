# La Categoría de Conjuntos
<script type="text/javascript" async
  src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML">
</script>

\\(
  \newcommand{\noin}{\in \!\!\!\!\! / }
  \newcommand{\ds}{\displaystyle}
  \newcommand{\R}{\mathbb{R}}
  \newcommand{\Rd}{\R^{d}}
  \newcommand{\Sr}{\mathcal{S}(\mathbb{R}^{d})}
  \newcommand{\Rt}{\R^{3}}
  \newcommand{\vp}{\varphi}
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
## Productos

Sean \\( X, Y \\) conjuntos. Sabemos que
$$ X \times Y = \lbrace (x,y) \: | \: X \in X , \, y \in Y \rbrace $$

Existen dos **proyecciones canónicas**, \\( \pi_{1}: X \times Y \rightarrow X \\) y \\( \pi_{2}: X \times Y \rightarrow Y \\). Gráficamente:

..... imagen

También sabemos cuál es el producto de tres o más conjuntos, por ejemplos \\[ X \times Y \times Z = \lbrace (x,y,z) \; / \; X \in X , \, y \in Y,  \, z \in Z \rbrace \\]

Ahora viene...

### LA PROPIEDAD UNIVERSAL del producto
> Sean \\( X, Y \\) conjuntos. Para todo conjunto \\( A \\) y funciones \\( f: A \rightarrow X \\) y  \\( g : A \rightarrow Y\\) entonces *existe un única función* \\( \langle f,g \rangle: A \rightarrow X \times Y \\), llamada **función inducida** por \\(f \\) y \\(g\\), tal que el siguiente diagrama conmmuta.....  


### Un ejemplo (usando la notación del lema):
Supongamos que \\( |X| = m \\) y \\( |Y| = n  \\). Sabemos que puede representarse como una matriz de dimensiones \\( m \times n \\); además \\( \ds X \stackrel{\pi_{1}}{\leftarrow} X \times Y \stackrel{\pi_{2}}{\rightarrow} Y \\). Gráficamente:

....

Supongamos que \\( A \\) representa a un grupo de personas. Digamos que una persona \\(a \in A \\) escoge un elemento \\( f(a) \in X\\) y otro elemento \\( g(a) \in Y\\); pero al hacerlo está "escogiendo" el elemento \\( (f(a), g(a)) \\), ¡lo cual justamente define a la función \\( \langle f,g \rangle \\)!

#### Productos en ologs
Sean \\(c \\) y \\(d \\) dos tipos, podemos etiquetar el producto \\( c \times d \\) de esta manera: $$  "c \times d " := \mbox{un par } (x,y) \mbox{ donde }  x \mbox{ es } c  \mbox{ y }  y  \mbox{ es } d  $$

Veamos un ejemplo. Consideremos los tipos \\( \ulcorner \\)un dueño de carro\\(\urcorner\\) y \\( \ulcorner \\)un carro\\( \urcorner \\); una persona puede tener varios. La relación que asocia a cada dueño el carro que usa más es una función (un aspecto). Además, un economista puede preguntar cuánto ingresa le genera a cierto dueño el uso de cierto carro (es claro que el ingreso es cero si el carro no le pertenece). Usando la propiedad universal, tenemos el siguiente gráfico.


## Coproductos
Sean \\( X \\) y  \\( Y \\) conjuntos. El **coproducto** de \\( X \\) y \\( Y \\), denotado por \\( X \sqcup Y \\), es la "unión disjunta", es decir, consiste en juntar los elementos de los dos conjuntos, considerando los elementos que se repiten como diferentes en \\( X \sqcup Y \\).

Existen dos **inclusiones canónicas**, \\( i_{1} : X \rightarrow X \sqcup Y \\) y \\(i_{2}: Y \rightarrow X \sqcup Y \\). Gráficamente,

........

*Los elementos de \\( X \sqcup Y \\) no son tan importantes; lo importante son las inclusiones* \\(i_{1}\\) y \\( i_{2}\\), ya que ellas nos permiten saber de donde provienen los elementos de \\( X \sqcup Y\\). *Podemos identificar dos conjuntos isomorfos como iguales*, ese un hecho básico en la teoría de categorías.

### Un ejemplo
El coproducto de \\( X = \lbrace a,b,c,d \rbrace \\) y \\( Y = 1,2,3 \\) es \\[ X \sqcup Y \simeq \lbrace a,b,c,d,1,2,3 \rbrace \\]

El coproducto de \\( X \\) consigo mismo es \\[ X \sqcup X = \lbrace i_{1} a , i_{1} b, i_{1} c, i_{1} d, i_{2}a , i_{2} b , i_{2} c, i_{2} d \rbrace  \\]

### Propiedad universal del coproducto
> Sean \\(X , Y \\) conjuntos. Para todo conjunto \\( A \\) y funciones \\( f : X \rightarrow A \\) y \\( g: Y \rightarrow A \\), existe una única función \\( \displaystyle \left\lbrace {f \atop g } \right. : X \sqcup Y \rightarrow A \\) tal que el siguiente diagrama conmuta

................

### Coproductos en ologs

A diferencia que en los productos, no hay una forma estándar de etiquetar los coproductos usando las etiquetas de sus términos.

Consideremos el siguiente olog, el cual incluye las funciones inducidas.

..............

 \\( "X \sqcup Y" = \\) \\( \ulcorner \\)un asiento en un avión\\( \urcorner \\) significa que todos los asientos en cualquier avión son ecónomicos o de primera clase.

 Gracias a la propiedad universal, llegamos a las siguientes conclusiones *(estamos formalizando nuestra intuición)*:
 1. Si sabemos cuánto cuestan los asientos ecónomicos y cuánto cuestan los de primera clase, y si sabemos que todo asiento (en todo avión) es económico o de primera clase, entonces sabemos cuánto cuesta cualquier asiento (en cualquier avión)

 2. Si sabemos en qué avión está cada asiento económico y en qué avión está cada asiento de primera clase, no necesitamos más información para saber en qué avión está un asiento cualquiera.


## [Límites finitos en **Set**](limites_finitos_en_set.md)
Los límites (categóricos) tienen bellas aplicaciones en Topología, Análisis y otras ramas de la Matemática. Aquí veremos su aplición para formalizar ideas usando ologs.

La razón del nombre "límites" será vista en la sección **Formalizando**.


## [Colímites finitos en **Set**](colimites_finitos_en_set.md) 

"Conceptos dual = col-". Usaremos la noción de relación equivalencia y conjunto conciente.
