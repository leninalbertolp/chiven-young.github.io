---
layout: post
image: /images/img-post/que-es-markdown.webp
title: "Qué es Markdown, su sintaxis, sabores y editores"
serp_title: "¿Qué es Markdown? sintaxis, sabores y editores"
description: "Conoce qué es Markdown, como es su sintaxis, que son los sabores y los mejores editores para escribir en este lenguaje"
date: 2019-10-03 06:00:00
tags: [desarrollo-web]
author: leninalbertop
---
Hace año y medio por temas de economía (Venezuela) me toco migrar este blog de [**Wordpress**](https://es.wordpress.org/){: target="_blank" rel="noopener"} a [**Jekyll**](https://jekyllrb.com/){: target="_blank" rel="noopener"}, fue un cambio de 360º en todos los sentidos; sin dudas, porque con ello toco también adaptarse a la nueva forma de escribir los post, pase de usar el editor *WYSIWYG* de Wordpress para escribir el texto plano que todos conocemos, a utilizar mi editor de código para **escribir en Markdown**.

Mi primer contacto con Markdown fue gracias a Github allí las documentaciones se escriben en este lenguaje de marcado.

En un principio, mis repositorios en Github eran solo cosas pequeñas y sencillas como un *template HTML* reutilizable, *snippets* y uno más que otro *hack* de CSS nada que me obligara a escribir una extensa documentación.

No fue si no hasta finales de 2016 cuando cree un plugin para el editor de código [**Visual Studio Code**](/mi-setup-vscode#materializecss-snippets){: target="_blank" rel="noopener"} donde me sumergí un poco más en Markdown y a partir de la nueva fase de este blog toco redactar los post en este enriquecido lenguaje de marcado.

Por tal motivo quise hacer esta especie de guía para tenerla como referencia para futuras consultas y puede que tal vez te sirva a ti también. Espero te guste.

## ¿Qué es Markdown?

Markdown es un lenguaje de marcado ligero para darle estilos a los textos planos. El lenguaje fue creado por **Jhon Gruber** en **2004** y uno de mis ídolos friki [**Aaron Swartz**](https://es.wikipedia.org/wiki/Aaron_Swartz){: target="_blank" rel="noopener"} (*QEPD*) aporto contribuciones importantes en el desarrollo de la sintaxis.

En un principio Markdown fue desarrollado como una herramienta que permitiera una conversión amigable de texto plano a código HTML que evitara tener que escribir los pares de etiquetas propias de este lenguaje de marcado con el que se estructuran las páginas web.

Es decir, escribías tus textos en Markdown y en un vuelo tenias un documento HTML valido y estructurado con sus respectivas etiquetas h1, p, strong, ol y ul.

Claro eso fue en un principio, ya que con la popularidad alcanzada por el lenguaje ahora es implementado en muchos sitios de *microblogging* y utilizado por escritores y redactores profesionales.

## Sintaxis Markdown.

La sintaxis no es más que "las reglas de escritura propias de cada lenguaje", por ejemplo, el idioma Español tiene sus reglas de sintaxis, como escribir la primera letra en mayúscula al principio de un escrito o después de un punto y a parte.

Markdown al ser considerado un lenguaje aunque no lingüístico, también tiene su propia sintaxis, así que hay parámetros sintácticos explícitamente establecidos que debemos seguir.

Por ejemplo: si queremos resaltar un texto en negritas este debe llevar dos asteriscos **\**** al principio y al final de la palabra. Esto solo es uno de los tantos parámetros de formateado que existen en este lenguaje. 

Cabe acotar que, la sintaxis que nació junto a Markdown no es un estándar, la necesidad de añadir nuevas características sobre la base creada por **Jhon Gruber** y **Aaron Swartz** considerado por muchos como obsoleto, ha dado paso a lo que se conoce como Markdown flavors o sabores de Markdown esto lo veremos más delante; por ahora adentrémonos en la sintaxis básica de Markdown.

### Párrafos.

Los párrafos en Markdown se escribe como en cualquier otro editor de texto, no llevan ninguna sintaxis especial, el lenguaje al detectar que dicho escrito no lleva consigo algún comando de formateado lo interpretara como un párrafo.

**Entrada**:

{% highlight markdown %}
Estos es un párrafo escrito en Markdown.
{% endhighlight %}

**Salida**:

Esto es un párrafo escrito en Markdown.

### Títulos o encabezados.

Los títulos o encabezados en Markdown se genera con un signo numeral **\#** y la especificidad de cada uno se establece por el numero de **\#** que lo antecedan. 

Por ejemplo: si queremos un título de primer nivel bastaría con un **\#**, en cambio si queremos un subtitulo debería antecederlo dos **\#** y así sucesivamente hasta el ultimo nivel que serian seis **\#**.

También hay dos comandos de formateado con alcance para los dos primeros niveles de título, siendo estos el signo igual **=** para los títulos de nivel 1 y el guion **-** para el nivel 2.

**Entrada**:

{% highlight markdown %}
# Título 1
## Título 2
### Título 3
#### Título 4
##### Título 5
###### Título 6

Título 1
=

Título 2
-
{% endhighlight %}

**Salida**:

**\# Título 1**. Por razones de **SEO** he marcado este título para que no sea interpretado como tal, ya que un artículo o post redactado para la web no debe llevar más de un encabezado de primer nivel (h1) para no romper la estructura semántica. 

## Título 2

### Título 3

#### Título 4

##### Título 5

###### Título 6

### Negritas.

Para resaltar un palabra en negritas debes usar dos **\**** al principio y final de la palabra. También puedes usar dos guiones bajos **\__** para lograr el mismo objetivo.

Como buena practica sintáctica, si comienzas resaltando texto en negritas con los asterisco deberías mantener estos en el resto del documento.

**Entrada**:

{% highlight markdown %}
**Esto es un texto en negritas con dos asteriscos**.

__Esto es un texto en negritas con dos guiones bajos__.
{% endhighlight %}

**Salida**:

**Esto es un texto en negritas**.

### Cursivas.

Para las cursivas puedes usar un **\*** al principio y final de la palabra. También puedes utilizar un guion bajo **\_** para obtener el mismo resultado.

**Entrada**:

{% highlight markdown %}
*Esto es un texto en cursiva con un asterisco*.

_Esto es un texto en cursiva con un guion bajo_.
{% endhighlight %}

**Salida**:

*Esto es un texto en cursiva*.

### Texto tachado.

El texto tachado se obtiene con dos pares de *virgulillas* **\~** o como yo le llamo "acento de la eñe". Para sacar la *virgulillas* en el teclado presiona la combinación de teclas `Alt Gr + 4`.

**Entrada**:

{% highlight markdown %}
~~Esto es un texto tachado~~
{% endhighlight %}

**Salida**:

~~Esto es un texto tachado~~.

### Enlaces.

Los enlaces se establecen de la siguiente manera: **\[Texto del enlace](url del enlace "Título del enlace")** entre los corchetes iría el texto visible y dentro de los paréntesis iría la url, si por el contrario quieres mostrar la url el marcado seria el siguiente: **\<url del enlace>**.

**Entrada**:

{% highlight markdown %}
[Este es mi enlace](https://www.leninalbertop.com.ve "Este es mi enlace")

<https://www.leninalbertop.com.ve>
{% endhighlight %}

**Salida**:

[Este es mi enlace](https://www.leninalbertop.com.ve "Este es mi enlace")

<https://www.leninalbertop.com.ve>

### Imágenes.

El marcado para las imágenes es similar al de los enlaces solo que se debe anteponer el signo de exclamación **\!** quedando de la siguiente manera: **\!\[Texto alternativo ALT](url de la imagen "Título de  la imagen")**.

**Entrada**:

{% highlight markdown %}
![Una imagen asombrosa](/image/mi-asombrosa-imagen.webp "Esta imagen si que esta cool.")
{% endhighlight %}

**Salida**:

![Una imagen asombrosa](/images/img-post/una-imagen-asombrosa.webp "Esta imagen si que esta cool.")

### Listas ordenadas.

Las listas ordenadas se generan utilizando números en orden ascendete, es decir comienza con el **número 1** y va ascendiendo según la cantidad requerida.

**Entrada**:

{% highlight markdown %}
1. Lista ordenada 1
2. Lista ordenada 2
3. Lista ordenada 3
{% endhighlight %}

**Salida**:

1. Lista ordenada 1
2. Lista ordenada 2
3. Lista ordenada 3

También puedes crear sublistas dentro de una lista. Solo debes "sangrar" tres espacios para crearlas.

**Entrada**:

{% highlight markdown %}
1. Lista ordenada 1
2. Lista ordenada 2
   1. Sublista 1
   2. Sublista 2
3. Lista ordenada 3
{% endhighlight %}

**Salida**:

1. Lista ordenada 1
2. Lista ordenada 2
   1. Sublista 1
   2. Sublista 2
3. Lista ordenada 3

### Listas desordenadas.

Las listas desordenadas se pueden generar a partir de los siguientes signos: **\-**, **\+**, **\***. Puedes usar una combinación de ellos para generar tu lista desordenada pero nuevamente te recuerdo que lo ideal es mantener una sintaxis coherente. Yo suelo usar los asterisco.

**Entrada**:

{% highlight markdown %}
* Lista desordenada 1
* Lista desordenada 2
* Lista desordenada 3
{% endhighlight %}

**Salida**:

* Lista desordenada 1
* Lista desordenada 2
* Lista desordenada 3

Para las sublista se aplica los mismo que en la lista ordenada.

**Entrada**:

{% highlight markdown %}
* Lista desordenada 1
* Lista desordenada 2
  * Sublista 1
  * Sublista 2
* Lista desordenada 3
{% endhighlight %}

**Salida**:

* Lista desordenada 1
* Lista desordenada 2
   * Sublista 1
   
   * Sublista 2
* Lista desordenada 3

### Citas o Blockquotes.

Para generar bloques de citas se utiliza el signo o caracter mayor que **\>**.

**Entrada**:

{% highlight markdown %}
> Todos somos muy ignorantes, lo que ocurre es que no todos ignoramos las mismas cosas. -Albert Einstein
{% endhighlight %}

**Salida**:

> Todos somos muy ignorantes, lo que ocurre es que no todos ignoramos las mismas cosas. -Albert Einstein

### Bloques de código.

Los bloques de código se generan de la siguiente manera: usando un par del caracter o signo **\`** conocido en informática como *backticks* dará como resulta un bloque de código en lineá.

**Entrada**:

{% highlight python %}
`Print("¡Que tal, Universo!")`
{% endhighlight %}

**Salida**:

`Print("¡Que tal, Universo!")`

Para bloques de código más extensos se debe de utilizar tres pares de *backticks*, llevando el trio superior la referencia al lenguaje en el que se escribe.

**Entrada**:

{% highlight markdown %}
```python
my_variable = "¡Que tal, universo!"

print(my_variable)
```
{% endhighlight %}

**Salida**:

{% highlight python %}
my_variable = "¡Que tal, universo!"

print(my_variable)
{% endhighlight %}

### Tablas.

Las tablas Markdown son quizás "lo que más canas saca", sobre todo si estas son complejas ya que el lenguaje no fue creado para reemplazar a HTML. En línea general la estructura de una tabla en Markdown sería la siguiente.

**Entrada**:

{% highlight markdown %}
| uno  | dos    | tres  |
| ---- | :----: | ----: |
| tres | dos    | uno   |
| uno  | dos    | tres  |
| tres | dos    | uno   |
{% endhighlight %}

**Salida**:

| uno  | dos  | tres |
| ---- | :--: | ---: |
| tres | dos  |  uno |
| uno  | dos  | tres |
| tres | dos  |  uno |

Los dos puntos **:** en los guiones de la tabla hacen referencia a la alineación que tendrá cada celda.

Guiones sin puntos es la alineación por defecto a la izquierda, dos puntos al principio y final de los guiones es una alineación centrada, dos puntos al final de los guiones alinea el contenido a la derecha, dos punto al principio de los guiones cumple el mismo objetivo de la alineación por defecto.

### Caracter de escape.

En este punto seguro ya te haz dado cuenta que Markdown utiliza caracteres conocidos en nuestro idioma cotidiano; asteriscos, signo de exclamación, corchetes, paréntesis.

Dichos signos o caracteres son interpretados por el lenguaje como operadores de formateado y serán leídos de esta manera a menos que explícitamente le indiquemos que no lo haga.

Para lograr este fin debemos colocar la barra invertida **\\** o *backslash* en inglés por delate del operador de formateado. Ejemplo: **\\+** aquí le pido a Markdown que el signo **\+** que sirve para crear listas, sea interpretado como eso, un signo de suma y no un elemento de formateado.

## Markdown Flavors.

En un principio no todo era perfecto en Markdown, la base original de la sintaxis creada en 2004 por **Jhon** y **Aaron** no era explicita sobre algunas reglas que trajeron consigo muchas preguntas sin respuestas algunas de ellas eran.

* ¿Cuantas sangrías se necesitan para una sublista?
* ¿Se necesita una línea en blanco antes de una comilla o encabezado?
* ¿Se necesita una línea en blanco antes de un bloque de código sangrado?
* ¿Pueden los elementos de una lista estar vacíos?

Sin existir una variable que diera respuesta a estas preguntas no faltaron los que se adentraron a consultar la base para tratar de resolver estas ambigüedades, pero se encontraron que la base de Markdown era bastante defectuosa  y arrojaba errores muy malos en muchos casos al tratar de solventar lo antes mencionado.

¡*Eh aquí el talón de Aquiles de Markdown*! nacieron los sabores de Markdown que propiamente dicho serian nuevas versiones sobre la base original que técnicamente podríamos llamarle fragmentación.

Para muchos, un motivo para huir de Markdown como lo explica **Eric Holscher** en su artículo [Por qué no deberías usar Markdown](https://www.ericholscher.com/blog/2016/mar/15/dont-use-markdown-for-technical-docs/){: target="_blank" rel="noopener"}.

Para otros tantos aplica el dicho *en la variedad esta el gusto*, en fin. Quizás el sabor más implementado es  **CommonMark** que vino a sentar una base claramente definida para una sintaxis estándar e inequívoca para Markdown.

Existen sabores de Markdown más que los dedos de mis manos, la mayoría toman a Markdown y CommonMark como base. Aquí una listo de algunos de los más utilizados.

* [CommonMark](https://commonmark.org/){: target="_blank" rel="noopener"}
* [Github flavors](https://github.github.com/gfm/){: target="_blank" rel="noopener"}
* [kramdown](https://kramdown.gettalong.org/){: target="_blank" rel="noopener"}

Para un lista con sabores más extensa visita el siguiente [**Link**](https://github.com/commonmark/commonmark-spec/wiki/markdown-flavors){: target="_blank" rel="noopener"}.

## Editor Markdown.

Por regla general hasta el bloc de notas te sirve para escribir en Markdown, pero no es el editor acorde para  ello, sobre todo si estas empezando con el lenguaje.

![Markdown en Bloc de notas](/images/img-post/markdown-bloc-de-notas.webp "Escribiendo Markdown en el Bloc de notas")

La razón principal es que no tiene un soporte adecuado y por tal motivo no cuenta con resaltado de sintaxis, vista previa o capacidad de exportación a otros formatos tales como docx, pdf, html.

Un editor para Markdown viene a facilitar las cosas ya que incluyen lo mencionado en el párrafo anterior, a demás de incluir atajos de teclado para insertar los operadores de formateado, soporte para varios sabores y una "interfaz parecida al de Microsoft Word".

La variedad de editores Markdown es tal, cual confeti para arrojar por los aires. 

Los hay para escritorio y smartphone, de pagos, gratis y hasta on-line por este ultimo comenzaremos este recorrido, eso si no esperes una lista extensa en este post porque no la va haber. La razón es que no quiero abrumarte por ello solo listare "los más populares".

### Editores Markdown On Line.

Tal vez la mejor opción para tener un primer contacto. Comencemos.

* [**Stackedit**](/stackedit-editor-markdown){: target="_blank" rel="noopener"} Es mi editor on line preferido, Stackedit cuenta con varios agregados estupendos como iniciar Sesión con tu cuenta de Google, Github, Gitlab para almacenar tus documentos en la nube, vista previa con desplazamiento en vivo, espacios de trabajo colaborativos, soporte para los sabores Markdown Extra, CommonMark y Github Flavor.
* [**Dillinger**](https://dillinger.io/){: target="_blank" rel="noopener"} Dillinger esta desarrollado en Angular, cuenta con vista previa e inicio de sesión con Dropbox, Google Drive, One Drive, Github para almacenar documentos en la nube.
* [**Hackmd**](https://hackmd.io/){: target="_blank" rel="noopener"} Permite trabajo colaborativo en tiempo real, vista previa, capacidad de exportar Markdown en otros formatos
* [**Stackeditpro**](https://stackeditpro.io/){: target="_blank" rel="noopener"} Esto es un Fork de Stackedit pero con baterías recargadas.

### Editores Markdown para Escritorio.

* [**Typora**](https://typora.io/){: target="_blank" rel="noopener"} Es el editor que utilizo en mi pc, en combinación con mi editor de código VScode le dan vida a los post de este blog. Typora tiene una vista previa un tanto diferente al resto de editores ya que este se produce sobre la marcha.
* [**Haroopad**](http://pad.haroopress.com/user.html){: target="_blank" rel="noopener"} Un potente editor gratuito disponible para Windows, Linux y MacOS, Github Flevor mas extensiones, exportación a otros formatos.
* [**Writemonkey**](http://writemonkey.com/){: target="_blank" rel="noopener"} Es un editor minimalista en todos los sentidos, cuenta con características igual que los anteriores. Pese a poder usarse de forma gratuita si haces una donación monetaria recibirás una clave que te permitirá desbloquear extras adicionales. 
* [**Visual Studio Code**](https://code.visualstudio.com/){: target="_blank" rel="noopener"}, [Sublime Text](https://www.sublimetext.com/){: target="_blank" rel="noopener"}, [Atom](https://atom.io/){: target="_blank" rel="noopener"} Meramente, no son editores exclusivos para Markdown pero cuentan con infinidades de plugins que les permiten trabajar de buena manera con este lenguaje.

Hasta aquí llega este post, espero que pueda serte de ayuda. Recuerda que estoy abierto a tus preguntas y puedes formularlas en el apartado de comentarios.