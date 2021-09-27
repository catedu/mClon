# 2.2 SENSORES, ACCESORIOS Y EXTRAS de mClon versus mBot

## 2.2.1.- Que vienen con el kit básico de mBot

Hay ciertos acceorios y extras que vamos a añadir a nuestro mClon para ser compatible con el mBot comercial :

* **Sensor ultrasónico** evita obstáculos
* **LED RGB** dos a cada lado del sensor ultrasónico
* **Sensor sigue-líneas**. Dos para cada lado de la línea.
* **Sensor de luz**
* **Zumbador**

![](/assets/mBot-300x266.png)

_Fuente Makeblock_

## 2.2.2- Que no vienen con el kit básico mBot

### 2.2.2.1.- BRAZO

Con mBlock existe la posibilidad de añadir un servo

![](/assets/brazombot.jpg)

La propuesta de Catedu es también añadir este extra que le da al mClon unas posibilidades muy creativas :

{% youtube %}https://www.youtube.com/watch?v=O53jw98uCAo{% endyoutube %}

<hr />

# Otras propuestas no contempladas en el paquete de CATEDU

<hr />

## Matriz LED

mBot tiene una matriz de LEDs 8x16 que permite escribir o dibujar

![](/assets/matrizled.jpg)

_Fuente: Web de Makeblock.es_

Para mClon existe una matriz similar 8x8

![](/assets/matriz8x8_MAX7219.png)

Pero no es compatible con la instrucciónes de mBlock para la matriz:

![](/assets/instrucciones2.jpg)

En vez de estas, hay que instalar una librería MatrixLed y utilizar las instrucciones conrrespondientes. **Sólo compatible con la versión mBlock 3 ya en desuso**. Se explica este proceso en https://tecnoloxia.org/mclon/64leds/

Por esta razón **NO** está en la propuesta de Catedu.

## Dos LDRs

Nuetra propuesta, por simplificar el robot, tiene **un LDR** conectado al A6 que sería el **sensor de luz abordo** pero fácilmente se pueden poner dos LDRs uno al A3 y otro al A1 que serían los equivalentes al **sensor de luz Puerto3** y el **sensor de luz puerto4**

![](/assets/pinsLDR.png)

_Fuente: https://mclon.org Maria L CC-BY-SA_

>**info** En total se pueden poner **hasta 3 LDRs**.

En la web https://tecnoloxia.org/mclon/estrutura/impresion-3d/ se pueden imprimir unos soportes especiales :

![](/assets/CaraArriba-768x298.jpg)

_Fuente: https://mclon.org Maria L CC-BY-SA_



Para más info ver https://tecnoloxia.org/mclon/accesorios/sensor-de-luz/


Con dos LDRs se pueden hacer cosas interesantes :

<blockquote class="twitter-tweet"><p lang="es" dir="ltr">O segue luz non e moi espectacular, pero ten dous ....<br>LDR <a href="https://t.co/wNyDp1O5Hp">pic.twitter.com/wNyDp1O5Hp</a></p>&mdash; mClon (@mClonRobot) <a href="https://twitter.com/mClonRobot/status/1061278328936693760?ref_src=twsrc%5Etfw">November 10, 2018</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>


## Un spoiler con cronómetro

Se trata de una pantalla de cuatro dígitos que puede usarse como cronómetro, contador de eventos, etc..

![](/assets/mClon_cabezallo14.jpg)

 _Fuente: https://mclon.org Maria L CC-BY-SA_

Para ver cómo se conectaría hay que consultar https://tecnoloxia.org/mclon/accesorios/aleron-cronometro/

## Fuera de camino

Esta opción esta documentado también en la Web https://tecnoloxia.org/mclon/accesorios/todoterreo/

<blockquote class="twitter-tweet"><p lang="pt" dir="ltr">Xa falta pouco para que o modelo todoterreo estea documentado na web. Mentres tanto podedes ver como funciona cos dous modelos de oruga, flexible e PLA. <a href="https://t.co/svclPqMJYo">pic.twitter.com/svclPqMJYo</a></p>&mdash; mClon (@mClonRobot) <a href="https://twitter.com/mClonRobot/status/1252503943797780480?ref_src=twsrc%5Etfw">April 21, 2020</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>

## Resuelve laberintos

Consiste en cambiar la posición de un siguelíneas para detectar las paredes de enfrente y el sensor ultrasonidos para seguir la pared derecha, en https://tecnoloxia.org/mclon/accesorios/resolve-labirintos/ explica muy bien esta opción y las piezas 3d extras para hacerlo:

<blockquote class="twitter-tweet"><p lang="pt" dir="ltr">Xa resolvo laberintos! Pero, que sexan sinxelos.<br>Agora documentar e que a xente me replique <a href="https://t.co/QrWEvWiHqs">pic.twitter.com/QrWEvWiHqs</a></p>&mdash; mClon (@mClonRobot) <a href="https://twitter.com/mClonRobot/status/1063408748759257088?ref_src=twsrc%5Etfw">November 16, 2018</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
