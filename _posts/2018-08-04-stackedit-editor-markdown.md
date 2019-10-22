---
layout: post
image: /images/img-post/stackedit-editor-markdown.webp
title: Stackedit un potente editor Markdown a tener en cuenta.
description: "Stackedit es un Potente editor Markdown Online, cuenta con sincronización en Google, Dropbox y Github, y puedes usarlo con o sin conexión a Internet."
date: 2018-08-31 10:00:00
tags: [aplicaciones]
author: leninalbertop
---
Hay muchos editores de markdown allá afuera, tantos que fue difícil para mí elegir uno que se adaptara a mis necesidades.

## Pero ¿Qué es markdown?

Es un formato de texto plano para escribir documentos estructurados, basándose en las convenciones de formato de correo electrónico y Usenet. Fue desarrollado en 2004 por John Gruber, quien escribió el primer convertidor de Markdown a HTML en Perl, y pronto se hizo ampliamente utilizado en sitios Web. En 2014 había docenas de implementaciones en muchos idiomas.


## Que busco de un editor markdown

La verdad no soy muy exigente con los editores markdown porque solo lo uso para escribir en este blog y para escribir las documentaciones de mis repositorios en github, así que de ellos pido que se puedan ejecutar offline, que cuente con corrector ortográfico para el español y si es posible que sea gratuito y open source para de alguna manera poder retribuir la gratuidad.

En esa búsqueda encontré a [**Stackedit**](https://stackedit.io/){: target="_blank" rel="noopener noreferrer"}, un editor markdown que supera con creces las características necesarias para mi, ya que se puede ejecutar offline y ni siquiera requiere de instalación debido a que este funciona desde el navegador web, esto quiere decir que aprovecha las ventajas que esto supone incluyendo el corrector ortográfico.

## Características de stackedit.

### Espacios de trabajos.

Los espacios de trabajos son la forma en que  stackedit almacena la configuración y los documentos que creas y funcionan de dos maneras, la primera mediante la APi IndexedDB del navegador web una base de datos ligera y no muy recomendada ya que si borras los datos o desinstalas el navegador perderás todos tus escritos. Y la segunda, y la que que recomiendan es mediante el inicio de sesión con tu cuenta de google, al hacerlo tu espacio de trabajo se almacena en google drive en la [**carpeta datos de aplicación**](https://developers.google.com/drive/api/v3/appdata){: target="_blank" rel="noopener noreferrer"}, también puedes crear un espacio de trabajo permitiendo el acceso a tu google drive donde se creará una carpeta la cual podrás compartir con quien lo desees.

### Sincronización.

Podrás sincronizar tus archivos con dropbox, google driver o github, quizás esta opción no te haga sentir muy cómodo ya que requiere que le otorguen permisos de lectura y escritura para poder almacenar y traer de vuelta los archivos, aunque en stackedit dicen que los tokens de acceso solo se almacenan en el navegador y no son enviados a otro servidor o terceras partes.

### Publicar directamente en la web.

Puedes publicar directamente un documento en plataformas como wordpress, blogger, zendesk y github.

## Otras características

 - Gratuito y open source
 - Vista previa en tiempo real
 - Modo sin distracción o pantalla completa
 - Puedes crear un acceso directo en tu pc para que funcione como una PWA en una ventana
 - Editor WYSIWYG
 - Cuenta con un cheat sheet (chuleta) de markdown
 - Importar y exportar desde tu pc
 - Soporte para diagramas LaTeX math
 - Admite varios sabores de markdown

Sin duda es un editor muy completo que merece la pena darle una oportunidad, y tu ¿Qué editor markdown usas?