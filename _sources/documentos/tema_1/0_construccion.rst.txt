Construcción del RENA-BOT
=========================

En esta sección aprenderá a ensamblar paso a paso el **RENABOT 3 en 1**, desde la preparación del chasis hasta la primera prueba de movimiento.  

.. tip::
   Arme del robot en un área amplia y bien iluminada. Mantenga organizadas las piezas y herramientas para facilitar el proceso.


Inventario de piezas y herramientas
-----------------------------------

Lista completa de componentes incluidos en el kit:

.. list-table::
   :header-rows: 1
   :widths: 15 20 20 60

   * - N°
     - Elemento
     - Cantidad
     - Imagen de referencia
   * - 1
     - Chasis
     - 1
     - .. image:: ./img/chasis.jpg
          :width: 120px
          :align: center
   * - 2
     - Guardafango I/D
     - 1
     - .. image:: ./img/estructura_ultrasonico.jpg
          :width: 120px
          :align: center
   * - 3
     - Acople T
     - 3
     - .. image:: ./img/guardafangos.jpg
          :width: 120px
          :align: center
   * - 4
     - Acople I
     - 3
     - .. image:: ./img/frente.jpg
          :width: 120px
          :align: center
   * - 5
     - Acople servo radar
     - 1
     - .. image:: ./img/extension1.jpg
          :width: 120px
          :align: center
   * - 6
     - Acople servo gripper
     - 1
     - .. image:: ./img/extension2.jpg
          :width: 120px
          :align: center
   * - 7
     - Soporte ultrasónico
     - 1
     - .. image:: ./img/soporte_radar.jpg
          :width: 120px
          :align: center
   * - 8
     - Soporte frontal
     - 1
     - .. image:: ./img/soporte_pantalla.jpg
          :width: 120px
          :align: center
   * - 9
     - Acople gripper
     - 2
     - .. image:: ./img/chasis.jpg
          :width: 120px
          :align: center
   * - 10
     - Acople estructural rodamiento
     - 2
     - .. image:: ./img/estructura_servo.jpg
          :width: 120px
          :align: center
   * - 11
     - Ruedas de transmisión dentada
     - 4
     - .. image:: ./img/estructura_gripper.jpg
          :width: 120px
          :align: center
   * - 12
     - Rueda de transmisión 375 mm
     - 4
     - .. image:: ./img/tornillo_m3_10.jpg
          :width: 120px
          :align: center
   * - 13
     - Rueda de transmisión 490 mm
     - 4
     - .. image:: ./img/tornillo_m3_30.jpg
          :width: 120px
          :align: center
   * - 14
     - Llantas diferencial
     - 2
     - .. image:: ./img/tuercas.jpg
          :width: 120px
          :align: center
   * - 15
     - Orugas plásticas
     - 2
     - .. image:: ./img/separador_12.jpg
          :width: 120px
          :align: center
   * - 16
     - Rueda loca
     - 1
     - .. image:: ./img/separador_12.jpg
          :width: 120px
          :align: center
   * - 17
     - Switch 2 estados
     - 1
     - .. image:: ./img/rueda_loca.jpg
          :width: 120px
          :align: center
   * - 18
     - Rodamiento M4
     - 2
     - .. image:: ./img/llantas.jpg
          :width: 120px
          :align: center
   * - 19
     - Cables H-h distintos tamaños
     - 9
     - .. image:: ./img/cables.jpg
          :width: 120px
          :align: center
   * - 20
     - Tornillos y tuercas M3 
     - 50
     - .. image:: ./img/placa_control.jpg
          :width: 120px
          :align: center
   * - 21 
     - Tornillos y tuercas M4 
     - 2
     - .. image:: ./img/circuito.jpg
          :width: 120px
          :align: center
   * - 22 
     - Juego sensor ultrasónico
     - 1
     - .. image:: ./img/acople_ultrasónico.jpg
          :width: 120px
          :align: center
   * - 22 
     - Juego sensor QTR8 
     - 1
     - .. image:: ./img/caja_imu.jpg
          :width: 120px
          :align: center
   * - 23
     - Juego pantalla OLED
     - 1
     - .. image:: ./img/tapa_ultra.jpg
          :width: 120px
          :align: center
   * - 24
     - Motores TT con encoder
     - 2
     - .. image:: ./img/seguidor_linea.jpg
          :width: 120px
          :align: center
   * - 25
     - Juego sensor IMU
     - 2
     - .. image:: ./img/s_ultrasonico.jpg
          :width: 120px
          :align: center
   * - 26
     - Servomotor sg90
     - 1
     - .. image:: ./img/s_sonido.jpg
          :width: 120px
          :align: center
   * - 27
     - Acople 375
     - 2
     - .. image:: ./img/s_temperatura.jpg
          :width: 120px
          :align: center
   * - 29
     - Acople 490
     - 2
     - .. image:: ./img/imu.jpg
          :width: 120px
          :align: center
   * - 30
     - Acople eje motor 
     - 2
     - .. image:: ./img/servo.jpg
          :width: 120px
          :align: center
   * - 31
     - Separadores
     - 22
     - .. image:: ./img/helice.jpg
          :width: 120px
          :align: center
   * - 32
     - Bateria 220 mAh
     - 1
     - .. image:: ./img/buzzer.jpg
          :width: 120px
          :align: center
   * - 33
     - Cargador
     - 1
     - .. image:: ./img/eje_oruga.jpg
          :width: 120px
          :align: center
   * - 34
     - Cargador de bateria 
     - 1
     - .. image:: ./img/guardafangos.jpg
          :width: 120px
          :align: center


