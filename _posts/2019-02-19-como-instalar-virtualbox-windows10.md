---
layout: post
image: /images/img-post/como-instalar-virtualbox-windows10.webp
title: Cómo instalar Virtualbox en Windows 10 - Guía paso a paso.
description: "Guía paso a paso donde aprenderás a instalar Virtualbox en Windows 10, configurar una máquina virtual e instalar Ubuntu en Virtualbox."
date: 2019-02-19 10:00:00
tags: [aplicaciones]
author: leninalbertop
---
Virtualbox es mi aplicación favorita para crear máquinas virtuales en Windows, incluso sobre otras soluciones para este fin como [**VMWare Workstation Player**](https://www.vmware.com/latam/products/workstation-player.html){: target="_blank" rel="noopener norreferer"} o **Hyper-V** la aplicación nativa de Windows para crear máquinas virtuales.

¿Por que prefiero Virtualbox sobre otras soluciones?, pues básicamente porque es la que mejor resultado me ha ofrecido, además del plus de que es totalmente gratuito y de código abierto (*Open Source*).

En este post te guiaré a **cómo descargar e instalar VirtualBox en Windows 10**, cómo configurar una máquina virtual y también a **cómo instalar Ubuntu en Virtualbox**. Comencemos.

***

**También te podría interesar**:

[**Habilitar Linux (WSL) en Windows**](/windows-subsystem-linux)

[**Instalar ZSH y Oh My ZSH en Windows**](/instalar-zsh-ohmyzsh-windows10)

[**Cambiar idioma al bash de Ubuntu en Windows**](cambiar-idioma-bash-ubuntu-windows10)

***

## ¿Qué es Virtualbox?.

Virtualbox es una aplicación que cuenta con todas las herramientas necesarias para crear máquinas virtuales e instalar en ella un sistema operativo aislado en tu computadora, estos sistemas operativos virtualizados son utilizados para realizar pruebas sin dañar el sistema operativo base o anfitrión, o simplemente para experimentar con un sistema operativo diferente al instalado en nuestra computadora.

Claro que, a grandes rasgos Virtualbox es mucho mas que eso y para las empresas supone una potente solución profesional que ayuda a mitigar errores en sus plataforma.

## 01 - Cómo descargar Virtualbox.

Para descargar Virtualbox iremos al siguiente [**Link**](https://www.virtualbox.org/wiki/Downloads){: target="_blank" rel="noopener norreferer"} que te llevara a su página oficial.

![Descargar Virtualbox Windows 10](https://lh3.googleusercontent.com/3cl8ig0d0j_NTub6mLRhAs09Kzb3mhEb-1qQSO2BKga_HM9PN4oQOsrz_8teATPGbUx-wDtL1qQc=s768 "Descargar Virtualbox Windows 10")

Una vez allí, haz click sobre **Windows host** y guarda el archivo de instalación en la ruta o directorio de tu preferencia.

## 02 - Instalar Virtualbox en Windows 10.

El proceso de instalación es muy sencillo y no varía en nada a los típicos next, next, next cuando instalamos una aplicación en Windows. Si ya eres todo un pro en instalar aplicaciones en Windows (*lo mas probable*) puedes saltarte esta parte.

Sitúa el archivo de instalación que descargaste en el paso anterior y ejecutalo, de inmediato comenzará el proceso de instalación y en esta primera ventana haz click sobre **Next**.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/kZIEuJiNmgktuTLRaVysWcv3ujwrnDZOEDb1gzmW_tdDApgAf7rq3DOouCRbug6oJ-kGKBwuq4r1=s768 "Instalar Virtualbox en Windows 10")

En la siguiente ventana verás la información de lo que se va instalar, la recomendación es dejar todo tal cual esta y hacer click sobre **Next**.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/xSrCdCu88dKi_6cO58vWq49NpvSw0VVg12S5TankHoODOCMcl1YoqCmheYS9h46f1l1hJsFjhs7R=s768 "Instalar Virtualbox en Windows 10")

Ahora te dirá que va a crear los accesos directos en el **menú de inicio**, **en el escritorio**, **en la barra de inicio rápido** y **registrará la asociación de archivos**. Puedes desmarcar las opciones de crear iconos que desees pero **no desmarques la última opción**.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/H2HP_ltzdA8pNKBtKSBMTp7pDQA4xStvmHDGlDlgxMwj073kbzDpi7FwmRN8yApSSCBFYaHdvgQ7=s768 "Instalar Virtualbox en Windows 10")

