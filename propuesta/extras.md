# 2.2 EXTRAS

## 2.2.1.- Accesorios que vienen con el kit básico de mBot

Hay ciertos extras que vamos a añadir a nuestro mClon para ser compatible con el mBot comercial :

* **Sensor ultrasónico** evita obstáculos
* **LED RGB** dos a cada lado del sensor ultrasónico
* **Sensor sigue-líneas**. Dos para cada lado de la línea.
* **Sensor de luz**
* **Zumbador**

![](/assets/mBot-300x266.png)

_Fuente Makeblock_

## 2.2.2- Extras que no vienen con el kit básico mBot

### 2.2.2.1.- BRAZO

La propuesta de Catedu es añadir este extra que le da al mClon unas posibilidades muy creativas :

{% youtube %}https://www.youtube.com/watch?v=O53jw98uCAo{% endyoutube %}

### 2.2.2.2.- Matriz LED

mBot tiene una matriz de LEDs 8x16 que permite escribir o dibujar

![](/assets/matrizled.jpg)

_Fuente: Web de Makeblock.es_

Para mClon existe una matriz similar 8x8

![](/assets/matriz8x8_MAX7219.png)

Pero no es compatible con la instrucciónes de mBlock para la matriz:

![](/assets/instrucciones2.jpg)

En vez de estas, hay que instalar una librería MatrixLed y utilizar las instrucciones conrrespondientes. **Sólo compatible con la versión mBlock 3 ya en desuso**. Se explica este proceso en https://tecnoloxia.org/mclon/64leds/

Por esta razón **NO** está en la propuesta de Catedu.
