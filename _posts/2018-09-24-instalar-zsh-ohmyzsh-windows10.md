---
layout: post
image: /images/img-post/oh-my-zsh-windows10.webp
title: Cómo instalar zsh y oh my zsh en Windows 10.
description: "Cómo instalar zsh y oh my zsh en Windows Subsystem for Linux, también a cómo instalar temas y plugins en oh my zsh para que saques el mayor provecho de esta Shell."
date: 2018-09-24 10:00:00
tags: [desarrollo-web]
author: leninalbertop
---
En este post vamos a instalar **zsh** y **oh my zsh** en el **subsistema de windows para linux en windows 10**, pero para poder hacer esto primero debes tener habilitado el subsistema, así que si aun no lo haz hecho pásate por el siguiente link que dejare aquí abajito, el mismo te llevara al post en donde te explico como hacerlo.

***

**También te podría interesar**:

[**Habilitar Windows Subsystem for Linux en Windows 10**](/windows-subsystem-linux)

[**Cambiar idioma al Bash de Ubuntu en Windows 10**](/cambiar-idioma-bash-ubuntu-windows10)

***

## Que es zsh y oh my zsh.

**Zsh** es un intérprete de comando o shell para sistemas basados en Unix. **GNU/Linux** entre ellos, su creador **Paul Falstad** lanzó la primera versión de este shell en 1990 cuando era estudiante en la universidad de **Princeton**.

Zsh se diseñó para poder usarse interactivamente. Se le han incorporado muchas de las características principales de otras shells de Unix como, **bash**, **ksh**, o **tcsh** y además posee características propias originales.

