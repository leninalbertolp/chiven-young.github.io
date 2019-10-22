---
layout: post
image: /images/img-post/wsl-windows10.webp
title: Habilitar Windows Subsystem for Linux en Windows 10.
description: "Windows Subsystem for Linux en Windows 10 es la puesta en marcha por parte de Microsoft para que los desarrolladores en Linux se den una pasadita por el SO de Redmond."
date: 2018-08-31 10:00:00
tags: [desarrollo-web]
author: leninalbertop
---
"Microsoft ama a linux" fueron las palabras de Satya Nadella CEO de microsoft en una conferencia sobre cloud, de esta manera linux pasaría de ser un "cáncer" palabras de su antiguo CEO Steve Ballmer, a parte fundamental de sus servicios en la nube Windows Azure.

Así comenzó el romance entre microsoft y linux, hoy día microsoft es uno de los mayores contribuidores del open source, miembro platino de la linux foundation y dueño de github, pero pasemos a lo que vinimos porque estos son temas para otro topic.

## Qué es Windows Subsystem for Linux o WSL.

Es un espacio en windows que provee una interfaz que simula un kernel de Linux (sin contener código de Linux propiamente dicho),​ el cual puede correr aplicaciones de espacio de usuario GNU, por ejemplo, una instalación base de Ubuntu, openSUSE,​ SUSE Linux Enterprise Server,​ Debian​ y Kali Linux. Dicho entorno puede contener una shell Bash, junto con ejecutables de línea de comandos GNU/Linux nativos (sed, awk, etc.), lenguajes de programación (Ruby, Python, etc.), e incluso algunas aplicaciones gráficas (con la ayuda de un servidor X11).

## Lo que necesitas saber sobre Windows Subsystem for Linux.

Técnicamente esto no es linux, linux es el corazón de las distribuciones que se basan en este kernel, lo que nos permite WSL es tener un entorno empotrado por llamarlo de alguna manera, que nos permite ejecutar el shell bash y los binarios que normalmente corremos en ubuntu o en cualquier otra distro linux exceptuando aquellas con interfaz gráficas.

***

**También te podría interesa**:

[**Instalar ZSH y Oh My ZSH en Windows**](/instalar-zsh-ohmyzsh-windows10)

[**Cambiar idioma al bash de Ubuntu en Windows**](/cambiar-idioma-bash-ubuntu-windows10)

***

## Habilitar Windows Subsystem for Linux.

Lo primero que debes saber es que WSL solo funciona en arquitectura de 64 bits, si tu sistema es de 32 bits no podrás usar esta característica.

![Características Windows WSL](https://lh3.googleusercontent.com/pp8JEROWUQjSnyrHxWYhucZ-KOolviH1Lwv_Gt4zZKNiI87ePtvXBrzzbgL8PouCluJfXsaAnjwI=s768)

En cortana escribe `activar o desactivar las características de windows`, y en la ventana que se abre busca y activa `Subsistema de Windows para Linux` al activar esta opción te saldrá otra ventana donde te indica que se descargara esta característica, cuando finalice te pedirá que reinicies el sistema para completar la instalación.

![Ubuntu Windowa Subsystem for Linux](https://lh3.googleusercontent.com/_MD9y6jio_ts_AjrC0TsvOgcXEwRIBCMZtJsWlM68WXnhg_MAbMdlwdIrwJtvpYQMLmcXefSWHgo=s768)

Ya tenemos instalado el subsistema ahora nos falta una distro, para ello abre la microsoft store y busca ubuntu, o elige la distro de tu preferencia.

Luego que se descargue busca en cortana ubuntu y ejecuta el programa, se te abrirá la consola de comando que en este caso será el shell de ubuntu y dirá que necesita descargar algunas cosas, luego de eso te pedirá qué reinicies el sistema para completar la instalación.

![Ubuntu Shell Windows Subsystem for linux](https://lh3.googleusercontent.com/ozlopVzCEZ0XQ0UdxPA7UJPQOgUjJ7TMA1p1tp4AjvEveK_cs47N1ynroG33NsLpWmBjVypZpT7S=s768)

Después del reinicio toca abrir nuevamente ubuntu para terminar el proceso de configuración, en el que te pedirá que introduzcas un nombre y contraseña para crear el usuario.

![Sudo apt update ubuntu windows subsystem for linux](https://lh3.googleusercontent.com/vpxG-b6c07GsLmy88DlBggafyJ6oAQh4b9GJqwytU_f3sLF3uHN5yORcHJLcdpq8UjrKeQ_xU0wY=s768)

Lo siguiente que debes hacer es ejecutar el siguiente comando `sudo apt update` para actualizar la lista de paquetes y a continuación `sudo apt upgrade` para actualizar aquellos paquetes que sean necesarios.

**Nota**: ejecuta periódicamente `sudo apt update` y `sudo apt upgrade` para mantener tu subsistema actualizado.

## Y, ¿ahora qué?

Pues nada, "a convertirse en hacker". 🤪

Ya te había comentado que no se pueden ejecutar aplicaciones con interfaz gráfica, pues no es del todo cierto ya que si lo puedes hacer pero mediante servidores gráficos como [Xming X](https://sourceforge.net/projects/xming/){: target="_blank" rel="noopener noreferrer"} pero de igual forma con sus limitantes a mayor complejidad de la aplicación mayor sera la probabilidad de que no funcione debido a que el subsistema de windows para linux está pensado solo para correr aplicaciones que se ejecuten en consola y [aquí tienes una buena lista de ellas](https://blog.desdelinux.net/las-mejores-aplicaciones-para-usar-desde-el-terminal/){: target="_blank" rel="noopener noreferrer"} por si quieres experimentar.

Lo que sí puedes instalar sin problemas son herramientas de desarrollo que funcionan mejor en linux o mac que en windows, por ejemplo ruby.

Nos leemos en la próxima. Happy dev 👨‍💻