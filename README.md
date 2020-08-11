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

*Figura 5 Esquema de conexiones del circuito realizado en la plataforma tinkercad*


![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/C%C3%B3digo%20Fuente/C%C3%B3digo_Bloques.jpg](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/C%C3%B3digo%20Fuente/C%C3%B3digo_Bloques.jpg)

*Figura 6 Código funte en bloques*


5. Lista de componentes

-Software Thinkercad

-Software Visuino

-Listado de componentes dentro del software

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/LISTA_COMPONENTES.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/LISTA_COMPONENTES.JPG)

*Figura 7 lista de componentes obtenida de tinkercad


6. Explicación de la Estructura de bloques

La estructura de bloques se basa en las conexiones que se realizan por medio de arrastrar y pegar elementos en nuestro entorno de trabajo, por comodidad es preferible separar al armado del circuito en dos partes. Siendo la primera el circuito conformado por los leds y el sensor de ultrasonido, y la segunda, la explicación de la vinculación de la pantalla LCD con el sensor ultrasónico

**Parte 1**

Para esta primera parte, debemos vincular nuestra tarjeta arduino con nuestro sensor de ultrasonido, haciendo las conexiones en los pines tal como se ha realizado en tinkercad.

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido.JPG)

Haremos uso de la herramienta "ping average" para poder dictaminar la frecuencia de las pulsaciones de ultrasonido

Consecuentemente utilizaremos la herramienta "Compare Analog Value" que nos permite extablecer rangos con condiciones. En este caso resultan de utilidad para dictaminar el color del led que va a prenderse.
En la primera casilla, pondremos en la comparación ctBigger, que no es más que condicionar a nuestro valor a realizar una acción cuando tenemos un dato superior a 15 en este caso.

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido2.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido2.JPG)

Estableceremos los rangos como Rg1 para 30 cm Rg2 para 15 cm y Rg 3 para 0 cm.

Luego de realizar la conexión que define los rangos de distancia, procederemos a establcer condiciones para poder diferenciarlos, y que de esta manera tengan un rango de respuestas booleanas, es decir, que muestren diferentes respuestas dependiendo de los datos que recolecten, en este caso, hemos dispuesto que cada intervalo está definido por números superiores a los dispuestos. Por ejemplo, todos los números mayores a 3 cm serán un conjunto de soluciones, mientras que los que se encuentren inferiores a treinta pero superiores a quince tendrán otro rango, lo mismo con los números comprendidos del cero al quince

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido22.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido22.JPG)

Estos operadores Booleanos podemos hallarlos poniendo la palabra "gate" en el menú, por medio de ello estableceremos las condiciones como se indica en la figura. Leyéndolo de corrido se podría interpretar de la siguiente manera


Si el rango es mayor a 30 cm se encenderá un led, caso contrario, se encenderá el segundo led, que comprende al segundo rango de 15 cm hasta 30 cm. Bastará con repetir este proceso una vez más para el último led.


![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido3.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido3.JPG)

Finalmente lo único que tendremos que hacer será realizar la conexión de cada led, a los pines de nuestro arduino, como se indica en el diagrama de tinkercad y en el de bloques.

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido4.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Conexion_sensor_ultrasonido4.JPG)

Con esto tendríamos finalizada la primera parte de nuestra conexión.

**Parte 2**

Para la conexión de la pantalla LCD, tendremos que disponer en nuestro menú de componentes de la que posee las características de 16x2.

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Pantalla_LCD.JPG)

Al momento de arrastrar y pegar el componente debemos tener algo así, que por lo que se percibe a simple vista posee la misma nauraleza que la pantalla física, por lo que su conexión es más sencilla. Así que se debe proceder a conectar como se ha dispuesto en los diagramas de tinkercad y el código fuente.

Una vez realizada esta conexión, procedemos a hacer la vinculación de nuestro sensor de ultrasonido con la  herramienta "analog snapshot" que nos proporciona una traducción de los datos analógicos a datos digitales, lo que permite a la pantalla realizar la lectura de los mismos, a su vez, debemos utilizar "pulse generator" con el fin de mesurar la frecuencia en la que se tomarán los datos 


![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Programacion_pantalla_LCD11.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Programacion_pantalla_LCD11.JPG)

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Programacion_pantalla_LCD.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Programacion_pantalla_LCD.JPG)

