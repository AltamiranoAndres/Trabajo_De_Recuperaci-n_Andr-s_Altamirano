# Informe
Andrés Altamirano

1. **PLANTEAMIENTO DEL PROBLEMA**

Este trabajo se realiza para ofrecer una perspectiva de programación orientada a  la plataforma arduino mediante una plataforma auxiliar llamada visuino, se detalla la explicación del funcionamiento de componentes dentro de la plataforma, para  la realización de diversos proyectos que tengan como componente un  Display de Cristal Líquido (LCD) que es una pantalla  capaz de mostrar datos de variables, ó datos fijos.


2. **OBJETIVOS**

  GENERAL
  
  Explicar el funcionamiento de una pantalla  LCD de 16x2 en la plataforma visuino


  
  
  ESPECÍFICOS
  
-Demostrar cómo se pueden imprimir datos de sensores en pantallas LCD de 16x2 a través del uso de la plataforma visuino
--Explicar el modo de empleo de visuino y la aplicación de sus respectivas librerías para compilar el código programado
-Explicar el procedimiento para vincular la pantalla LCD con un sensor de ultrasonido  HC-SR04    
     
3. **MARCO TEÓRICO**

Dentro del desarrollo de la programación de arduino existen diversas applets que sirven como complemento ó como una guia para poder generar códigos complicados a través de procedimientos sencillos fundamentados en programación por bloques. En este caso Visuino es una plataforma que sirve para implementar códigos de arduino  utilizando un lenguaje gráfico intuitivo.

El modo de operación de visuino es sencillo , ya que se basa en arrastrar y soltar elementos hacia el área de trabajo, cada bloque posee una descripción de sus entradas, por lo que se pueden hacer diversas confuguraciones y acceder a diferentes menús que proporcionan información que puede modificarse. Es importante señalar que el software es compatible con diversos dispositivos de hardware, tanto genéricos como originales.

Partiendo de este punto es imprescindible mencionar la gama de diversos dispositivos que se pueden incluir, dentro del desarrollo del proyecto se involucrará  a un sensor de  ultrasonido y un pantalla LCD, que sea capaz de digitar los datos obtenidos por el sensor, además, también se dispondrá de diodos led que provean una referencia de rango, que se pueda visualizar, a su vez, en el componente LCD.

**Distribución de pines en los componentes**

La definición de pin, nace de la palabra "clavija" traducida del inglés, y se le denomina de este modo a las terminales o patas de conexión de un componente electrónico. Dentro del caso de estudio, cada uno de los pines de los componentes tienen diversas funciones, tales como el transporte de datos ó el suministro de energía de cada componente.

Primero nos enfocaremos en lo más sencillo, los diodos LED, cuyo acrónimo en inglés significa "Light Emitting Diode", no son más que diodos capaces de emitir diferentes  colores electroluminiscentes, que varían dependiendo el material semiconductor del que estén elaborados, están conformados por un par de pines denominados ánodo y cátodo, siendo este último el más corto. Cabe recalcar que su rango de tolerancia al voltaje va a de los 1.8 -3.8 [V]

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Diodo_led.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Diodo_led.JPG)
*Figura 2 Diodo led en tinkercad*

**Sensor de ultrasonido HC-SR04**

Por consiguiente nos enfocaremos en el sensor de ultrasonido HC-SR04. El cual puede definirse como un sensor de ultrasonido  que es usualment utilizado para mesurar distancias, cuyo funcionamiento, como su nombre lo indica, se basa en ultrasonido, mesurando distancias mediante la relación entre la frecuencia de los pulsos que emite en conjunto con la velocidad del sonido, de esta manera, puede medir distancias con bastante eficacia y a un precio .

Para la realización del proyecto es necesario saber que se deben conocer las funciones de cada pin, así que se pueden definir de la siguiente manera:

Vcc= pin de suministro de energía de 5 [V]
Gnd= pin de tierra
Echo= pin de recepción del ultrasonido
Trig= pin de emisión del ultrasonido

Existen algunas especificaciones técnicas que son important y se deben considerar.

