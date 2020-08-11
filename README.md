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

Para la descarga del software se puede ingresar a la siguiente página web:

https://www.visuino.com/

Se procede al sitio de descargas

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Visuino_Descargas.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Visuino_Descargas.JPG)

y luego se selecciona una opción

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Visuino_opciones_de_descarga.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Visuino_opciones_de_descarga.JPG)

La selección de uno de estos hipervínculos generará una descarga

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Zip_visuino.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Zip_visuino.JPG)


Por consiguiente  tendremos que descomprimir el archivo


![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Descompresion_archivo.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Descompresion_archivo.JPG)


Iniciamos el ejecutable y aceptamos los términos y condiciones, finalmente podremos instal el archivo


![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Acepta_Licencia.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Acepta_Licencia.JPG)

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Inst_final.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Inst_final.JPG)

Una vez instalado podemos distinguir que se despliega un área de trabajo


![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Area_gral.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Area_gral.JPG)

Cabe destacar que la placa que aparece ahí pertenece a la de un Arduino UNO la cual viene por defecto instalada y siempe apaecerá cuando deseemos iniciar un nuevo proyecto.


Esta área se encuentra dividida en otras que indican información acerca de lo que utilizaremos, por ejemplo

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Vista_gral.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Vista_gral.JPG)

Esta sección es un indicador panorámico que nos permitirá ver de una manera amplia el entorno de trabajo, se ubica en la esquina superior izquierda.

Asimismo, tenemos una sección que nos indica las propiedades de los componentes al momento de señalarlos.

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Propiedades_componentes.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Propiedades_componentes.JPG)

Con ello podremos modificar diversos parámetros y cambiarles el nombre a nuestros componentes para poder organizarnos mejor.

Por último, existe el menú de componentes, donde ejecutaremos la acción de arrastrar y pegar lo que necesitemos, componentes, operadores, condiciones, contadores analógicos, etc.

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/menu_components.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/menu_components.JPG)



**Distribución de pines en los componentes**

La definición de pin, nace de la palabra "clavija" traducida del inglés, y se le denomina de este modo a las terminales o patas de conexión de un componente electrónico. Dentro del caso de estudio, cada uno de los pines de los componentes tienen diversas funciones, tales como el transporte de datos ó el suministro de energía de cada componente.

Primero nos enfocaremos en lo más sencillo, los diodos LED, cuyo acrónimo en inglés significa "Light Emitting Diode", no son más que diodos capaces de emitir diferentes  colores electroluminiscentes, que varían dependiendo el material semiconductor del que estén elaborados, están conformados por un par de pines denominados ánodo y cátodo, siendo este último el más corto. Cabe recalcar que su rango de tolerancia al voltaje va a de los 1.8 -3.8 [V]

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Diodo_led.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Diodo_led.JPG)


*Figura 2 Diodo led en tinkercad*

Expresión del dispositivo en bloques

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Diodo_led_visuino.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Diodo_led_visuino.JPG)

Est dispositivo es batante sencillo, por lo que en su panel de descripción no muestra nada más que una caja para cambiar su nombre.


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

Expresión del dispositivo en bloques

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Sensor_de_ultrasonido.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Sensor_de_ultrasonido.JPG)

En este bloque que representa a nuestro sensor de ultrasonido, podemos apreciar los pines echo, trigger, y un pin llamado "out" que será el que dispondrá de la salida de los datos.

Las propiedades de este sensor se representan de la siguiente manera:

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Sensor_de_ultrasonido_config.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Sensor_de_ultrasonido_config.JPG)

Donde disponemos por lo general de tiempos que podemos manipular para hacer fluctuar la adquisición de datos ó la emisión pulsos ultrasónicos. También se puede elegir las unidades de medida en las que se desea obtener los datos, en este caso se utilizarán centímetros.


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


Expresión del dispositivo en Bloques

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD.JPG)

La expresión de este dispositivo es bastente intuitiva, ya que básicamente tenemos todos los pines que el mismo dispositivo físico, pero existe una ventaja, y es que podemos disponer de diferentes elementos que podemos añadir a nuestro bloque, en este caso usaremos "text fields" que son campos de texto.

Podremos añadirlos mediante la pestaña de propiedades, de la cual se debe hacer una vista preliminar

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD_config_gral.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD_config_gral.JPG)

En este caso, añadiremos dos elementos Textfield, para poder poner texto en la pantalla. Se debe recordar que la pantalla que se está usando es de 16x2 por lo que es importante hacer una revisión de las dimensions de filas y columnas que se están manejando.

Cada uno es configurable, así que en el valor incial se procede a hacer la escritura del mensaje que se desee

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD_config_el1.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD_config_el1.JPG)

En este caso cambiaremos el nombre del componente al de "Distancia" y pondremos un texto que diga lo mismo para poder verlo en la pantalla.

Para el otro Textfield bastará con no modificar nada en "initial value" puesto a que se hará más adelante la explicación de cómo se imprimen los datos del sensor directamente.

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD_config_el2.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD_config_el2.JPG)


4.**DIAGRAMA**

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Esquema_de_conexiones.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Esquema_de_conexiones.JPG)

*Figura 5 Esquema de conexiones del circuito arado en la plataforma tinkercad*

5. Lista de componentes

-Software Thinkercad

-Listado de componentes dentro del software

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/LISTA_COMPONENTES.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/LISTA_COMPONENTES.JPG)

*Figura 6 Lista de componentes obtenida de tinkercad*

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

