# Límites finitos en *Set*
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
  \newcommand{\xyz}{X \times_{Z} Y }
\\)

## Pullbacks

Consideremos el siguiente diagrama (1)


Su **producto fibra** es el conjunto \\[ X \times_{Z} Y  = \lbrace (x,y,z) \: / \:  f(x) = g(y) = z \rbrace \qquad  \\]

Las **proyecciones canónicas** son \\( \pi_{1}: X \times_{Z} Y \rightarrow X \\) y \\(\pi_{2}: X \times_{Z} Y \rightarrow Y \\).
Haciendo \\( W = \xyz \\), entonces el diagrama (2)

...........

conmuta. Cabe resaltar que el producto fibra depende de las funciones \\( f\\) y  \\( g \\).

En general, asumiendo la configuración del diagrama 1, se define el **pullback de \\(X \\) y \\(Y \\) sobre \\(Z\\)** como cualquier conjunto \\(W \\)  que es isomorfo a \\( \xyz \\). El símbolo \\( \lrcorner \\)  en el diagrama (2) indica que \\( W \\) es el pullback.

Observar que, si \\( W \\) es el pullback, entonces para todo \\(w \in W \\), \\( f (\pi_{1}(w)) = g ( \pi_{2}(w))= z \\) para algún \\(z \in Z\\); *podemos corresponder cada \\( w \\) con algún \\(z \in Im(f) \cap Im(g) \\)*. Cuando \\(f \\) y \\(g\\) son inclusiones inyectivas, *podemos decir que \\( W \simeq Im(f) \cap Im (g) \\)*, lo cual se verifica encontrando un isomorfismo con \\(X \times_{Z} Y \\). Esto será usado a continuación.


## Usando pullbacks para definir nuevas ideas de anteriores  
El diagrama de la derecha es el pullback del de la izquierda (*asumiendo que estamos de acuerdo con el etiquetado*),

...............

¿Qué significado tiene \\( A) B \times_{D} C \\)? Significa que, para nosotros: "Un buen cliente es un cliente rico y leal"


### Propiedad universal de los pullbacks
> Para todo conjunto \\( A \\) y funciones  \\(f: A \rightarrow X \\) y \\( g: A \rightarrow Y\\)  tales que  \\(t \circ g = u \circ g\\), existe una única función \\(\langle f,g \rangle : A \rightarrow \xyz \\) tal que el siguiente diagrama conmuta


### Pegando diagramas usando producto fibrado
> Sea un diagrama.........   
donde \\( B' \simeq B \times_{C} C' \\) es un pullback. Entonces se cumple: \\[  A \times_{B} (B \times_{C} C') \simeq A \times_{C} C'. \\]

Consideremos el diagrama

.....

Por el resultado anterior, el símbolo \\( \lrcorner \\) de la derecha indica que el rectángulo de la derecha y el rectángulo grande son pullbacks.

### Un ejemplo

Veamos como definir un celular con batería con precisión usando el siguiente olog:

.............

Por la propiedad fundamental, se concluye que \\( A \simeq B \times_{F}  E \\). Luego, yendo hacia abajo y luego a la derecha, obtenemos: "un celular con mala batería es un celular que tiene una batería que permanece cargada menos de una hora".



## Ámbitos, experimentos y matrices.

Sean \\( A \\)  y \\(B \\) dos conjuntos, un **ámbito con resultados \\(A\\) y \\(B\\)**  es un conjunto \\( R\\) junto con funciones \\( f: R \rightarrow A\\) y  \\(g: R \rightarrow B\\). Gráficamente,

.............

Podemos pensar en \\(A\\) y \\(B\\) como magnitudes observables y \\(R \\) como un conjunto de experimentos que produce valores para dichas magnitudes.

Sean \\( \displaystyle A \stackrel{f}{\leftarrow} R \stackrel{g}{\rightarrow} B \\) y \\( \displaystyle B \stackrel{f'}{\leftarrow} R' \stackrel{g'}{\rightarrow} C \\) dos ámbitos. El **ámbito compuesto** es el producto fibra \\( R \times_{B} R' \\). Gráficamente:

.........

En este caso, podemos decir que \\( R \times_{B} R' \\) representa un experimento que produce los mismos valores para las magnitudes \\( A\\), \\(B\\) y \\( C\\) que los experimentos \\( R \\) y \\( R' \\) cuando los valores de \\( B \\) coinciden.

### Matriz de un ámbito

Sea \\(  A \leftarrow R \rightarrow B \\) un ámbito. Sea \\( R \stackrel{p}{\rightarrow} A \times B \\) la función única generada por la propiedad universal del producto. Podemos considerar la matriz (*o mejor dicho, la función*) con índices \\( (a,b) \in A \times B \\) cuya entrada correspodiente es \\( \lvert  p^{-1}(a,b) \rvert \\). Esta es la **matriz del ámbito \\(  A \leftarrow R \rightarrow B \\)**.

Ahora daremos dos propiedades.
-  Sean \\(  A \leftarrow R \rightarrow B \\) y \\(  A \leftarrow R' \rightarrow B \\) dos \\( (A,B) \\)-ámbitos. Ambos ámbitos poseen matrices de dimensión \\( |A| \times |B| \\). Por la propiedad univesal del coproducto existe  un único ámbito \\(  A \leftarrow R \sqcup R' \rightarrow B \\ tal que el diagrama .....
conmuta. Luego, *la matriz del ámbito \\(  A \leftarrow R \sqcup R' \rightarrow B \\) es la suma de las matrices de los otros ámbitos*.

- Sean \\(  A \leftarrow R \rightarrow B \\) y \\(  B \leftarrow R' \rightarrow C \\) dos ámbitos. *La matriz del ámbito compuesto es la multiplicación (usual) de las matrices de los otros ámbitos*.


## Equalizadores y objetos terminales

Consideremos los siguientes diagramas:

..........

El **equalizador de \\( f\\)  y \\( g\\)** es el diagrama conmutativo de la derecha, donde \\[ Eq (f,g) := \lbrace x \in X \: / \: f(x) = g(x) \\] y \\( p \\) es la inclusión canónica.

Un **conjunto terminal** es un conjunto \\( S \\) tal que para todo conjunto \\(X \\) existe una única función \\(X \rightarrow S\\).
