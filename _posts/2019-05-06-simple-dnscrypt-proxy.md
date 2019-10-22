---
layout: post
image: /images/img-post/simple-dnscrypt-proxy.webp
title: Encripta tus consultas DNS con Simple DNSCrypt para Windows
description: "Simple DNSCrypt es un programa amigable gratuito y Open Source que te permite configurar DNSCrypt Proxy en Windows para cifrar las consultas DNS y evitar riesgos de ataques de DNS Spoofing o Envenenamiento de la Caché de DNS."
date: 2019-05-06 20:20:00
tags: [internet]
author: leninalbertop
---
Simple DNSCrypt es un programa con una interfaz amigable para administrar la configuración de dnscrypt proxy en sistemas operativos Windows.

[**Dnscrypt proxy**](https://github.com/jedisct1/dnscrypt-proxy){: target="_blank" rel="noopener norreferer"} es un proxy dns flexible con soporte para protocolos de encriptación modernos como [**DNS sobre HTTPS**](https://es.wikipedia.org/wiki/DNS_mediante_HTTPS){: target="_blank" rel="noopener norreferer"} y [**dnscrypt**](https://dnscrypt.info/protocol/){: target="_blank" rel="noopener norreferer"} estos protocolos se encargan de cifrar las consultas dns que se llevan a cabo en nuestras computadora cuando por medio de un navegador web accedemos a una página web, protegiendo que dichas consultas dns sea alteradas por un tercero como nuestro ISP *proveedor de servicio de internet* o delincuentes informáticos.

## ¿Por qué debes cifrar tus consultas DNS?

La pregunta se responde por si sola **SEGURIDAD** ya que una consulta dns no cifrada es blanco para los delincuentes informáticos que aprovechando esta brecha llevan a cabo ataques de [**DNS Spoofing**](https://en.wikipedia.org/wiki/DNS_spoofing){: target="_blank" rel="noopener norreferer"} o [**Envenenamiento de la Caché de DNS**](https://es.wikipedia.org/wiki/Envenenamiento_de_DNS){: target="_blank" rel="noopener norreferer"} un método que modifica la consulta dns original para por ejemplo redirigir dicha consulta a otro sitio de aspecto similar para obtener los datos de la víctima, a este otro ataque se le conoce como [**Man in the Middle**](https://es.wikipedia.org/wiki/Ataque_de_intermediario){: target="_blank" rel="noopener norreferer"} o hombre en el medio en español.

Recientemente en Venezuela se llevó a cabo un ataque de DNS Spoofing por parte de CANTV/Movilnet la principal proveedora de servicio de internet del país en mano del régimen actual.

Este evento fue documentado por [**VE SIN FILTRO**](https://vesinfiltro.com/){: target="_blank" rel="noopener norreferer"} y publicado en documento ejecutivo que puedes leer en [**Español**](https://vesinfiltro.com/noticias/Phishing_impulsado_por_gobierno_de_Venezuela/){: target="_blank" rel="noopener norreferer"} e [**Inglés**](https://vesinfiltro.com/noticias/Phishing_by_Venezuelan_government_targets_activists/){: target="_blank" rel="noopener norreferer"}.

## Configurar DNSCrypt-Proxy en Windows con Simple DNSCrypt.

LLevar el proceso de configuración de dnscrypt proxy tal cual se explica en su documentación oficial le pondría los pelos de punta a un usuario común y corriente debido a la exigencia técnica que este requiere y es ahí donde entra en juego Simple DNSCrypt.

Con Simple DNSCrypt nos podemos olvidar del tecnicismo y centrarnos en una interfaz visual amigable para dnscrypt proxy.

Simple DNSCrypt es un programa gratuito y open source (*código abierto*) para windows que con unos simples pasos nos permite cifrar nuestras consultas dns.

Lo primero que hay que hacer es descargar Simple DNSCrypt desde su [**Página Oficial**](https://simplednscrypt.org/){: target="_blank" rel="noopener norreferer"} donde tienes instaladores para versiones de windows de 64 bits y 32 bits así que elige la versión adecuada.

![Descargar Simple DNSCrypt Windows](https://lh3.googleusercontent.com/xTIudnlye9jPDlYxAvilYuwVKhw6xXPoCrDA2LNelb4uYYcjOHV5XZFnXBgkwQuX6C0hwquuytTP=s768 "Descargar Simple DNSCrypt Windows")

Si ya has instalado programas en windows entonces no tendrás dificultad alguna para instalar Simple DNSCrypt en tu computadora, el proceso es similar al de cualquier otro con los característicos siguiente, siguiente, siguiente o next, next, next.

Al iniciar el programa te encontrarás con una interfaz de navegación por pestañas desde donde podrás gestionar las configuraciones.

![Iniciar Simple DNSCrypt en Windows](https://lh3.googleusercontent.com/aEUStvubi95vKF6PQxZQW2GViHJ8lVUGp0BHTz5TQPzBR6wXpgconLJ1kSnqwIx2ndKEgaJQokVF=s768 "Iniciar Simple DNSCrypt en Windows")

En la pestaña de **menú principal** basta con dejar seleccionas las opciones del apartado de **configuración** tal cual están que en resumen sería.

* IPv4: Protocolo de interconexión de internet.
* DNSSEC: Extensiones de seguridad del sistema de nombres de dominio.
* Sin registro de actividad: Servidores dns que no guarden registro de las consultas dns, es decir las páginas web que visitas.
* Sin filtros: Servidores que no apliquen filtros arbitrarios ejemplo: bloqueadores de anuncios como es el caso de los dns de Adguard.
* DNSCrypt: Solo servidores dns con este protocolo de cifrado.
* DNS sobre HTTPS: Solo servidores dns con este protocolo de cifrado.

En el apartado **servicio** clickea sobre el switch para instalar el servicio que pone en marcha la encriptación.

Y en **tarjeta de red** debes seleccionar la tarjeta de red que transmite la conexión a internet.

Con esta simple configuración bastaría para estar protegido, pero si quieres ir un poco más allá y seleccionar por ejemplo un servidor dns en específico como es mi caso entonces ve a la pestaña **resolutores** para hacerlo.

![Resolutores Simple DNSCrypt](https://lh3.googleusercontent.com/kE8X7DPt_gTNZnq1v-mLd-IBoVADLGgMQ-vtfFskzorerSjSOQDF2aZ0DGTSqS1V-k9YRpyC4d9j=s768 "Resolutores Simple DNSCrypt")

En la configuración por defecto viene habilitada la opción de **modo automático** donde el programa seleccionará el servidor dns más rápido automáticamente según su criterio.

Yo elegí los [**dns de cloudflare**](https://1.1.1.1/es/){: target="_blank" rel="noopener norreferer"} por las bondades que brinda, si tu quieres elegir ese mismo o cualquier otro o varios si así lo deseas basta con clickear sobre el servidor dns y hacer click sobre aplicar ajustes.

También tienes otras opciones interesantes por si quieres aventurarte aún más allá. Por ejemplo en **ajustes avanzados** puedes configurar tu computadora como un resolutor dns global y actúe como puerta de enlace para tus otros equipos como smartphone o laptop.

Y en el apartado de **lista negra de dominios** puedes bloquear dominios o páginas web a los que no quieras que se accedan desde tu computadora por ejemplo bloquear páginas web con contenido para adultos para que los más pequeños de la casa no tengan acceso a ellas.

Opciones interesantes que hasta ahora no me he visto en la necesidad de utilizar por lo que corre de cuenta aventurarte en ellas.

En el caso que ya no quieres utilizar Simple DNSCrypt (*no veo el por que*) su desinstalación es aún más fácil, para ello ve a Panel de Control, luego a Programas y características y busca Simple DNSCrypt y lo demás es cuento.

¿**Qué tal te a parecido este post**? ¿**Ya conocías Simple DNSCrypt y lo importante que es encriptar tus consultas dns**?