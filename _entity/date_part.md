---
layout: entry
title: "Date Part"
shortdef: "Etiqueta para un elemento o componentes de una fecha o referencia a una."
---

Una fecha se comprende como cualquier expresión que tenga un día, mes y año especifico. Date_part correspondería a una expresión que tenga una o varias componentes de una fecha. También pueden ser expresiones que hagan referencia a una fecha específica.

## Reglas positivas

* Etiquetar todas las combinaciones de día, mes y/o año, excepto cuando se encuentren las 3.

<div class="annotation-correct" markdown="1">
~~~ ann
... Durante el día 20/3 se devolvía a su casa cuando...
T1 Date_Part 19 23 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... ocupacion: operario desde agosto del 2006...
T1 Date_Part 30 45 
~~~
</div>

* Etiquetar días de la semana

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE se accidentó el sabado subiendose a la micro...
T1 Date_Part 25 31 
~~~
</div>

<div class="annotation-correct" markdown="1">
Correcto: dos etiquetas separadas
~~~ ann
... Trabaja los lunes y miercoles desde 8am hasta 16pm...
T1 Date_Part 16 21 
T2 Date_Part 24 33 
~~~
</div>

* Etiquetar referencias a fechas con respecto a otra

<div class="annotation-correct" markdown="1">
~~~ ann
... El día de ayer se accidentó levantando cemento...
T1 Date_Part 14 18 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Desde hace 6 meses inicia con dolor...
T1 Date_Part 15 22 
~~~
</div>

## Reglas negativas

* NO etiquetar duraciones o repeticiones de intervalos de tiempo en donde no se pueda llegar a obtener una fecha a partir de otra.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Paracetamol c/8hrs durante 3 días.
T1 Date_Part 31 37 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Sufre de estres ya que sólo tiene libre 3 veces en el mes.
T1 Date_Part 44 61 
~~~
</div>

