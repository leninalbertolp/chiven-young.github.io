---
layout: post
image: /images/img-post/vulnerabilidad-winrar.webp
title: Si usas WinRaR estas expuesto a ser Hackeado.
description: "WinRaR llevaba 19 años con un fallo de seguridad que fue parcheado recientemente en su última versión pero aún es explotada por los delincuentes informáticos."
date: 2019-03-18 10:00:00
tags: [aplicaciones]
author: leninalbertop
---
El popular software de compresión de archivos para Windows **WinRAR con más de 500 millones de usuarios** a sus espalda está en la mira de los delincuentes informáticos debido a una vulnerabilidad crítica de **Recorrido de Ruta Absoluta**.

Esta brecha de seguridad compromete **todas las versiones de WinRAR de los últimos 19 años** y aunque la compañía lanzó una actualización del programa donde se corregía el fallo, **esta sigue siendo explotada activamente por los delincuentes informáticos** ya que **WinRAR no cuenta con un sistema de actualizaciones automáticas**.

## 500 Millones de usuarios de WinRAR en todo el mundo expuestos a un fallo de seguridad.

Así es, **toda la base de usuarios de WinRAR están expuestos a esta vulnerabilidad** que se cuenta casi desde los propios inicios del Software, debido a que WinRAR no cuenta con actualizaciones automáticas que instale la nueva versión que soluciona el problema.

Si eres usuario de WinRAR tendrás que [**descargar e instalar manualmente la versión 5.70**](https://www.win-rar.com/start.html?&L=6){: target="_blank" rel="noopener noreferrer"} para vacunarte ante los peligros que representa este fallo de seguridad.

Otra de las cosas que puedes hacer es desinstalar WinRAR y [**reemplazarlo por 7Zip**](https://www.7-zip.org/){: target="_blank" rel="noopener noreferrer"} un programa tan potente como WinRAR pero **gratuito y Open Source**.

## ¿Donde reside la vulnerabilidad crítica?.

Los expertos de Check Point dieron detalles técnico sobre la vulnerabilidad explicando que la falla reside en la biblioteca de tercero **UNACEV2.DLL** utilizada para descomprimir archivos con **extensión ACE** (.ace), ACE es un formato de fichero de archivo para compresión de datos.

<iframe width="768" height="450" src="https://www.youtube-nocookie.com/embed/R2qcBWJzHMo" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Ya que WinRAR detecta el formato por el contenido del archivo y no por la **extensión .ace**, los delincuentes informáticos pueden perfectamente cambiar la **extensión a .rar** para que "se vea normal" y poder llevar a cabo la infección del virus.

Debido a que la vulnerabilidad es el error del **Recorrido de Ruta Absoluta** el atacante puede extraer un archivo infectado (virus) en la carpeta de inicio de Windows.

## Cómo se está aprovechando este fallo de seguridad en WinRAR.

Como ya lo comente, WinRaR no cuenta con un sistema de actualizaciones automática, por lo que para poder descargar la actualización que corrige la vulnerabilidad primero debes estar informado de dicho fallo (ahora ya lo estas 😉) y segundo descargar la actualización manualmente.

he aquí donde los delincuentes informáticos entran en acción ya que la gran mayoría de esos usuarios ni siquiera sabrán qué su software de descompresión WinRaR tiene un fallo que compromete su seguridad, y seguirán usándolo como si nada pasara.

El principal señuelo es la música, se pudo conocer que el **exitoso álbum de Ariana Grande "Thank U, Next"** se distribuye con el nombre de archivo "**Ariana_Grande-thank_u, _next (2019) _ [320] .rar**" en sitios de descargas piratas, este archivo viene con la vulnerabilidad de WinRaR explotada, por lo que al descomprimirlo tu sistema queda infectado.

Pero no te engañes, los delincuentes informáticos no solo utilizaran la música para aprovechar esta vulnerabilidad.

A la fecha de este artículo solo [**30 motores de antivirus han detectado la amenaza**](https://www.virustotal.com/#/file/a1c06018b4e331f95a0e33b47f0faa5cb6a084d15fec30772923269669f4bc91/detection){: target="_blank" rel="noopener noreferrer"}.

Quedas advertido, si usas WinRAR ve ya ya ya a actualizarlo.

¿Qué notición no? yo me libre porque desde hace varios años utilizo 7zip 😓, ¿y tú qué software de descompresión utilizas?

Visto en: [**The Hacker News**.](https://thehackernews.com){: target="_blank" rel="noopener noreferrer"}