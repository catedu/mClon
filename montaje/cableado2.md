# 3.4 Cableado - Motores

Tenemos el Robodyn, el escudo Protoboard, cables, el driver motor B6612FNG, el 7404 y una R10k

![](/assets/pezas3-914x1024.jpg)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

Recuerda que la placa protoboard, los agujeros están conectados verticalmente a ambos lados, es decir lo rojo está conectado:

![](/assets/protoshield2-204x300.png)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

En https://tecnoloxia.org/mclon/electronica/protoshield/ tienes unos consejos para realizar correctamente las conexiones.

## 3.4.1 Driver motor B6612FNG y 7404

Vamos a conectar este esquema

![](/assets/ProtoShield_1_esq_corrixido.png)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

Conecta los chips **dejando dos columnas libres** tal y como indica la figura, y conectamos Vcc y GND en la columna libre de la izquierda:

![](/assets/Protoshield1-300x255.png)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

Ponemos las conexiones de alimentación de los dos chips

![](/assets/alimentdrivermotor.jpg)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

Y ahora conectamos los pines de velocidad y dirección:

![](/assets/ProtoShield_3_esq1-e1535918627421.png)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

Es decir, estos cables

>**info** ATENCIÓN, no se han dibujado las conexiones anteriores, para simplificar los dibujos, es decir ,**no** quites los cables anteriores

Primero el motor A

![](/assets/ProtoShield_3_frit1.png)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

Y luego el motor B

![](/assets/ProtoShield_3_frit2.png)

_Fuente: https://tecnoloxia.org/mclon Maria L CC-BY-SA_

Ahora conectamos los motors **OJO CON LA POLARIDAD** si te equivocas, el motor girará al revés :

![](/assets/conexionmotor.jpg)

Al alimentar mClon con PowerBank, la tensión de la pila le llega diréctamente al Arduino Robodyn, luego alimentamos Vm con los 5V del Arduino ( Vcc ya estaba a 5V )

![](/assets/powerbank_esquema-fixed.png)

Luego las conexiones quedan así :

![](/assets/finaldriver.jpg)
