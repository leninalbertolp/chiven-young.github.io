---
layout: post
image: /images/img-post/cambiar-idioma-bash-ubuntu-windows10.webp
title: Cómo cambiar el idioma al Bash de Ubuntu en Windows 10.
description: "Aprende de manera práctica a cómo cambiar el idioma del Bash de Ubuntu en el Subsistema de Windows para Linux en Windows 10."
date: 2018-09-25 10:00:00
tags: [desarrollo-web]
author: leninalbertop
---
En este post veremos **cómo cambiar el idioma de inglés a español al bash de ubuntu 18.04 LTS** en el subsistema de windows para linux (wsl), esto es ideal por si no entendemos a la perfección el idioma inglés que es con el que viene por defecto.

Al hacerlo tendremos la ventaja ante cualquier error que se presente en el sistema, ya que podremos leerlo en nuestro idioma natal, obteniendo con ello una interpretación correcta de dicho evento.

## Antes de continuar.
>En post anteriores hemos visto [**cómo habilitar el subsistema de windows para linux**](/windows-subsystem-linux), también a [**cómo instalar zsh y oh my zsh**](/instalar-zsh-ohmyzsh-windows10) personalizarlo con temas e instalar plugins para extender el potencial de esta shell.

![Configurar idioma español al bash de ubuntu en windows 10](https://lh3.googleusercontent.com/Qyey5aDhdojvuYsha-1XzTlzEKopdZpSRB-xhdP5LAx0l7BFD-b702ftGXQ-9nfF9fMId3QRhX08=s768 "Cambiar el idioma al español al bash de ubuntu en windows 10")

Lo primero que tenemos que hacer es descargar los paquetes de idioma en español, para ello ejecuta el siguiente comando en la terminal o bash de ubuntu.

{% highlight bash %}
$ sudo apt install language-pack-es
{% endhighlight %}

Luego de descargado los paquetes toca configurar el idioma de la interfaz, así que en el terminal ejecuta este otro comando.

{% highlight bash %}
$ sudo dpkg-reconfigure locales
{% endhighlight %}

![enter image description here](https://lh3.googleusercontent.com/79AVl_ouP4FJ9rQkYD8kTMsi0rjhTTaW40eqk_fDFlKzpjy0rbBG3pE9uSvi5p8RfPWSv5wKvp2b=s768 "Configuración de idioma en el bash de ubuntu 18.04 en windows 10")

Acto siguiente se nos abrirá la interfaz de configuración local, en la que debes seleccionar el idioma según tu país y con juego de caracteres **UTF-8**, en mi caso `es_VE` por **Venezuela**.

Para moverte entre las opciones utiliza las teclas de flechas, para elegir una opción usa la tecla `Enter`, para saltar a las opciones `<Ok>` y `<Cancel>` usa la tecla `Tabulador`.

![Seleccionar idioma en el bash e ubuntu en windows 10](https://lh3.googleusercontent.com/JmMQw2tNu1WP-QVG-n4gKUiBUeQ6ZrOmq5_Y3-km4HxC664qGzNTH1ITvu6rW9jb5k5Ld4iuH2Ax=s768 "Seleccionar idioma español en el bash de ubuntu en windows 10")

En la siguiente ventana y como último paso elige el idioma `es_` con la terminación local acorde a tu país.

![Cambiar idioma desde terminal a ubuntu 18.04](https://lh3.googleusercontent.com/Wc5N7P5HR-6jVmTQYj_assDy4Ff793beGuFoETfZFzJhpwUvGAqjOMsIJ8fNUUftKIYEf1C5JR2z=s768 "Cambiar idioma a ubuntu desde el terminal")

Ahora ya tienes tu bash de ubuntu en tu idioma natal y hasta aquí nos ha traído este post, esperando como siempre que haya sido de tu utilidad.

Nos leemos en la próxima.