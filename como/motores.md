# 1.2.- Motores

Los motores son de corriente contínua sin control de su posición, es deicr, sólo podemos controlar su sentido de giro y su potencia.

![](/assets/motor.jpg)

El control de los motores implicará poner en el escudo Protoboard dos circuitos integrados y su cableado correspondiente, vamos a verlo:

## 1.2.1.- Driver motor B6612FNG

Para realizar el control de los motores, tanto su potencia como su sentido de giro se va a utilizar el controlador **TB6612FNG**

![](/assets/driver_explicacion.png)

_Fuente: https://tecnoloxia.org/mclon/ Maria L      CC-BY-SA_

La potencia de los motores se controla por los pines PWMA y PWMB indicando un valor entre 0 y 255.

## 1.2.2.- Los giros, una complicación más: 7404

Los giros se controlan con los pines AIN, por ejemplo para el motor A :

| Giro motor    | AIN1   | AIN2 |
|---------------|--------|------|
| clockwise     | 0      | 1    |
| anticlockwise | 1      | 0    |

Para no gastar dos pines del Arduino para esta función, un truco consiste en gastar sólo uno, y el otro que sea el inverso de ese mismo. Ese truco es lo que utiliza mBot y si queremos compatibilidad mClon y mBot tenemos que hacerlo.

Pero esto implica tener que utilizar un **circuito impreso más**, el 7404 que tiene 4 inversores :

![](/assets/7404-2.png)

### 1.2.3.- Otra opción para los giros

Tal y como dice la página https://tecnoloxia.org/mclon/robotica/o-control-dos-motores/ también se puede utilizar dos transistores y resistencias, (de echo, mBot lo hace así) pero no lo utilizaremos, pues pensamos que es más cómodo el 7404.