Voltaje de Operación: 5V DC
Corriente de reposo: < 2mA
Corriente de trabajo: 15mA
Rango de medición: 2cm a 450cm
Precisión: +- 3mm
Ángulo de apertura: 15°
Frecuencia de ultrasonido: 40KHz
Duración mínima del pulso de disparo TRIG (nivel TTL): 10 μS
Duración del pulso ECO de salida (nivel TTL): 100-25000 μS
Dimensiones: 45mm x 20mm x 15mm
Tiempo mínimo de espera entre una medida y el inicio de otra 20ms (recomendable 50ms)

*Datos técnicos tomados de: https://naylampmechatronics.com/sensores-proximidad/10-sensor-ultrasonido-hc-sr04.html*

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Componente_ultrasonico.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Componente_ultrasonico.JPG)
*Figura 3 Descripción de los pines de un sensor ultrasónico, tomado de https://cdmxelectronica.com/producto/sensor-ultrasonico-hc-sr04/*

**Pantalla LCD 16x2**

La pantalla LCD con su acrónimo en inglés (Liquid Crystal Dysplay) es un componente electrónico que tiene como funcionalidad otorgar datos a través de su pantalla, sean estos números, letras, símbolos o caracteres de diversa índole, se caracteriza por ser capaz de distribuir en su pantalla información en celdas dispuestas en una matríz de 16x2 como lo indica su nombre. Su distrubución de pines es la siguiente:

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Distribucion_de_pines_LCD.jpg](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Distribucion_de_pines_LCD.jpg)

*Figura 4 distribución de pines en una pantalla LCD obtenido de  http://todoelectrodo.blogspot.com/2013/02/lcd-16x2.html*

Donde se pueden apreciar claramente los  pines de alimentación

Vss=Tierra

Vdd= 5 [V]

Vcc =Control del contraste, generalmente conectado a una resistencia variable de 10kohms

Pines de control

RS= Es el pin que hace el registro y selección de datos

RW= Pin que permite leer o escribir un dato desde la pantalla

E= es el pin llamado enabled, el cual habilita la activación de la LCD para la activación de datos

Pines de Bus de datos

Son los pines que se utilizan para la transferencia de datos, siendo escnciales los pins D4 hasta el D7.




4.**DIAGRAMA**

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Esquema_de_conexiones.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Esquema_de_conexiones.JPG)

*Figura 1 Esquema de conexiones del circuito arado en la plataforma tinkercad*

5. Lista de componentes

-Software Thinkercad

-Listado de componentes dentro del software

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/LISTA_COMPONENTES.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/LISTA_COMPONENTES.JPG)

*Figura 2 Lista de componentes obtenida de tinkercad*

6. Mapa de Variables 





7. ANÁLISIS DE RESULTADOS 





8. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN





9. **CONCLUSIONES**

-Se puede concluir que el software visuino provee al usuario de diversas facilidades al momento de realizar la programación de una placa, gracias a que resulta intuitivo, por lo que se pueden realizar códigos de manera más rápida y eficiente, si es que se carece de conocimientos de programación




10. **RECOMENDACIONES**

-Es importante accedder a información confiable al momento de realizar la investigación de librerías, en este caso, suelen ser de utilidad foros donde las personas discuten problemas que hayan surgido por la falta de librerías.


-Se debe saber interpretar correctamnte los datos adquiridos por los sensores, ya que al momento de registrarlos podríamos tener problemas con las unidades de medida que estamos adquiriendo de los sensores.


-Es importante correr los programas de prueba suministrados por el software, ya que ofrecen diferentes modos de empleo de elementos y sensores que pueden ser fácilmente modificables y ayudan a desarrollar un proyecto de manera más sencilla, rápida y eficaz.


-Es importante conocer a detalle los elementos tratados, por lo que se recomienda encarecidamente investigar acerca de la información que provee cada pin al momento de conectarse con la placa arduino.



11. CRONOGRAMA


12. BIBLIOGRAFÍA
-https://www.youtube.com/watch?v=u93nrGvITxI&fbclid=

-http://robopapa.com/Coding/

-https://www.youtube.com/watch?v=

-https://programarfacil.com/tutoriales/fragmentos/arduino/texto-en-movimiento-en-un-lcd-con-arduino

-https://www.youtube.com/watch?v

-https://naylampmechatronics.com/sensores-proximidad/10-sensor-ultrasonido-hc-sr04.

-https://cdmxelectronica.com/producto/sensor-ultrasonico-hc-sr04/

