---
layout: entry
title: "Location"
shortdef: "Etiqueta para cualquier ubicación o referencia a alguno"
---

Esta entidad corresponde a expresión que represente lugares físicos o geográficos especificos. Estas entidades pueden ser nombres de ciudades, países, estados, regiones, puntos de referencia, direcciones, coordenadas geográficas y cualquier otro tipo de ubicación física identificable en un texto.


## Reglas positivas

* Anotar cualquier subdivision geográfica más pequeña que un país, incluida la dirección, la ciudad, población, comuna, región y el código postal .

<div class="annotation-correct" markdown="1">
~~~ ann
... Paso a la Bodega en Sucursal La Reina, en donde chocó...
T1 Location 33 41 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Se desmayó camino al trabajo en metro Los heroes en la mañana del martes...
T1 Location 36 52 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Estaba en terreno al sur de chile bajando por una cuesta cuando...
T1 Location 25 37 
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