En la siguiente ventana te saldrá una "advertencia" que dirá que la *función de red restablecerá su conexión de red y lo desconectará temporalmente de la red*, esto es debido a que Virtualbox instalará una conexión de red que posteriormente usará el sistema operativo virtualizado. Así que puedes proceder a hacer click en **Yes**.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/QGsJzmUulOY7w8eqSKL4MryeWzKDPXwf1I2vMHNd4VPitgE7jtD1W0NV6YYNL-YBx9cRevUnr6Tz=s768 "Instalar Virtualbox en Windows 10")

En la siguiente ventana haz click en **Install** para proceder ahora si, con la instalación de Virtualbox en tu computadora.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/_7ISyG4GAs6v5wySR4Qmc9D5UGtzvo5X1GnFntwp3YWB9ZIMWKcwDQH13yujR76s4j3FnlDiUun-=s768 "Instalar Virtualbox en Windows 10")

A continuación te saldrá el progreso de instalación.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/aohrWV9-GVPzqr6yv6eSbaSJBwbW0QLcmFh9N9bucRrGfct8paSc0NF94G6P5Rq2xFfC1X9BioWK=s768 "Instalar Virtualbox en Windows 10")

En el proceso de instalación te saldrá una ventana donde te informa que se instalará un controlador de bus, este es necesario para que el sistema operativo virtualizado pueda conectarse por ejemplo con los puertos USB de tu computadora, por lo tanto debes hacer click en **Instalar**.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/bPTUJ4I6bV-NNxDHc72Z499EjVn-8n_v4LpskkDEGz9PtqoLwtfIiEZ_GB07vt38etBWK0OAtKIE=s768 "Instalar Virtualbox en Windows 10")

Por último te saldrá una ventana en donde te confirma que Virtualbox se instaló sin problemas en tu computadora, deja seleccionada la opción marcada para que se ejecute de inmediato Virtualbox y haz click en **Finish**.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/VoK1TZOEh8vjdppRtV0jmq3IdXBHp9uul-ix9I1_m728zzGc_vVzUMhxRs9kGOn1JQ6OtAP7_eYg=s768 "Instalar Virtualbox en Windows 10")

La siguiente imagen te muestra la interfaz de Virtualbox desde donde crearemos nuestra máquina virtual, pero antes toca instalar el **Extension Pack**. Así que sigamos adelante con esta guía paso a paso.

