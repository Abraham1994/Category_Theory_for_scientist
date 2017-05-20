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

En general, suponiendo la configuración del diagrama 1, se define el **pullback de \\(X \\) y \\(Y \\) sobre \\(Z\\)** como cualquier conjunto \\(W \\)  que es isomorfo a \\( \xyz \\). El símbolo \\( \drcorner \\)  en el diagrama (2) indica que \\( W \\) es el pullback.

Observar que, si \\( W \\) es el pullback, entonces para todo \\(w \in W \\), \\( f (\pi_{1}(w)) = g ( \pi_{2}(w))= z \\) para algún \\(z \in Z\\); *podemos que corresponder \\( w \\) con algún \\(z \in Im(f) \cap Im(g) \\)*. Cuando \\(f \\) y \\(g\\) son inclusiones, *podemos decir que \\( W = Im(f) \cap Im (g) \\)*, lo cual se verifica encontrando un isomorfismo con \\(X \times_{Z} Y \\). Esto será usado a continuación.


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

Por el resultado anterior, el símbolo \\( \drcorner \\) de la derecha indica que el rectángulo de la derecha y el rectángulo grande son pullbacks.

### Un ejemplo

Veamo como definir Group actions on algebraic varieties \\( \ulcorner \\)un celular con batería\\( \urcorner\\) con precisión usando el siguiente olog:

.............

Por la propiedad fundamental, se concluye que \\( A \simeq B \times_{F}  E \\). Luego, yendo hacia abajo y luego a la derecha, obtenemos: "un celular con mala batería es un celular que tiene una batería que permanece cargada menos de una hora". 
