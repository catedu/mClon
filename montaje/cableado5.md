# 3.7 Cableado extras

## 3.7.1 Leds RGB

Tienes dos tipos

* APA 106-F5 de 5mm
* APA 106-F8 de 8mm

### 3.7.1.1 APA - F5 de 5mm

 Es lo más recomendable, estos leds RGB tienen esta configuración :

 ![](/assets/ledsRGB.jpg)

 _Fuente: https://mclon.org Maria L CC-BY-SA_

 ![](/assets/APA-106-F5.png)

 Fuente: Datasheet

 Con cables Dupond y con ayuda de regletas, podemos hacer la siguiente conexiones :

 - Los dos Vcc conectados y al Vcc de la placa 5V
 - Los dos GND conectados y al GND de la placa 0V
 - El Din de un led al pin 13 de la placa Arduino
 - El Dout de ese led al Din del otro led
 - El Din del otro led sin conectar

 ![](/assets/conexionesRGB.jpg)

 _Fuente: https://mclon.org Maria L CC-BY-SA_

 >**tip** Sujeta las conexiones de los cables Dupond y los leds RGB con cinta aislante para que no se desconecten.

 Y los colocas en el chasis en sus soportes :

 ![](/assets/chasisRGB.jpg)

 _Fuente: https://mclon.org Maria L CC-BY-SA_

 Conecta el cable rojo a 5V, el negro a GND y el amarillo al pin 13, y voila !!

 ![](/assets/RGB_neopixel6-768x576.jpg)

 _Fuente: https://mclon.org Maria L CC-BY-SA_

 ### 3.7.1.2 APA - F8 de 8mm

 En este caso, el led no cabe por el hueco, tienes que ponerlo por encima:

 ![](/assets/ledgordo.jpg)

 Y su configuración de pines **es diferente** al APA-106-F5 :

 ![](/assets/APA-106-F8.png)

 Luego la conexión es :

 - Los dos Vcc conectados y al Vcc de la placa 5V
 - Los dos GND conectados y al GND de la placa 0V
 - El Din de un led al pin 13 de la placa Arduino
 - El Dout de ese led al Din del otro led
 - El Din del otro led sin conectar

 ![](/assets/conexionRGB-F8.png)

  ![](/assets/conexionRGB-F8-REAL.png)

 ## 3.7.2 Brazo robot: Servomotor

 Coloca el servomotor en su soporte usando los tornillos que vienen en su bolsa:

 ![](/assets/servoSoporte1-768x576.jpg)

  _Fuente: https://mclon.org Maria L CC-BY-SA_

Normalmente los colores de los cables del servo tienen este significado :

![](/assets/servo_cables.jpg)

  _Fuente: https://mclon.org Maria L CC-BY-SA_

Lo uniremos con 3 cables Dupond Macho-Macho y lo fijaremos con cinta aislante :

![](/assets/servoCables.jpg)

  _Fuente: https://mclon.org Maria L CC-BY-SA_

Y conectaremos el cable amarillo Señal al pin D11 para poder usar la instrucción (si queremos que sea slot2 o banco2 ponerlo a D12):

![](/assets/instruccionservo.jpg)

finalmente colocamos el brazo, para ello tienes que identificar cual es el ángulo 90ª ejecutando la instrucción anterior, y una vez puesto el servo en esa posición, poner el brazo levantado con un ligero ángulo hacia delante, tal y como indica la figura :

![](/assets/brazo.jpg)

_Fuente: Adaptado de https://mclon.org Maria L CC-BY-SA_

>** info** Puedes poner un tornillo en para asegurarlo o no pornerlo para quitar el brazo y ponerlo con facilidad para que sea más cómodo el almacenaje del robot.
