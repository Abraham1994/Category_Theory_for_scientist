# Colímites finitos en *Set*
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

## Pushout

Consideremos  el siguiente diagrama (1):

........

Su **suma fibrada** denotada por \\( X \sqcup_{W} Y \\), se define como el cociente  de \\( X \sqcup W \sqcup Y \\) entre la relación de equivalencia \\( \sim \\), generada por \\( w \sim f(w)\\) y \\( w \sim g(w)\\) para todo \\( w \in W \\).

Las inclusiones canónicas se denotan por \\( i_{1}: X \rightarrow X \sqcup_{W} Y \\) y \\( i_{2}: Y \rightarrow X \sqcup_{W} Y \\). Por ejemplo, para todo \\(x \in X \\): \\( i_{1}(x) = \overline{x} \\). Cabe resaltar que estas inclusiones *no son inyectivas*. Observamos que si \\( Z = X \sqcup_{W} Y \\) entonces el siguiente diagrama conmuta:

............

En general, suponiendo asumiendo la configuración del diagrama (1), se define el **pushout de \\( X\\) y \\(Y \\) sobre \\( W\\)** como cualquier conjunto \\( Z \\) que es isomorfo a \\( X \sqcup_{W} Y \\). El símbolo \\( \ulcorner\\) indica que \\( Z \\) es el pushout.

### Ejemplo 1

Supongamos que \\( X = [ 0,1 ] \\), \\(Y= [1,2]\\) y \\(W = \lbrace 1 \rbrace \\). Si \\( f =g = ( 1 \mapsto 1 ) \\), entonces el pushout es \\( X \sqcup_{W} Y \simeq [0,2] \\). Este ejemplo será generalizado *cuando formalizemos todas estas ideas*; veremos que la recta puede formarse al unir intervalos como en este ejemplo.

## Ejemplo 2
