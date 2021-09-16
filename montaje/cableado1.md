# 3.3 Cableado - esquema general

Este es la parte más dificil !!!

<iframe src="https://giphy.com/embed/3o7abrH8o4HMgEAV9e" width="480" height="241" frameBorder="0" class="giphy-embed" allowFullScreen></iframe><p><a href="https://giphy.com/gifs/starwars-3o7abrH8o4HMgEAV9e">via GIPHY</a></p>

Tenemos que conseguir unir los diferentes elementos con los pines del Robodyn:

* Los pines digitales D0,D1,D2,D3,D4,D5,D6,D7,D8,D9,D10,D11,D12,D13
* Los pines analógicos A0,A1,A2,A3,A4,A5,A6,A7
* Los pines de alimentación GND, VIN

Y tinen que ser estas conexiones y no otras para que sea compatible con mBlock y mBot [planos de mBot](https://tecnoloxia.org/mclon/mbot/) :

## 3.3.1.- Tabla de conexiones

| PIN | ELEMENTO |
|-----|---------|
| A0  |  |
| A1 |  |
| A1 |  |
| A2 |  |
| A3 | Pines Echo y Trg del sensor ultrasonidos |
| A4 |  |
| A5 |  |
| A6 | Al LDR |
| A7 | Pulsador |
| D1 |  |
| D2 |  |
| D3 |  |
| D4 | Pin BIN1 del driver B6612FNG y en pin 11 del 7404 |
| D5 | Pin PWMB del driver B6612FNG |
| D6 | Pin PWMA del driver B6612FNG  |
| D7 | Pin AIN1 del driver B6612FNG y en pin 13 del 7404 |
| D8 | Buzzer |
| D9 | Sensor izquierdo siguelineas |
| D10 | Sensor derecho siguelineas  |
| D11 | Al servo del brazo |
| D12 |  |
| D13 | Leds RGB |



## 3.3.2.- Esquema elementos básicos

![](/assets/Esquema_RobotDyn-1_corrixido.png)

_Fuente: https://mclon.org Maria L CC-BY-SA_

## 3.3.3 Esquema accesorios

Los dos leds RGB

![](/assets/LEDsRGB_conexion.png)

_Fuente: https://mclon.org Maria L      CC-BY-SA_

El servo del brazo:

![](/assets/Servo_conexion-300x274.png)

_Fuente: https://mclon.org Maria L      CC-BY-SA_

El LDR :

![](/assets/ldr-esquema.jpg)

_Fuente: Adaptado de https://mclon.org Maria L      CC-BY-SA_
