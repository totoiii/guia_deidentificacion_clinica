---
layout: entry
title: "Health_Care_Unit"
shortdef: "Etiqueta para nombres de instituciones de salud."
---

## Reglas positivas

* Etiquetar todos los nombres específicos para instituciones de salud.

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE trabaja en CESFAM La Cisterna...
T1 Health_Care_Unit 20 38 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Refiere no acudir a ACHS porque no tenia reemplazo en trabajo...
T1 Health_Care_Unit 24 28 
~~~
</div>

* Etiquetar la descripción del lugar como parte de la institución de salud, en caso de que esta información aparezca pospuesta.

* Etiquetar el nombre de la institución de salud aunque se esté refiriendo a esta como un lugar.

## Reglas negativas

* NO etiquetar nombres genéricos de instituciones de salud, como "Hospital", "CESFAM", "SAPU", etc.

## Caso Típico

* En general, la manera de hacer referencia a los nombres de instituciones de salud en Chile es: nombre genérico + lugar en el que se encuentra, como por ejemplo (EJEMPLO). En estos casos, se etiquetará la entidad completa ya que corresponde íntegramente al nombre de la institución de salud referida.

## Caso Típico

* En ocasiones, las anamnesis vienen incialmente nombrando a la agencia en donde se llevo a cabo la consulta clínica, esto se debe anotar como Health_Care_Unit debido a que pertenece a una institución de salud.

<div class="annotation-correct" markdown="1">
~~~ ann
... Agencia Concepción. PCTE ACUDE EN LA MAÑANA POR ...
T1 Health_Care_Unit 24 28 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... AG PTO MONT. ALERGIAS NO. EDAD 28 AÑOS ...
T1 Health_Care_Unit 24 28 
~~~
</div>
