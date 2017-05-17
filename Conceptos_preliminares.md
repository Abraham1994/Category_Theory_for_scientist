# Conceptos Preliminares

<script type="text/javascript" async src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.1/MathJax.js?config=TeX-MML-AM_CHTML"> </script>

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

## Ologs
Los científicos tienen una constante necesidad de organizar sus experimentos, datos, resultados y conclusiones en algún *esquema* de tal forma que su trabajo sea reutilizable, transferible y comparable con el trabajo de otros científicos. Puede que los **ologs** sean la solución a esta necesidad :)

Olog es la abreviatura de "ontological log"(apunte ontológico). Fueron introducidos en 2010 por David Spivak , profesor investigador del MIT. En mi opinión, los ologs tienen un futuro prometedor. Algunas ventajas de usar ologs son:

- permiten una formulación precisa de un punto de vista.
- pueden convertirse a esquemas de datos
- pueden expandirse a medida que aumenta la información
- pueden ser referenciados fácil y precisamente
- los ologs pueden compararse usando funtores, lo cual genera una "traducción" automática de las distintas terminologías.

En este trabajo veremos muchos teoremas e ideas aplicándose a ologs; sin embargo, estos no serán estudiados profundamente. En vez de eso, vamos a dar las definiciones y conceptos más necesarios para las aplicaciones. Hay mucho que decir acerca de los ologs, puede encontrarse más información en las referencias. Procedamos a definir algunps térmnos importantes:

### Tipos 
Un **tipo** es un concepto abstracto, es decir, una distinción hecha por el autor. Se representan como cajas que contienen una *frase nominal singular indefinida*. Por ejemplo, las siguientes cajas son tipos: ........................



.....¿Diagramas?
