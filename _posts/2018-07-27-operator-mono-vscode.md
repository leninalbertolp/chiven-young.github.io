---
layout: post
image: /images/img-post/operator-mono-vscode.webp
title: Configurar Operator Mono en Visual Studio Code.
description: "Aprende a configurar Operator Mono en cualquier theme de Visual Studio Code, Operator Mono la fuente tipográfica que enamora a los programadores."
date: 2018-07-27 10:00:00
tags: [desarrollo-web]
author: leninalbertop
---
Operator mono es una fuente monoespaciada caracterizada por incluir un tipo de letra cursiva que le dan un toque diferente al código que escribimos, bueno realmente esto sería lo más superficial de esta fuente ya que su creador detalla los procesos de su creación en este [post](https://www.typography.com/blog/introducing-operator){: target="_blank" rel="noopener noreferrer"}.

Una fuente muy bonita y amigable a la lectura pero con un valor de $200 que lleva a muchos a cuestionarse si vale la pena soltar tantos trump por una fuente.

Si usted fue una de esas personas que valoro el trabajo que conlleva crear una fuente y la compro, pues entonces has llegado al lugar indicado porque te mostrare a como configurarla sin mucho lío en cualquier theme de vscode para que pueda mostrar el tipo de letra cursiva.

Presiona la combinación de tecla `Ctrl`+`,` para abrir la configuración de usuario y establece operator mono como fuente principal de la siguiente manera `"editor.fontFamily": "'Operator Mono', Consolas, 'Courier New', monospace",`.

A continuación copia y pega el siguiente bloque de código en tu archivo de configuración, y reemplazar donde dice `Nombre del theme` por el nombre del theme que estés utilizando.

{% highlight json %}
"editor.tokenColorCustomizations": {
  "[Nombre del theme]": {
    "textMateRules": [{
      "scope": [
        "comment",
        "punctuation.definition.comment",
        "comment.block",
        "comment.line",
        "comment.block.documentation",
        "comment.line.double-slash",
        "entity.other.attribute-name",
        "entity.other.attribute-name.html",
        "markup.italic",
        "entity.other.attribute-name.id",
        "entity.other.attribute-name.class.css",
        "entity.other.attribute-name.tag.jade",
        "entity.other.attribute-name.class.jade",
        "entity.other.attribute-name.id.jade",
        "keyword.control",
        "storage",
        "emphasis",
        "variable.language"
      ],

      "settings": {
        "fontStyle": "italic"
      }
    }]
  }
}
{% endhighlight %}

Listo eso es todo, ahora ya tienes una configuración adecuada para operator mono. Happy dev 👨‍💻