Herramientas necesarias:

- Destornillador tipo estrella.   

El RENA-BOT puede ser armado de 4 formas diferentes, **1. Velocista**, **2. Todoterreno** y **3. Exporador**.

Modos de construcción
---------------------

Modo Velocista
~~~~~~~~~~~~~~

.. figure:: ./img/rena/velocista.svg
   :alt: modelorobot
   :align: center
   :width: 400px


Rena velocista En esta modalidad, el robot utiliza la máxima potencia de sus motores y su sistema de locomoción diferencial con tres ruedas: dos motrices y una de apoyo para estabilidad.  
Permite el desplazamiento libre en el entorno y la realización de actividades como:  

* Seguimiento de inteligente de trayectorias mediante el sensor seguidor de línea.

* Evitar de obstáculos utilizando el sensor ultrasónico.  

Ejercicios de control de velocidad y giros.   

Guía de armado:

:download:`Descargar ficha Velocista <../../_static/Velocista.pdf>`

Modo Velocista transportador
~~~~~~~~~~~~~~~~~~~~~~~~~~~~

.. figure:: ./img/rena/transportador.svg
   :alt: modelorobot
   :align: center
   :width: 400px

La versión transportador del RENABOT utiliza los Guardafangos como piezas del 
gripper que permiten transportar objetos.

Guía de armado:

:download:`Descargar ficha transportador <../../_static/velo_transportador.pdf>`

Modo Todoterreno
~~~~~~~~~~~~~~~~

.. figure:: ./img/rena/todoterreno.svg
   :alt: modelorobot
   :align: center
   :width: 400px

En esta configuración, el RENABOT adopta un diseño de movilidad con orugas, lo que lo convierte en un robot todoterreno capaz de desplazarse de manera eficiente sobre superficies 
irregulares, tanto en interiores como en exteriores.
El sistema de locomoción se basa en un control diferencial de doble oruga, 
que le permite realizar giros precisos y mantener estabilidad en terrenos complejos. A través 
del sensor ultrasónico se puede programar la evasión de obstáculos o utilizar el modo automático para evitar choques.

Guía de armado:

:download:`Descargar ficha Todoterreno <../../_static/todoterreno.pdf>`


Modo Explorador
~~~~~~~~~~~~~~~

.. figure:: ./img/rena/explorador.svg
   :alt: modelorobot
   :align: center
   :width: 400px

En esta configuración, el RENABOT utiliza el sistema de locomoción del modo todoterreno 
e incorpora una estructura adicional que eleva el sensor ultrasónico, montado sobre un 
servomotor SG90. Esta combinación le permite al robot simular un radar de exploración,
capaz de realizar un barrido configurable de 120° a 200º para la detección de obstáculos 
en el entorno.

De esta manera, el Rena Explorador no solo amplía sus capacidades de movilidad, 
sino que también potencia el aprendizaje en áreas como:

-	Robótica móvil avanzada y navegación autónoma.
-	Uso de sensores de proximidad con movimiento angular.
-	Implementación de mapas básicos y estrategias de exploración.

Guía de armado:

:download:`Descargar ficha Explorador <../../_static/Explorador_orig.pdf>`

Revisión final
--------------

Checklist de verificación:

- Todas las piezas atornilladas.  
- Conexiones firmes y sin falsos contactos.  
- Ruedas giran libremente.  

Prueba básica de movimiento
~~~~~~~~~~~~~~~~~~~~~~~~~~~

- Encendido inicial.  
- Verificación de motores.
- Práctica de movimiento libre.  

Revisa la sección :ref:`Práctica de movimiento libre <modo-libre>`.


.. tip::
	Para una mejor visualización del armado de las diferentes versiones del RENA-BOT revisa la tarjeta de consutrucción de la aplicación movil o escritorio

.. image:: ./img/rena.gif
   :width: 700px
   :align: center

Continúa con la revisión de los componentes electrónicos del RENA-BOT