lógicamente todos los datos que colecte nuestro snapshot tendremos que vincularlos con la pantalla LCD, y es aquí cuando recurrimos a lo explicado en el marco teórico

Anteriormente se habían creado dos elementos en la pantalla LCD, con el fin de darle un nombree al primero, y al segundo text field darle los valores que perciba el sensor de ultrasonido, respectivamente, haremos las conexiones de la siguiente manera

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Programacion_pantalla_LCD2.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Programacion_pantalla_LCD2.JPG)


Una vez realizado esto procedemos a realizar la carga del programa al software de arduino, siempre y cuando se cumplan con los requisitos previos

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/btn_arduino.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/btn_arduino.JPG)

Al momento de hacer esto símplemente debemos darle a subir el programa a nuestra tarjeta y el proceso estará finalizado.


7. ANÁLISIS DE RESULTADOS

Dentro del análisis de resultados, en cuanto a los dispositivos se puede acotar que su eficacia depende de las pulsaciones que se emitan , ya que podrán tomar mayor cantidad de medidas een intervalos de tiempo cortos, lo que otorgará cierta exactitud, pero asímismo basante ruido y difuminación en la medida, el sensor es asequible y confiable, por lo que las medidas no difieren mucho entre intervalos de tiempo.

Es también menester recalcar la versatilidad del software al momento de interaccionar con los operadores booleanos ya que simplifica bastante el trabajo.


8. DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

Para la correcta compilación del programa es muy importante tener en cuenta que se requieren librerías qu no necesariamente vienen incluidas en visuino, es por ello que mediante la búsqueda en foros es posible halla las librerías .Mitov requeridas en el desarrollo de la programación.

Para instalarlas solo basta con descargarlas, e instalarlas desde el software de Arduino.
Nos dirigimos a Programa -> Incluir librería -> Añadir biblioteca ZIP

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Instalacion_librerias.jpg](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Instalacion_librerias.jpg)

Luego símplemente debemos seleccionar nuestra librería ZIP.



9. **CONCLUSIONES**

-Se puede concluir que el software visuino provee al usuario de diversas facilidades al momento de realizar la programación de una placa, gracias a que resulta intuitivo, por lo que se pueden realizar códigos de manera más rápida y eficiente, si es que se carece de conocimientos de programación

-Visuino es una plataforma versatil que permite la interaccion de diversos dispositivos electrónicos de una manera dinámica que resulta amigable ccon el usuario, por lo que es recomendable aplicarla si es que se desconoce el lenguaje de programación de arduino

-Visuino  carece de componentes escenciales en su versión gratuita, por lo que tarde o temprano dependiendo de las necesidades del usuario, tiene a volverse una plataforma de pago




10. **RECOMENDACIONES**

-Es importante accedder a información confiable al momento de realizar la investigación de librerías, en este caso, suelen ser de utilidad foros donde las personas discuten problemas que hayan surgido por la falta de librerías.


-Se debe saber interpretar correctamnte los datos adquiridos por los sensores, ya que al momento de registrarlos podríamos tener problemas con las unidades de medida que estamos adquiriendo de los sensores.


-Es importante correr los programas de prueba suministrados por el software, ya que ofrecen diferentes modos de empleo de elementos y sensores que pueden ser fácilmente modificables y ayudan a desarrollar un proyecto de manera más sencilla, rápida y eficaz.


-Es importante conocer a detalle los elementos tratados, por lo que se recomienda encarecidamente investigar acerca de la información que provee cada pin al momento de conectarse con la placa arduino.



11. CRONOGRAMA

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Crono_trello1.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Crono_trello1.JPG)

![https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Crono_trello2.JPG](https://github.com/AltamiranoAndres/Trabajo_De_Recuperaci-n_Andr-s_Altamirano/blob/master/Img/Crono_trello2.JPG)




12. BIBLIOGRAFÍA

-https://www.youtube.com/watch?v=u93nrGvITxI&fbclid=

-http://robopapa.com/Coding/

-https://www.youtube.com/watch?v=

-https://programarfacil.com/tutoriales/fragmentos/arduino/texto-en-movimiento-en-un-lcd-con-arduino

-https://www.youtube.com/watch?v

-https://naylampmechatronics.com/sensores-proximidad/10-sensor-ultrasonido-hc-sr04.

-https://cdmxelectronica.com/producto/sensor-ultrasonico-hc-sr04/

