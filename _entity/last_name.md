---
layout: entry
title: "Last Name"
shortdef: "Etiqueta para el Apellido de una persona"
---

## Reglas positivas

* Etiquetar todos los apellidos de personas, cada uno por separado.


<div class="annotation-correct" markdown="1">
~~~ ann
... NOMBRE Y OCUPACIÓN DE LA PERSONA HERNANDO SOTO JEFE DE AREA …
T1 Last_Name 46 50 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... ocupacion: mecanico. n: Jose Luis Prieto Vasquez …
T1 Last_Name 38 44 
T2 Last_Name 45 49 
~~~
</div>

* Etiquetar apellidos compuestos cómo un sólo apellido.

<div class="annotation-correct" markdown="1">
~~~ ann
... aviso a la empresa, el nombre y cargo es Roberta Ríos-Prado Rodríguez, jefe de prevencion de riesgos...
T1 Last_Name 64 73 
T2 Last_Name 53 63 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... aviso a la empresa, el nombre y cargo es Javiera Fernandez de León...
T1 Last_Name 53 70 
~~~
</div>
