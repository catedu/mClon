# 4.5 Testeo completo con mBlock

Para superar el curso, tienes que entregar un vídeo donde se demuestre que funcionan todos los elementos :

* Motores
* Sensores
  * Sensor ultrasónico
  * Sensores sigue-líneas
  * Sensor luz
* Accesorios
  * Botón
  * Buzzer
* Extras
  * Leds RGB
  * Brazo

## 4.5.1 Propuesta TEST-CATEDU

Puedes hacer tú mismo un programa, una propuesta **que englobe los 8 elementos expuestos**, o si quieres, te proponemos esta propuesta que te la puedes descargar aquí [TEST-CATEDU.sb2](https://drive.google.com/drive/folders/1D8vIUNfCDCvM_04RG5HMXtUEGcaBmnTI?usp=sharing)

La plantilla del circuito la podeis descargar [aquí imprimiento 4 hojas del fichero Word](https://drive.google.com/drive/folders/1D8vIUNfCDCvM_04RG5HMXtUEGcaBmnTI?usp=sharing) pero puede ser otra cualquiera.

{% youtube %}https://www.youtube.com/watch?v=6lOyVTUxPSo{% endyoutube %}

Tiene varios bloques definidos, este bloque **SIGUE LINEA** cumple la función de seguir la línea negra, pero si detecta un 3, llama al bloque **Buscalinea** pues está fuera del circuito:

![](/assets/mblock1.png)

El bloque **BuscaLinea** elige un número al azar y el 80% de veces retrocede a buscarlo, el otro 20% busca girando. Esto se hace así porque algunas veces se queda "atascado" hacia delante y hacia atrás, ese 20% es para romper ese ciclo vicioso.

![](/assets/mblock2.png)

La función **VERLATA** mira si hay una lata delante, y en ese caso la retira :

![](/assets/mblock3.png)

Para probar el sensor de luces, hemos pensado [en esta idea](https://www.youtube.com/watch?v=p9543Fjx4sM) :

La función **Para-si-oscuridad** se detiene en el caso de que se apaguen las luces y reproduce un juego de luces con RGB y sonidos con el Buzzer:

![](/assets/mblock11.png)

Donde el bloque **LUCES** enciende los RGB al azar

![](/assets/mblock12.png)

Finalmente el programa principal que llama a todos los bloques es

![](/assets/mblock15.png)

Donde tenemos que definir:

* La variable **velocidad** si es muy alta puede saltarse el circuito, si es muy baja puede que los motores no tengan suficiente fuerza para arrancar, depende del estado del PowerBank
* La variable **luz** que depende de las condiciones de la habitación, hay que elegir un valor lo suficientemente alto para que la luz detectada por el LDR sea mayor cuando las luces de la habitación están encendidas, y lo suficientemente baja para que cuando se apaguen, el valor medido por el LDR este más bajo de ese valor.

Para la variable **luz** recomendamos usar el programa visto en [4.3 Testeo sensores](https://catedu.github.io/mClon/testeo/mBlock3.html)

![](/assets/mblock17.png)

## 4.5.2 Otros testeos

En la página https://mclon.org/ puedes encontrar interesantes propuestas en el apartado mBlock :

* Movimiento https://tecnoloxia.org/mclon/o-robot-en-movemento/
* Cerramiento en línea https://tecnoloxia.org/mclon/recinto-con-lina-2/
* Sigue líneas https://tecnoloxia.org/mclon/unha-lina-no-chan/
* Detectar objetos https://tecnoloxia.org/mclon/detectar-obxectos/
* Luces RGB https://tecnoloxia.org/mclon/extras/luces-de-cores/
* Brazo robótico https://tecnoloxia.org/mclon/extras/brazo/
* Siguiendo una luz https://tecnoloxia.org/mclon/extras/seguindo-a-luz/
