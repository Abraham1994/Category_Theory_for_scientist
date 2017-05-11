## Teoría de Categorías 


### ¿Para qué?
**La teoría de categorías** ha servido mucho a la Matemática "Pura", ya que es una manera de encontrar conexiones entre diversos contextos matemáticos. Nos permite dar cuenta que hay estructuras que se repiten, lo cual es sospechoso (y provechoso)... y hermoso.

Pero eso no es todo. El Álgebra, a grandes rasgos, estudia cómo se comportan los objetos que están sujetos a una estructura. *La teoría de Categorías hace algo parecido, pero con ideas y conceptos*. Gracias a la generalidad de la Matemáticas, estas ideas y conceptos pueden venir de cualquier lugar. 
*Los teoremas se cumplirán, como siempre*, y sus implicaciones permiten aumentar nuestro entendimiento, crear nuevas estructuras, generar nuevas preguntas... En otras palabras, pueden ser muy útiles en la Ciencia

En este pequeño trabajo vamos a estudiar los conceptos y teorema básicos sobre esta fascinante teoría; además se darán algunos ejemplos actuales y posibles aplicaciones. 


### Una advertencia acerca del *Lenguaje*
Muchos piensan que la Matemática es perfecta...
Entre los cimientos de la Matemática están la Teoría de Conjuntos y la Lógica. Es increíble e inquitante saber que estos cimientos, en lugar de fortalecer, pueden hacer tambalear la Matemática conocida. 
Al respecto, podemos citar los famosos teoremas de incompletitud de Gödel y el debate sobre el axioma de elección. 

En la definición más amplia de categoría se usa el concepto de clase. Sin entrar en detalles, este concepto se desarrolló debido a la aparición de paradojas, como la de Russel: 

#### Paradoja de Russel
Digamos que un conjunto es una colección de elementos. Sea *M* el conjunto de todos los conjuntos que no son elementos de sí mismos. Luego, ¿M es elemento de sí mismo?

En este pequeño trabajo usaremos **categorías pequeñas**, las cuales se basan en conjuntos "normales", es decir, clases que son conjuntos. De esta manera podemos avanzar sin tener que preocuparnos de contradicciones. 


### Definición de categoría 
Una **categoría** es una clase *Ç* de objetos junto con 
1. Una clase de conjuntos disjuntos, *hom*; además por cada par de objetos *A,B* en *Ç* hay un solo conjunto, *Hom(A,B)*. Un elemento de *Hom(A,B)* es llamado **morfismo de *A* a *B*** es denotado por *f:A→B*. 
2. Por cada terna *(A,B,C)* de objetos en *Ç*, una función *hom(B,C)×hom(A,B)→hom(A,C)*; para morfismos *f:A→B*, 









You can use the [editor on GitHub](https://github.com/Abraham1994/Category_Theory_for_scientist/edit/master/README.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/Abraham1994/Category_Theory_for_scientist/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://help.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
