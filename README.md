# Teoría de Categorías
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
## ¿Para qué?
**La teoría de categorías** ha servido mucho a la Matemática "Pura", ya que es una manera de encontrar conexiones entre diversos contextos matemáticos. Nos permite dar cuenta que hay estructuras que se repiten, lo cual es sospechoso (y provechoso)... y hermoso.

Pero eso no es todo. El Álgebra, a grandes rasgos, estudia cómo se comportan los objetos que están sujetos a una estructura. *La teoría de Categorías hace algo parecido, pero con ideas y conceptos*. Gracias a la generalidad de la Matemáticas, estas ideas y conceptos pueden venir de cualquier lugar.
*Los teoremas se cumplirán, como siempre*, y sus implicaciones permiten aumentar nuestro entendimiento, crear nuevas estructuras, generar nuevas preguntas... En otras palabras, pueden ser muy útiles en la Ciencia

En este pequeño trabajo vamos a estudiar los conceptos y teorema básicos sobre esta fascinante teoría; además se darán algunos ejemplos actuales y posibles aplicaciones.

## Definición de categoría
Un **categoría** es una clase \\( \C \\) de objetos junto con  

1. una clase de conjuntos disjuntos, \\( hom(A,B)\\), por cada par de objetos \\( (A,B \in \C) \\); (los elementos de \\(hom (A,B)\\)  son llamados **morfismos** de \\( A \\) en  \\(B \\) y se denotan escribiendo \\( f:A \rightarrow B \\)) ;

2. por cada terna \\( (A,B, C) \\) de objetos de \\(\C\\), una función \\[ hom(B,C) \times hom (A,B) \rightarrow hom (A,C) ; \\] (para morfismos \\(f: A \rightarrow B, \; g:B \rightarrow C \\), esta función se escribe \\( (g,f) \mapsto g \circ f \\) y \\( g \circ f : A \rightarrow C\\) es llamada la **composición** de \\(f\\) y \\(g\\)); todo sujeto a los axiomas:

   + **Asociatividad**. Si \\(f: A \rightarrow B\\), \\(g: B \rightarrow C\\), \\(h: C \rightarrow D\\) son morfismos de \\(\C \\), entonces \\( h \circ (g \circ f) = (h \circ g) \circ f\\).

   + **Identidad**. Para cada objeto \\(B \in C\\) existe un morfismo \\( id_{B}: B \rightarrow B \\) tal que para  todo \\(f: A \rightarrow B\\), \\(g: B \rightarrow C\\): $$ id _{B} \circ f = f \mbox{  y  } g\circ id_{B} = g $$



### Una advertencia acerca del *Lenguaje*
Muchos piensan que la Matemática es perfecta...

Entre los cimientos de la Matemática están la Teoría de Conjuntos y la Lógica. Es increíble e inquitante saber que la investigación sobre dichos cimientos, en lugar de fortalecer, puede hacer tambalear a la Matemática conocida.
Al respecto, podemos citar los famosos [teoremas de incompletitud de Gödel](https://es.wikipedia.org/wiki/Teoremas_de_incompletitud_de_G%C3%B6del) y el debate sobre el [axioma de elección](https://es.wikipedia.org/wiki/Axioma_de_elecci%C3%B3n).

En la definición más amplia de categoría se usa el concepto de clase. Este concepto se desarrolló debido a la aparición de paradojas, como la de Russel:

#### [Paradoja de Russel](https://es.wikipedia.org/wiki/Paradoja_de_Russell)
>Supongamos que conjunto se define como colección de elementos. Sea *M* el conjunto de todos los conjuntos que no son elementos de sí mismos. Luego, ¿M es elemento de sí mismo?

Para evitar esto, se introduce el concepto de **[clase](https://es.wikipedia.org/wiki/Clase_(teoría_de_conjuntos))** el cual es un generelización de conjunto. Digamos que una clase es una colección tal que se puede determinar si un objeto pertenece o no a ella. Es como un "conjunto muy grande". En este caso, un conjunto se define como una clase tal que existe otra clase de la que es un elemento.   
En la práctica estas paradojas no son un obstáculo, por lo menos al principio.


## Conceptos preliminares
En esta sección se presentarán algunos conceptos que se usarán en las definiciones y proposiciones. También se introducen los ***OLOGS***.
- [Conceptos preliminares](Preliminares/Conceptos_preliminares.md)
  + [Ologs](Preliminares/olog.md)



## La Categoría de Conjuntos
En esta sección vamos a ver como los conceptos categóricos se aplican a los conjuntos. Las definiciones y resultados serán casos particulares de cosas más profundas. No seremos taaan formales, porque la intención aquí es sentar ideas y comenzar con las aplicaciones.
- [La Categoría de Conjuntos](Set_category/La_categoria_de_conjuntos.md)
  + [Limites en **Set**](Set_category/limites_finitos_en_set.md)
  + [Colímites en **Set**](Set_category/colimites_finitos_en_set.md)
  + [Otras nociones en **Set**](Set_category/otras_nociones_en_set.md)

## Más aplicaciones
Se definirán varias estructuras algebraicas muy utlizadas en la Ciencia: Monoides, grupos, grados, órdenes y bases de datos. En en el fondo, cada una de ellas es una categoría, vista por dentro y por fuera; aunque no hablaremos mucho de categorías en esta sección...
- [Más aplicaciones](More_aplications/Mas_aplicaciones.md)
  + [Monoides](More_aplications/monoides.md)
  + [Grupos](grupos.md) 1
  + [Grafos](grafos.md) 1
  + [Órdenes](ordenes.md) 1  
  + [Bases de datos: Esquemas e  instancias](bases_de_datos.md) 2

## Formalizando
Como la rigurosa y bella estructura logra englobarlo todo. Algunas consecuencias de este hecho. Muchos resultados parecerían poco prácticos si no se tiene en cuenta las secciones anteriores.
-[Formalizando](Formalizing/Formalizando.md)
  + [Categorías y funtores](Formalizing/categorias_y funtores.md)
  + [Transformaciones naturales](Formalizing/transformaciones_naturales.md)
  + [**Cat** \\( \simeq \\) **Sch**](Formalizing/equiv_cat_y_sch.md)
  + [Límites y colímites](Formalizing/limites_y_colimites.md)
  + [Otras nociones en **Cat**](Formalizing/otras_nociones_en_cat.md)


## Categorias en el trabajo científico
- [Más teoría y resultados](More_theory_and_results/Mas_teoria_y_resultados)
  - [Funtores adjuntos ](More_theory_and_results/funtores_adjuntos.md) 3
  - [Categoría de funtores](More_theory_and_results/categoria_de_funtores.md)
  - [Mónadas](More_theory_and_results/monadas.md) 4
  - [Operadas](More_theory_and_results/operadas.md) 4 (Estas son una generalización de categorías).
- [Categorías en la ciencia](More_theory_and_results/categorias_en_la_ciencia.md)
  + [Ciencia de la Computación](More_theory_and_results/ciencia_de_la_computacion) 5


## Referencias y lectura adicional
- [Category Theory for Scientists](categorias_aplicadas.pdf) Este el libro base, de David I. Spivak, quien creó el concepto de olog. El libro se basa en un curso dictado por el autor en el MIT.
- [OLOGS: A CATEGORICAL FRAMEWORK FOR KNOWLEDGE REPRESENTATION](olog.pdf) Del mismo autor, muy interesante.
- [Category Theory for Computing Science](Barr-Wells-ctcs.pdf) De Michael Barr y Charles Wells.
- [Physics, Topology, Logic and Computation: A Rosetta Stone](aplicaciones.pdf) Más aplicaciones :)