![Instalar Virtualbox en Windows 10](https://lh3.googleusercontent.com/gLiZuRNkzhz05iYV51OvkRDNkhziaijCMkm9EuFgbtYdwBJecDVotEFheSMugwKfTBJsu1kWQgeO=s768 "Instalar Virtualbox en Windows 10")

## 03 - Instalar Virtualbox Extension Pack.

El **Virtualbox Extension Pack** es un paquete que brinda mayor compatibilidad con USB 2.0 y 3.0, controladores de host, cámaras web, discos sólidos NVMe, encriptación de disco entre otros.

Accede al siguiente [**LINK**](https://www.virtualbox.org/wiki/Downloads){: target="_blank" rel="noopener norreferer"} para descargar el Virtualbox Extension Pack, haz click en **All supported platforms** como se muestra en la siguiente imagen y guarda el archivo en la ruta o directorio de tu preferencia.

![Descargar VirtualBox Extension Pack](https://lh3.googleusercontent.com/o7rUlPyONQyBUqeBNCL2CjEjaQ8WSykv5p4qa3SZeCC58NEMT-Ckb2k-gYZatzg6-Dr2An3ItOAr=s768 "Descargar VirtualBox Extension Pack")

Ubica el archivo descargado en el paso anterior, haz click derecho del ratón sobre él y elige la opción **Abrir con**.

![Descargar VirtualBox Extension Pack](https://lh3.googleusercontent.com/ZzDAd1ntB7jBjAI3YnyFNrvY1PeNDAHBhQLaJeffhV3oxZmi8dv6B3GdFLGNqvYS36HkJZnGmdcv=s768 "Descargar VirtualBox Extension Pack")

En la siguiente ventana asegurate que **Virtualbox Manager** esté seleccionado y haz click en **Aceptar**.

![Descargar VirtualBox Extension Pack](https://lh3.googleusercontent.com/hjgr1eXqr9_AZk1vZVIiI39W_4fpkw4goxcytREpTVMXxQ8qFZh3uPV_bZxRdDYVaIzsYoAdHrtt=s768 "Descargar VirtualBox Extension Pack")

Acepta el contrato de licencia para continuar.

![Descargar VirtualBox Extension Pack](https://lh3.googleusercontent.com/tNdSrrO2qp1HVlvtLW64tKp7725MPcdnaTACqbw8la1aUt3OWckKbfhrJ2mkneH45G6BJO1rjUxU=s768 "Descargar VirtualBox Extension Pack")

Ahora haz click en **Instalar** para comenzar con la instalación de los Virtualbox Extension Pack.

![Descargar VirtualBox Extension Pack](https://lh3.googleusercontent.com/ohG8GtIV8ERiwnIsnJwPS8C41d4GNlpJDHwxxHPnzCKEzRENxN46nwKRmFsxvYBLi9-k9ScQSGZV=s768 "Descargar VirtualBox Extension Pack")

Por último selecciona **Aceptar**. Listo ya tenemos los Virtualbox Extension Pack instalado.

![Descargar VirtualBox Extension Pack](https://lh3.googleusercontent.com/xYo78IKN-118SLU-RpTaPs_9o9PuLS8UfX1YSwfBO-49emC_Q7Om5L6jee4eb05ziZBcW0rFaFWV=s768 "Descargar VirtualBox Extension Pack")

## 04 - Configurar máquina virtual para instalar Ubuntu.

Nos toca ahora configurar Virtualbox para instalar Ubuntu en una máquina virtual, a por ello.

En Virtualbox selecciona el icono **Nueva** para crear nuestra máquina virtual.

![Configurar VirtualBox](https://lh3.googleusercontent.com/gLiZuRNkzhz05iYV51OvkRDNkhziaijCMkm9EuFgbtYdwBJecDVotEFheSMugwKfTBJsu1kWQgeO=s768 "Configurar VirtualBox")

Dale un nombre descriptivo a tu nueva máquina virtual, en la **Carpeta de máquina** puedes dejarlo tal cual o si lo prefieres puedes elegir otra ruta, como esta máquina la estamos configurando para instalar Ubuntu  en **Tipo** elige la opción de **Linux** y en **Versión** debes seleccionar los bit correspondiente a la distribución de Linux que vayas a utilizar.

Para esta guía paso a paso **instalaremos Ubuntu 18.04 LTS** por lo tanto elegiremos **Ubuntu (64-bit)** ya que esta versión de Ubuntu no tiene instalador de 32-bit.

Completa estos campos y haz click en **Next**

![Configurar VirtualBox](https://lh3.googleusercontent.com/H-9smo4v2i7po8oUxdWeLqZO1HsryKH0bZc7Ih9Y0r7NLMaa83nDxtVg-EvLp6EkNVXcPNyf2AKz=s768 "Configurar VirtualBox")

Ahora elegiremos cuanta memoria ram tendrá nuestra máquina virtual, para Ubuntu **se recomienda un mínimo de 2gb** y aquí hay que aclarar lo siguiente.

Si tu computadora tiene 2gb de ram o menos puedes dar por sentado que no podrás ejecutar una máquina virtual, porque simplemente tu computadora no tendrá la ram suficiente como para mantenerse estable.

Así que **recomiendo que como mínimo tu computadora cuente con al menos 6gb o más** de memoria ram para que esta sea compartida de la siguiente manera **2gb para la máquina virtual** y los **4 restante para tu sistema operativo anfitrión**.

Cuando ya tengas definido cuanta memoria ram le asignaras a tu máquina virtual haz click en **Next**

![Configurar VirtualBox](https://lh3.googleusercontent.com/WjmjjqguHRYIBmR8f4nhep38_R3Mbk2eWvXZe0OCxG_hIMLJyrhSQ07M_EVsowK7P60uA8nvSGL-=s768 "Configurar VirtualBox")

Toca ahora crear el disco duro en donde instalaremos Ubuntu, elige **Crear un disco duro virtual ahora** y haz click en **Crear**.

![enter image description here](https://lh3.googleusercontent.com/Zz_A7zX0AwwPOwNcJJtf1JhYMsYZPK18yUkXwBeqF_TtGNK5Dh38Qg_uSfyUqY1nu8hV80F9gE4j=s768 "Configurar VirtualBox")

Para el tipo de archivo de disco duro elige la opción **VDI (VirtualBox Disk Image)** y haz click en **Next**.

![Configurar VirtualBox](https://lh3.googleusercontent.com/nfhohguCRtQt9ifEib_fHNMl2Fjm1roDaZ9Ma85tk8qmEFnrWu1DoSdXfDs4DhpdEQulnU6e-PQV=s768 "Configurar VirtualBox")

Para el almacenamiento en unidad de disco duro física, este apartado se explica claramente por si solo, para esta guía utilizare la opción **Reservado dinámicamente**. Casi se me olvida haz click en **Next**. :-)

![enter image description here](https://lh3.googleusercontent.com/p8UnJf7JDR02HfjLUGkGAL9Ey35LffciWRK0D61mPMucHaQnSjvC_waZzLNavaxiL7tHC3zsZ9U3=s768 "Configurar VirtualBox")

A continuación le daremos un tamaño inicial a nuestro disco duro virtual, **para Ubuntu se recomiendan unos 25gb**, entonces eso es lo que debes establecer en este apartado. Como siempre haz click en **Crear** y se creará nuestra máquina virtual.

![Configurar VirtualBox](https://lh3.googleusercontent.com/E-dSgSSkqp4SEiiNaRVo1rg09AVwKT7QBBIR7cOMlSaurED6zun2kJyjI3IRLpt2T7DunOYhtV-D=s768 "Configurar VirtualBox")

Ya casi tenemos nuestra máquina virtual configurada para poder instalar Ubuntu, solo faltan un par de configuraciones más para poner todo a punto.

En la recién creada máquina virtual haz click en el icono **Configuración**.

![Configurar VirtualBox](https://lh3.googleusercontent.com/Df4p2x8JQNNP9Y6kl5tZWPtOTnUZCLjCdLGjk-dLsDNtH2wGyQvBz7_tjeDgbZv7YzIfQZastwBw=s768 "Configurar VirtualBox")

Sitúate en la opción **Sistema** y selecciona la pestaña **Procesador**, allí debes de establecer cuántos núcleos de tu procesador le asignará a la máquina virtual.

**Para Ubuntu se recomiendan 2 núcleos**, pero ten presente que si tu procesador es de solo 2 núcleos (Dual Core) debes dejar esta opción en 1 ya que si eliges en asignar los 2 núcleos de tu procesador tanto tu sistema operativo anfitrión como la máquina virtual irían a tropezones.

Mi recomendación es que tu procesador se de 4 núcleos (Quad Core) para que todo corra literalmente de manera fluida.

![Configurar VirtualBox](https://lh3.googleusercontent.com/URn-Bdd2freTT5IEgQP7ZRR62UnrpLAN1-ZseIrHyRzU1F660uFRXzLV4ZOWLwUnkF8e1HsVHxN9=s768 "Configurar VirtualBox")

Ahora toca cargar la imagen iso de Ubuntu para su booteo, si aun no la has descargado ve al siguiente [**Link**](https://www.ubuntu.com/download/desktop){: target="_blank" rel="noopener norreferer"} y descargalo.

Ya con la imagen iso de Ubuntu en nuestra computadora y desde la configuración de nuestra máquina virtual sitúate en la opción **Almacenamiento** selecciona el disco **Vacío** y a tu derecha haz click sobre el **icono alegórico de CD** y haz click en **Seleccione archivo de disco óptico virtual...** y navega hasta el directorio o carpeta en donde tengas guardado la imagen iso de Ubuntu.

![Configurar VirtualBox](https://lh3.googleusercontent.com/RLiht3IIU1vEUJ2l69benl9BUIogHK4rWM7TCWVrZie8GjBV85XyZOj4gWjqPjJapXDicTZpERYL=s768 "https://www.ubuntu.com/download/desktop")

Cuando ya tengas la imagen iso cargada en la configuración haz click en **Aceptar** para proceder con el booteo e instalación de Ubuntu.

![Configurar VirtualBox](https://lh3.googleusercontent.com/qTFqhdnduLMmipJAGr6TkEuoiHSgt87mC3x3d3NkBm4Yv-ixxYhF3CrXu3rbYhxSOp7iBjgZY822=s768 "Configurar VirtualBox")

## 05 - Instalar Ubuntu en Virtualbox.

Haz click en el icono **Iniciar** para arrancar la máquina virtual.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/Df4p2x8JQNNP9Y6kl5tZWPtOTnUZCLjCdLGjk-dLsDNtH2wGyQvBz7_tjeDgbZv7YzIfQZastwBw=s768 "Instalar Ubuntu en Virtualbox")

En lo que la máquina virtual encienda nos saltara la primera ventana de instalación de Ubuntu en la que debes elegir el idioma de instalación, en este caso **Español** y haz click en **Instalar Ubuntu**.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/F0yjHssTCprKKIQ6C4SlZ6N1dJ7NXJwJ2Tv_wPNtqhyozl4hPNcn92wGltUHW479cjfWVqeWk1uI=s768 "Instalar Ubuntu en Virtualbox")

Luego debes elegir si quieres una **Instalación normal** o **Instalación mínima**,  y también si deseas **Descargar actualizaciones al instalar Ubuntu** e **instalar programas de terceros para hardware de gráficos y de wifi y formatos multimedia adicionales**.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/xWR3K9V9iYLXr2GrfztdZ8Qsf2Yg1Gb_fkaHrNL_ozMEYY3txSYbRKj6QrlT25RgspaTZA46i23K=s768 "Instalar Ubuntu en Virtualbox")

Toca ahora elegir el tipo de instalación, para esta guía elegiremos **Borrar disco e instalar Ubuntu**.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/z7ATHPidgcG4KK7sXXYi8ynUCGVyj1jQ61Iu8O3nCCyxlh7PWbE-hV8n0LEMYoDI5_2q4hSuJfaN=s768 "Instalar Ubuntu en Virtualbox")

Al hacer click en **Instalar ahora** saldrá una ventana de confirmación con los cambios que se harán en el disco duro virtual.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/fklyBVzrxWTY-h83Qio7TYqqAY9OqKWZSwlRVZkbWbYg7hXChbjznDeBUYf4ov8zXGYRd7EQpEQt=s768 "Instalar Ubuntu en Virtualbox")

Selecciona la región donde te encuentres, esto también establecerá la zona horaria.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/RH5h8RPk01mNGbkPxXyFhKppCEjdtX-oSoSxhgxnGYqUKYgz-qIpHhY73lEsoQ2EOwWJhn4JyhXh=s768 "Instalar Ubuntu en Virtualbox")

Elige la distribución de teclado.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/nruzY-ClQb7tRLBiDDTY2fCkD8Iio4Xab6VxaBhUHA2OSscxn96Cy_babQf5kXJ2oaSDjmhCq9SI=s768 "Instalar Ubuntu en Virtualbox")

Por último establece el nombre de usuario y la contraseña que utilizarás para acceder al sistema.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/RpkppX3RHtCWX_OFLSi5quVqvDIduXahcdt8Rmm2u32ZmJCksw5xiXzrL89n_mpGnkCn4QvONIQY=s768 "Instalar Ubuntu en Virtualbox")

Ahora debes esperar que termine el proceso de instalación.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/W3YAVSyafjp8zip1zR3GVKeBYPFXItba4A3bm31EJxq1a2I441_U2wpmmH8RZUwgYpsaIG3SGoAV=s768 "Instalar Ubuntu en Virtualbox")

Cuando finalice el proceso de instalación te pedirá que reinicies el sistema.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/X0hWAnxn1jQZ6Y8V1ClMOn4z1-9eUXoiPwY2lhdBuayG_wy53ke0YwWI4BO3Pgnil9PVDJjGAsE0=s768 "Instalar Ubuntu en Virtualbox")

Luego del reinicio toca iniciar sesión con los datos establecidos en el proceso de instalación.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/C1w9xVJJbUDUC6WmtKQjH6PIbxyB2xgTObCVzpthQlWUxpQo8Hz3zpPTtLS0RQVWPJvHYwVX-0Az=s768 "Instalar Ubuntu en Virtualbox")

Y vualá, ya tenemos Ubuntu instalado en Virtualbox listo para realizar lo que se nos antoje xd.

![Instalar Ubuntu en Virtualbox](https://lh3.googleusercontent.com/RqyWmvBOF5t_p4E1KTolk9yYpe4tWGB_qPllvp5nrLwHEpLZ2xjNilWVqA3PA54qbyJARKGDkonU=s768 "Instalar Ubuntu en Virtualbox")

## 06 - Instalar Virtualbox Guest Additions.

Entramos en la última parte de esta guía en donde hemos visto hasta ahora como descargar he instalar Virtualbox en Windows 10, como configurar virtualbox y como instalar Ubuntu en Virtualbox.

Solo nos queda instalar los **Virtualbox Guest Addition** en Ubuntu, esto nos permitirá copiar archivos entre sistema anfitrión/huésped y viceversa, mejora la integración con el mouse, mejora el soporte para video, crear carpetas compartidas etc...

Iniciada la máquina virtual con Ubuntu lo primero que debes hacer es abrir la terminal y copiar la siguiente instrucción para buscar alguna actualización de paquetes y actualizarlos de una vez .

```bash
sudo apt update && sudo apt upgrade
```

Luego hay que instalar lo siguiente.

```bash
sudo apt-get install build-essential gcc make perl dkms
```

Y por último reinicia el sistema con el siguiente comando.

```bash
reboot
```

Luego del reinicio haz click en ** Dispositivo** y luego en **Insertar imagen de CD de las Guest Additions...**

![Instalar Virtualbox Guest Additions](https://lh3.googleusercontent.com/cJZ6XGAxZn6TMO_ouNHsW7N0J26EGYUy48Iuc_plwakYAWH8uXk_2OI1h4H1jCBXfPkZ23dthMS-=s768 "Instalar Virtualbox Guest Additions")

Confirma la instalación de las Guest Additions haciendo click en **Ejecutar**.

![Instalar Virtualbox Guest Additions](https://lh3.googleusercontent.com/hmfLkkC8Ilwfv-raw8eFFKtcGoJZnZsWMHchxL8RRLDFAsUtgX9aANDlQ5JzgqbQXNq5-rWuLQog=s768 "Instalar Virtualbox Guest Additions")

A continuación se te pedirá tu contraseña de usuario y se abrirá una terminal desde donde se mostrará el proceso de instalación de las Guest Additions. Una vez terminado el proceso de instalación presiona **Enter** en tu teclado para finalizar.

![Instalar Virtualbox Guest Additions](https://lh3.googleusercontent.com/J6Pxdjod-QlRW4485-w93jxndLLK-s00_j_96Y3ugzEABlLRvMBrsFnfn-PZGzMrdxeiEbcDLy1j=s768 "Instalar Virtualbox Guest Additions")

Ahora debes apagar el sistema operativo huésped (Ubuntu) para poder habilitar el **drag and drop** o arrastrar y soltar entre máquinas y el **Clipboard** o portapapeles.

Para ello haz click en el icono de **Configuración** de la máquina virtual, sitúate en la opción **General** y selecciona la pestaña **Avanzado** y en las opciones **Compartir portapapeles** y **Arrastrar y soltar** elige **Bidireccional** y haz click en **Aceptar**.

![Instalar Virtualbox Guest Additions](https://lh3.googleusercontent.com/NVeGjCpxWEfafWkrRsIE8CP0D12OWDqJ2yWHNEGArc-P_JH4HgCtyfj9srawlUQgmydcP7iRwKmN=s768 "Instalar Virtualbox Guest Additions")

¡Felicidades! Ya tienes una máquina virtual con Ubuntu corriendo al 100%.

¿Qué te ha parecido esta guía paso a paso? en donde hemos aprendido a descargar e instalar Virtualbox en Windows 10, cómo configurar una máquina virtual para instalar Ubuntu, y como instalar los Guest Additions para una mejor gestión e integración entre anfitrión y huésped.

Si te consigues con algún error al seguir esta guía no dudes en usar la sección de comentarios para tratar de ayudarte a dilucidarlo.

Hasta la próxima.