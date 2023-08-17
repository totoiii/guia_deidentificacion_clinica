---
layout: entry
title: "Date Part"
shortdef: "Etiqueta para un elemento o componentes de una fecha o referencia a una."
---

## Reglas positivas

Una fecha se comprende como cualquier expresión que tenga un día, mes y año especifico. Date_part correspondería a una expresión que tenga una o varias componentes de una fecha. También pueden ser expresiones que hagan referencia a una fecha específica.

## Reglas positivas

* Etiquetar todas las combinaciones de día, mes y/o año, excepto cuando se encuentren las 3.

<div class="annotation-correct" markdown="1">
~~~ ann
... Durante el día 20/3 se devolvía a su casa cuando...
T1 Body_Part 26 33 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... ocupacion: operario desde agosto del 2006...
T1 Body_Part 26 33 
~~~
</div>

* Etiquetar días de la semana

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE se accidentó el sabado subiendose a la micro...
T1 Body_Part 26 33 
~~~
</div>

<div class="annotation-correct" markdown="1">
Correcto: dos etiquetas separadas
~~~ ann
... Trabaja los lunes y miercoles desde 8am hasta 16pm...
T1 Body_Part 0 6 
T2 Body_Part 9 15 
~~~
</div>

* Etiquetar referencias a fechas con respecto a otra

<div class="annotation-correct" markdown="1">
~~~ ann
.. El día de ayer se accidentó levantando cemento...
T1 Body_Part 32 36 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Desde hace 6 meses inicia con dolor...
T1 Body_Part 2 12 
~~~
</div>

## Reglas negativas

* NO etiquetar duraciones de intervalos de tiempo en donde no se pueda llegar a obtener una fecha

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Paracetamol c/8hrs durante 3 días.
T1 Body_Part 30 35 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Sufre de estres ya que tiene libre 3 veces en el mes.
T1 Body_Part 30 35 
~~~
</div>

## Reglas multipalabra

* Etiquetar como una sola entidad las partes del cuerpo en las que se precisa su localización.

<div class="annotation-correct" markdown="1">
~~~ ann
Leiomiosarcoma muslo derecho con metástasis pulmonares
T1 Body_Part 15 28 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
Diverticulosis severa de colon sigmoides.
T1 Body_Part 25 40 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
… falanges distales 4 dedos mano izq.
T1 Body_Part 2 19 
T2 Body_Part 22 36 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
Extremidades inferiores: Pulsos pedios presentes… 
T1 Body_Part 0 23 
~~~
</div>