>Las letras **zsh** no significan **z shell** como muchos suelen creer o incluso afirmar, zsh proceden del nombre del profesor de la universidad de Yale [**Zhong Shao**](http://flint.cs.yale.edu/shao/index.html){: target="_blank" rel="noopener noreferrer"} y profesor asistente en **Princeton** para cuando **Paul Falstad** tenía en mente este proyecto, y el pensó que zsh seria un excelente nombre para una shell.

Por su parte **oh my zsh** es uno de los tantos framework que existen allá afuera para manejar la configuración de zsh, es quizás el más conocidos.

Oh my zsh viene cargado con útiles funciones que le dan "superpoderes" a tu terminal, como por ejemplo plugin de resaltado de sintaxis y autocompletado entre otros, además de unos alucinantes temas que cambian por completo el aspecto del shell.

>Puedes ver una lista de frameworks para manejar la configuración de zsh [**Aquí**](https://github.com/unixorn/awesome-zsh-plugins#frameworks){: target="_blank" rel="noopener noreferrer"}.

## Instalando zsh y oh my zsh en windows 10.

Lo primero que necesitamos instalar es **GIT**, si ya lo tienes instalado puedes obviar este paso, solo recuerda que el git instalado en windows no es el mismo que se instala en la distro (Ubuntu, Debian, OpenSUSE etc..) que tengas corriendo en el subsistema de windows para linux.

**Para Debian/Ubuntu**

Todos estos pasos debes de hacerlo desde el bash de ubuntu o el de tu distro instalada. En este caso yo lo haré sobre ubuntu.

Para instalar la última versión estable lanzada con el sistema operativo.

{% highlight bash %}
$ sudo apt install git
{% endhighlight %}

Para instalar la última versión estable lanzada por git, y que esta se mantenga actualizada con el tiempo debemos añadir su repositorio o PPA.

{% highlight bash %}
$ sudo add-apt-repository ppa:git-core/ppa
$ sudo apt update
$ sudo apt install git
{% endhighlight %}

En el siguiente [**LINK**](https://git-scm.com/download/linux){: target="_blank" rel="noopener noreferrer"} tienes los comandos para instalar git en otras distribuciones linux.

Ahora toca instalar zsh, por fortuna esta shell está listada en los repositorios oficiales así que con una línea de comando la instalamos.

{% highlight bash %}
$ sudo apt install zsh
{% endhighlight %}

En el siguiente [**LINK**](https://github.com/robbyrussell/oh-my-zsh/wiki/Installing-ZSH#how-to-install-zsh-in-many-platforms){: target="_blank" rel="noopener noreferrer"} tienes los comandos para instalar zsh en otras distribuciones linux

Toca ahora instalar oh my zsh, para ello copia y pega el siguiente código en la terminal.

**Para instalar zsh via Curl**.

{% highlight bash %}
$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
{% endhighlight %}

**Para instalar zsh via wget**.

{% highlight bash %}
$ sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
{% endhighlight %}

Cualquiera de las dos instrucciones hacen los mismo, descargar e instalar oh my zsh. Lo que varían son los métodos **curl** y **wget** ambos permiten la descarga de contenido de servidores web.

![Oh my zsh instalado en windows 10](https://lh3.googleusercontent.com/YeVSpXaX7H_9xPlpB_RXrRuxXEKRev19WU51PM8HWvKeIlfn9gRTjnZ3yPad9bzZ-iGD_0th_G4t=s768 "Instalación correcta de oh my zsh en windows 10")

Ahora que ya tenemos tanto zsh y oh my zsh toca establecerlo como shell predeterminado, para ello en la terminal teclea la siguiente instrucción.

{% highlight bash %}
$ chsh -s $(which zsh)
{% endhighlight %}

Esto hará que zsh se ejecute al abrir la terminal, y si quieres regresar al shell predeterminado usa la siguiente instrucción.

{% highlight bash%}
$ chsh -s $(which bash)
{% endhighlight %}

**¡Oh my zsh, superpoderes para zsh!**

Ya te comente que oh my zsh es un framework que potencia a zsh con plugins y temas, así que vamos a ver como se instalan.

## Oh my zsh themes.

![Temas para oh my zsh](https://lh3.googleusercontent.com/p10zyN7aPEz_EES5MJsTfo8J4u2y0kqXbjGJDK15Im-ozBf5rCfi7lMXnpisSDfJi6vSSHCXFX36=s768 "temas oh my zsh")

Oh my zsh tiene un "centenar" de temas para todos los gustos y algunos requieren de pasos adicionales, por ejemplo: El tema **agnoster** requieren que se instalen fuentes powerline, estas fuentes están parcheadas para mostrar iconos, como se muestra en la imagen de arriba.

Yo usare como ejemplo el tema **rkj-repos** *que no requiere pasos adicionales*. En la terminal escribe la siguiente instrucción para abrir el archivo **zshrc**.

{% highlight bash %}
$ nano ~/.zshrc
{% endhighlight %}

![archivo de configuración zshrc](https://lh3.googleusercontent.com/Il_diZ6SMLLvLfJGRTjRrrFlp7p-MnKAflc_9SxtkY79XZ9lZVeCYaN-182xM5zs2jh9b5vbJX0N=s768 "Archivo zshrc")

Ubicate en la línea `ZSH_THEME=""` y entre las comillas debes escribir el nombre del tema que quieras usar, por defecto viene el tema **robbyrussell**.

Luego de establecido el tema debes presionar las teclas `Ctrl + O` y luego `Enter` para guardar, y `Ctrl + X` para salir, refresca el archivo de configuración con el siguiente comando `source ~/.zshrc` para que se aplique el tema.

![Rkj-repos tema para oh my zsh](https://lh3.googleusercontent.com/nv3N9y_gqUltj05-gwZfDXPttvSUiRrEfa6XOGmG54IVqJTMsHnCO4LJAgN6vQfJkSSE3DC-B2go=s768 "Tema rkj-repos oh my zsh")

Mi terminal con el tema **rkj-repos** 😉

**Recomendaciones**

- [Temas oficiales para oh my zsh](https://github.com/robbyrussell/oh-my-zsh/wiki/themes){: target="_blank" rel="noopener noreferrer"}
- [Temas externos para oh my zsh](https://github.com/robbyrussell/oh-my-zsh/wiki/External-themes){: target="_blank" rel="noopener noreferrer"}
- [Cómo instalar fuentes powerline en windows 10](https://medium.com/@slmeng/how-to-install-powerline-fonts-in-windows-b2eedecace58){: target="_blank" rel="noopener noreferrer"}
- [Nerd Fonts](https://nerdfonts.com/){: target="_blank" rel="noopener noreferrer"} fuente parcheada mucho más completa que las powerline, si vas a usar estas fuentes debes instalar los archivos .ttf con la variante _**Windows Compatible**_.

## Oh my zsh plugins.

Para instalar los plugins en oh my zsh basta con seguir las instrucciones de los mismo, en su mayoría solo consiste en clonar el repositorio mediante git y añadir el nombre del plugin a la configuración en el archivo **.zshrc**.

Actualmente estoy utilizando solo dos plugins muy buenos que son [**zsh autosuggestions**](https://github.com/zsh-users/zsh-autosuggestions){: target="_blank" rel="noopener noreferrer"} y [**zsh syntax highlighting**](https://github.com/zsh-users/zsh-syntax-highlighting){: target="_blank" rel="noopener noreferrer"} el primero suguiere comandos mientras se escribe, y el segundo resalta la sintaxis del shell zsh mientras se escribe.

### Instalando los plugins.

En la terminal copia el siguiente comando que clona el repositorio del plugin a la carpeta de plugins de oh my zsh.

### Zsh autosuggestions.

{% highlight bash %}
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
{% endhighlight %}

### Zsh syntax highlighting.

{% highlight bash %}
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting
{% endhighlight %}

![Plugins oh my zsh](https://lh3.googleusercontent.com/q8izzWmMYO7jlikhf5HxONFaiEeGalDwaCqEytQ254b6_C32mYYUPcRzpzoHtb-oJacgN7-h0qmE=s768 "Configuración de plugins en oh my zsh")

Para activar los plugins accede al archivo de configuración mediante el comando `nano ~/.zshrc`, navega hasta la línea `plugins=(git)` y añade el nombre del plugin tal como lo indican sus instrucciones, en este caso los nombres son `zsh-autosuggestions` y `zsh-syntax-highlighting`, y al igual que con los temas `Ctrl + O` y luego `Enter` para guardar los cambios, `Ctrl + X` para salir y `source ~/.zshrc` para actualizar el archivo de configuración. Listo ya tienes tus plugins instalados y activados.

>[**Repositorio de plugins para oh my zsh**](https://github.com/robbyrussell/oh-my-zsh/wiki/Plugins){: target="_blank" rel="noopener noreferrer"}

**Problemas de permisos con los plugins en oh my zsh.**

![Permisos en oh my zsh](https://lh3.googleusercontent.com/HuesPxJw4ePJP5IMRMdkLcomx2lpGyv6i0qkzU77Ozso-QD_ztJ1n_mSVZkdJBZIVyNnQDQu7pRo=s768 "Permisos oh my zsh")

Para resolver problemas de permisos tienes dos opciones.

1- Saltar la verificación de directorios inseguros, para ello abre el archivo de configuración `nano ~/.zshrc` y escribe lo siguiente `ZSH_DISABLE_COMPFIX="true"` arriba/antes de

{% highlight bash %}
export ZSH="/home/tu-usuario/.oh-my-zsh"
{% endhighlight %}

2- Dar los permisos correctos a la carpeta del plugin, desde mi humilde opinión sería lo mejor, así que a por ello.

{% highlight bash %}
sudo chmod -R 775 /home/tu-usuario/.oh-my-zsh/custom/plugins/carpeta-del-plugin
{% endhighlight %}

Hasta este punto ya tienes la **terminal de Windows Subsystem for Linux** potenciada y listo para "convertirte en un hacker", pero aun me queda una cosita que compartir contigo.

![Error ls, cd en Windows Subsystem for Linux](https://lh3.googleusercontent.com/DBanw2NoEvez4dUCxzyHLEG8kpC9PQJFMUdNXhFC7IrD3zUvDzhc28-jpQeHFxdxx9tkuXzpksy3=s768 "Error en ls, cd, windows subsystem for linux")

Si ya has trasteado con la terminal y te has movido por los directorios haciendo uso de **cd** y **ls** seguro habrás notado que ciertos directorios se muestran con un color de fondo horrible, para solucionarlo copia lo siguiente al final del archivo de configuración **.zshrc**

{% highlight bash %}
LS_COLORS="ow=01;36;40" && export LS_COLORS

zstyle ':completion:*' list-colors "${(@s.:.)LS_COLORS}"
autoload -Uz compinit
compinit
{% endhighlight %}

Y el resultado lo tienes en la siguiente imagen.

![ls, cd Windows Subsystem for Linux](https://lh3.googleusercontent.com/J93s_iJOcGcULAEdUIVv35sp3GrofNqPO4FxLl_CO65ZK1HIDPzf5tM7LjEZtAWW6HMih_u-xU5X=s768 "Colores corregidos en ls, cd Windows Subsystem for Linux")

Bien esto ha sido todo en este post, espero te haya sido de utilidad. Nos leemos en la próxima. Bye.