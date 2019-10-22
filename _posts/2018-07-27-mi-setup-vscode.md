---
layout: post
image: /images/img-post/setup-vscode.webp
title: Mi setup en Visual Studio Code.
description: "Así tengo configurado mi editor de código Visual Studio Code, y te muestro los Plugins y Themes que uso en este popular editor Open Source creado por Microsoft."
date: 2018-07-27 09:30:00
tags: [desarrollo-web]
author: leninalbertop
---
Que pasa coders, en este pequeño post te mostrare el setup que tengo actualmente en visual studio code (vscode para los amigos), los theme, extensiones y un poco de mi setting.js. Nada más así que comencemos.

## VSCode Themes.

![One Dark Pro Visual Studio Code Theme](https://raw.githubusercontent.com/Binaryify/OneDark-Pro/master/static/screenshot1.png){: width="768"}

Desde que estoy usando este editor de código muchos han sido los temas visuales que han desfilado frente a mis ojos, de ellos puedo nombrarte algunos de los siguientes: [Dracula](https://marketplace.visualstudio.com/items?itemName=dracula-theme.theme-dracula){: target="_blank" rel="noopener noreferrer"} el de la old school, [material theme](https://marketplace.visualstudio.com/items?itemName=Equinusocio.vsc-material-theme){: target="_blank" rel="noopener noreferrer"} este fue muy popular en sublime text, [nord](https://marketplace.visualstudio.com/items?itemName=arcticicestudio.nord-visual-studio-code){: target="_blank" rel="noopener noreferrer"}, [panda theme](https://marketplace.visualstudio.com/items?itemName=tinkertrain.theme-panda){: target="_blank" rel="noopener noreferrer"} y [ayu](https://marketplace.visualstudio.com/items?itemName=teabyii.ayu){: target="_blank" rel="noopener noreferrer"}, pero el que mejor se ha adaptado a mis exquisitos y refinados gusto (sarcasmo) ha sido [one dark pro](https://marketplace.visualstudio.com/items?itemName=zhuangtongfa.Material-theme){: target="_blank" rel="noopener noreferrer"}, así que este es el que estoy usando actualmente junto al pack de iconos [Vscode Icons](https://marketplace.visualstudio.com/items?itemName=robertohuertasm.vscode-icons){: target="_blank" rel="noopener noreferrer"}.

## VSCode Extensions.

Los plugins que utilizo en vscode son muy pocos y están enfocado al front-end el workspace en el que me desenvuelvo. Nada del otro mundo. 😉

### Materializecss Snippets.

![Materialize Snippets Visual studio code plugin](https://github.com/leninalbertolp/materialize-snippets-vscode/raw/master/images/mz-example.jpg){: width="768"}

Como no podía ser de otra manera comienzo con el plugin de la casa, materialize snippets es una colección de bloques de código del framework [materialize](https://materializecss.com/){: target="_blank" rel="noopener noreferrer"} y nació como una necesidad al trabajar en un proyecto para un cliente basado en este framework.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=leninp.materialize-snippets){: target="_blank" rel="noopener"}

### Auto close tag.

![Auto close tag](https://github.com/formulahendry/vscode-auto-close-tag/raw/master/images/usage.gif){: width="768"}

Este plugin inserta automáticamente la etiqueta de cierre, cosa que vscode posee desde la versión 1.16 pero solo para HTML, Handlebars y Razor, así que este plugin añade soporte para otros tipos de extensiones como javascript, php, typescript entre otros.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-close-tag){: target="_blank" rel="noopener"}

### Auto rename tag.

![Auto rename tag](https://github.com/formulahendry/vscode-auto-rename-tag/raw/master/images/usage.gif){: width="768"}

Como puedes apreciar en la imagen, este plugin te permite renombrar el par de etiqueta html de un solo jalón.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=formulahendry.auto-rename-tag){: target="_blank" rel="noopener"}

### Auto file name.

![Auto file name](https://trello-attachments.s3.amazonaws.com/56c86fd76bf599f4fa62ee7f/1152x720/4b439177b0fb1c04af133aa733ba2a09/Untitled.gif){: width="768"}

Vscode ya cuenta con esta función de forma nativa pero solo para archivos html y css, así que este plugin viene a completar el binomio.

Auto file name navega por las carpetas de tu proyecto y te ayuda a completar la ruta para la inserción de imágenes o de otros archivos.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=JerryHong.autofilename){: target="_blank" rel="noopener"}

### Beautify.

Un plugin para embellecer código html, css, scss, json y javascript, yo lo uso mucho para formatear los archivos de otros coders acorde a mi workspace.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=HookyQR.beautify){: target="_blank" rel="noopener"}

### IntelliSense for CSS class name in HTML.

![IntelliSense for CSS class names in HTML](https://i.imgur.com/5crMfTj.gif){: width="768"}

Como puedes apreciar en la imagen este plugin de vscode recolecta y almacena en cache los nombres de las clases e id de tus archivos css para luego ayudarte a insertarlos en tu html, muy útil si trabajas con framework css, funciona tanto para archivos locales como para los enlaces de CDN.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=Zignd.html-css-class-completion){: target="_blank" rel="noopener"}

### Spell right.

![Code Spell Checker](https://raw.githubusercontent.com/bartosz-antosik/vscode-spellright/master/media/screenshot-documents.png){: width="768"}

"Quien esté libre de pecado que arroje la primera piedra". Un corrector ortográfico para evitar esos errores comunes que solemos cometer cuando escribimos.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=ban.spellright){: target="_blank" rel="noopener"}

### Jekyll syntax support, jekyll snippets.

Ahora que he dado el salto de wordpress a jekyll estos plugins forman parte de mi stack de desarrollo. Este par de extensión añade soporte para el resaltado de la sintaxis de jekyll.

[**Jekyll sintax**](https://marketplace.visualstudio.com/items?itemName=ginfuru.ginfuru-vscode-jekyll-syntax){: target="_blank" rel="noopener"} - [**Jekyll Snippets**](https://marketplace.visualstudio.com/items?itemName=ginfuru.vscode-jekyll-snippets){: target="_blank" rel="noopener"}

### Live server.

![**Live server**](https://github.com/ritwickdey/vscode-live-server/raw/master/images/Screenshot/vscode-live-server-animated-demo.gif){: width="768"}

Un potente servidor local con auto refresh incluido.

[**Ver extensión**](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer){: target="_blank" rel="noopener"}

## Algunas de las modificaciones en mi settings.js

{% highlight json %}
"editor.fontFamily": "'Menlo, Consolas, 'Courier New', monospace",
"editor.fontSize": 16.8,
"editor.letterSpacing": 0.5,
"editor.lineHeight": 24,
"editor.fontWeight": "normal",
"editor.tabSize": 2,
"editor.detectIndentation": true,
"editor.fontLigatures": true,
"editor.renderWhitespace": "boundary",
"editor.wordWrap": "on",
"editor.minimap.enabled": true,
"editor.minimap.renderCharacters": true,
"editor.wrappingIndent": "same",
"editor.renderControlCharacters": true,
"editor.renderIndentGuides": true,
"editor.dragAndDrop": true,
"telemetry.enableTelemetry": false,
"telemetry.enableCrashReporter": false,
"editor.quickSuggestions": {
  "other": true,
  "comments": true,
  "strings": true
},
"files.autoSave": "off",
"editor.multiCursorModifier": "ctrlCmd",
"extensions.autoUpdate": false,
"editor.smoothScrolling": true,
"emmet.triggerExpansionOnTab": true,
"emmet.showSuggestionsAsSnippets": true,
"editor.snippetSuggestions": "top",
"auto-close-tag.SublimeText3Mode": true,
"window.zoomLevel": 0,
"git.autofetch": true,
"terminal.integrated.shell.windows": "C:\\Windows\\System32\\bash.exe",
"markdown.preview.fontSize": 15
{% endhighlight %}

Con esto último vamos llegando al final de este post, Y tu ¿Qué plugins y themes utilizas en vscode? me gustaría que los mencionaras en los comentarios.