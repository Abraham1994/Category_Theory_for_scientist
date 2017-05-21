# Conceptos Preliminares

<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"> </script>

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


## Relaciones de equivalencia

Durante esta sección, \\( X \\) representa un conjunto cualquiera. Una **relación en \\( X \\)** es un subconjunto \\( R \subset X \times X \\). Se suele denotar \\( (a,b) \in R \\) por \\( a \sim b \\)

Las funciones son un tipo especial de relaciones ;)

Una **relación de equivalencia** es una relación \\( R \subset X \times X \\) que satisface las siguientes propiedades:
- **Reflexividad:** \\( (x,x) \in R \\) para todo \\( x \in X \\).
- **Simetría:** \\( (x,y) \in R \\) si y solo si \\( (y, x) \in R \\).
- **Transitividad:** Si \\( (x,y) \in R \\) y \\( (y,z) \in  R\\) entonces \\( (x,z) \in R \\)

La **clase de equivalencia de \\(x \in X \\)** es el conjunto \\[ \overline{x} = \lbrace y \in X \: / \: y \sim x \rbrace \\]

El **conjunto cociente de la relación \\( R \\) (o de \\( \sim \\))** es el conjunto de las clases de equivalencia.

### Generando clases de equivalencia (lema)
> Sea \\( X \\) un conjunto y \\( R \subset X \times X \\) una relación. Existe una relación \\( S \subset X \times X \\) tal que
- \\(S \\) es una relación de equivalencia.
- \\(R \subset S\\)
- para toda relación de equivalencia \\(S'\\) tal que \\( R \subset S' \\) se tiene que \\( S \subset S' \\).

La relación \\(S'\\) es llamada **la relación de equivalencia generada por \\(R\\)**. Para construirla, podemos seguir el siguiente proceso heurístico (válido cuando \\(X\\) es finito), en este orden:
1. Añadir a \\(R \\) los elementos que demanda la reflexividad.
2. Añadir al resultado los elementos que demanda la simetría.
3. Añadir al resultado los elementos  que demanda la transitividad.

## Isomorfismos
Sean los conjuntos \\( X \\) y \\(Y \\). Una función \\(f :X \rightarrow Y\\) es un **isomorfismo** si existe una función \\( g : \rightarrow X \\) tal que \\( g \circ f = id_{X} \\) y \\( f \circ g = id_{Y}\\). En tal caso, \\(g \\) es llamada la **inversa** de \\( f\\) y se denota por \\(f^{-1} \\).
 Si existe un isomorfismo entre dos conjuntos, estos son llamados **isomorfos**; se usa el símbolo \\( \simeq \\) .

Los siguientes son hechos triviales acerca de los isomorfismos:
1. Todo conjunto es isomorfo a sí mismo.
2. Si \\( A \simeq B \\) entonces \\(B \simeq A\\).
3. Si \\( A \simeq B \\) y \\( B \simeq C \\) entonces \\( A \simeq C \\)
4. Una función es un isomorfismo si y solo si es biyectiva.


## Cardinalidad
Se dice que dos conjuntos tienen el mismo **cardinal** si existe una función biyectiva entre ellos (es decir, si son isomorfos).

Para todo \\(  n\in \N_{0}\\) vamos a considerar \\( \underline{n} = \lbrace 0, 1, \ldots , n \rbrace \\).
Sea \\(A \\) un conjunto. Decimos que \\( A \\) tiene **cardinalidad** \\(n\\) si tiene el mismo cardinal que \\( \underline{n} \\), lo cual se denota por \\(  |A| =n \\). En este caso, decimos que \\( A\\) es finito. Un conjunto es **infinito** cuando no es finito.

Dos conjuntos finitos tienen la misma cardinalidad si y solo si existe un isomorfismo entre ellos.

## "Diagramas" conmutativos
Consideremos la siguiente figura
$$ \xymatrix { a \ar [r] & b \ar [d] \\
               c \ar [u] & d \ar [l]
} $$

Se dice que este es un **diagrama de conjuntos** si \\( A,B, C \\) son conjuntos y \\( f,g,h \\) son funciones. Decimos que es un **triángulo conmutativo de conjuntos** si \\( g \circ f = h\\).

Ahora consideremos la siguiente figura
$$ \xymatrix { a \ar [r] & b \ar [d] \\
               c \ar [u] & d \ar [l]
} $$

Se dice que este es un *diagrama de conjuntos* si \\( A,B, C,D \\) son conjuntos y \\( f,g,h \\) son funciones. Decimos que es un **cuadrado conmutativo de conjuntos** si \\( g \circ f = i \circ h\\).

.... Más dibujos....


## [Ologs](olog.md)
Los científicos tienen una constante necesidad de organizar sus experimentos, datos, resultados y conclusiones en algún *esquema* de tal forma que su trabajo sea reutilizable, transferible y comparable con el trabajo de otros científicos. Puede que los **ologs** sean la solución a esta necesidad :)

Olog es la abreviatura de "ontological log"(apunte ontológico). Fueron introducidos en 2010 por David Spivak , profesor investigador del MIT. En mi opinión, los ologs tienen un futuro prometedor. Algunas ventajas de usar ologs son:

- permiten una formulación precisa de un punto de vista.
- pueden convertirse a esquemas de datos
- pueden expandirse a medida que aumenta la información
- pueden ser referenciados fácil y precisamente
- los ologs pueden compararse usando funtores, lo cual genera una "traducción" automática de las distintas terminologías.
