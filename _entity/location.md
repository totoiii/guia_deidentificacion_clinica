---
layout: entry
title: "Location"
shortdef: "Etiqueta para cualquier ubicación o referencia a alguno"
---

Esta entidad corresponde a expresión que represente lugares físicos o geográficos especificos. Estas entidades pueden ser nombres de ciudades, países, estados, regiones, puntos de referencia, direcciones, coordenadas geográficas y cualquier otro tipo de ubicación física identificable en un texto.


## Reglas positivas

* Anotar cualquier subdivision geográfica más pequeña que un país, incluida la dirección, la ciudad, población, comuna, región y el código postal.

<div class="annotation-correct" markdown="1">
~~~ ann
... Paso por la comuna San Miguel, en donde chocó...
T1 Location 16 33 
~~~
</div>

* Anotar la descripción mas extensa de lugar al que se refiera.

<div class="annotation-correct" markdown="1">
~~~ ann
... Estaba en terreno al sur de chile bajando por una cuesta cuando...
T1 Location 14 37 
~~~
</div>

* Anotar menciones lugares identificables con una subdivisión geográfica.

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE relata que se encontraba en parque los reyes cuando empieza a sentir picazón...
T1 Location 37 53 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Al momento de entrar a costanera center pcte comienza a presentar mareo intenso...
T1 Location 27 43 
~~~
</div>

* Anotar menciones a nombres de transportes públicos, ya que son identificables con una subdivisión geográfica.

<div class="annotation-correct" markdown="1">
~~~ ann
... ME ENCONTRABA VIAJANDO EN MICRO 201 YENDO A MI HOGAR CUANDO...
T1 Location 30 39 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Se desmayó camino al trabajo en metro Los heroes en la mañana del martes...
T1 Location 36 52 
~~~
</div>


## Reglas negativas

* No anotar lugares físicos o geográficos generales

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Estaba trabajando en obras bajando por el cerro y sufre contusion facial...
T1 Location 46 51 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... tras bajarse de la micro en la esquina sufre torsion de tobillo izquierdo...
T1 Location 35 42 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... tras salir de la sala de clase siente dolor intenso en brazo izquierdo...
T1 Location 21 34 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... LLevaba mas de 5 horas sentado en oficina cuando presencia hormigueos en la pierna...
T1 Location 38 45 
~~~
</div>
