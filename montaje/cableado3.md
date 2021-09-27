# 3.5 Cableado sensores

## 3.5.1 Sensores de línea

Se conlocan en el soporte de la cabeza loca, van justos, incluso puede ser no necesario atornillarlos. Tiene 3 pines:

* Vcc al 5V del Arduino.
* GND al GND del Arduino.
* OUT del sensor derecho a D9 mirándolo a los ojos del ultrasonido.
* OUT del sensor izquierdo a D10 mirándolo a los ojos del ultrasonido.

![](/assets/Sensores_lina-1_corrixido.png)

_Fuente: https://mclon.org Maria L CC-BY-SA_

![](/assets/Sensores_lina_frit_corrixido.png)

_Fuente: https://mclon.org Maria L CC-BY-SA_

## 3.5.2 Sensor ultrasonidos

Los pines Trig y Echo del sensor **tienen que estar soldados** por lo que se conecta uno de los dos al A3

![](/assets/ultrason_frit.png)

_Fuente: https://mclon.org Maria L CC-BY-SA_

## 3.5.3 Sensor de luz LDR.

Para el sensor de luz, tenemos que hacer el siguiente esquema :

![](/assets/ldr-esquema.jpg)

_Fuente: Adaptado de https://mclon.org Maria L CC-BY-SA_

Luego tenemos que hacer los siguientes empalmes, conectados o mejor soldados y aislarlos con una cinta aislante:

1. La resistencia 10k a uno de los pines del LDR y al cable que tiene que ir al A6
1. Un cable Dupond al otro extremo de la R10k que irá a GND del Arduino.
1. Un cable Dupond al otro extremo del LDR que irá al 5V del Arduino.

![](/assets/conexionLDR.jpg)

_Fuente: Adaptado de https://mclon.org Maria L CC-BY-SA_

Nuestra propuesta es de sólo **un LDR** pero recuerda que en [2.2](https://catedu.github.io/mClon/propuesta/extras.html) vimos una opción de poner dos LDRs con interesantes propuestas y fácilmente realizable.

Por simplifiación, no se ha impreso en 3D ningún soporte especial LDR al chasis, pero en https://tecnoloxia.org/mclon/estrutura/impresion-3d/ lo tienes por si quieres imprimírtelo. Nosotros proponemos poner la resistencia en la parte debajo del chasis, pasar los cables hacia el escudo Protoboard por los numerosos agujeros que hay en el chasis, y pasar el LDR por el agujero de los cables del sensor siguelíneas :

![](/assets/conexionchasisLDR.jpg)
