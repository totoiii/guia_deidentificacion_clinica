---
layout: entry
title: "Occupation"
shortdef: "Etiqueta para el oficio, profesión u ocupación de una persona"
---

La ocupación de una persona se refiere al trabajo, empleo, profesión o actividad que dicha persona realiza como parte de su vida laboral.

## Reglas positivas

* Etiquetar términos que hacen referencia directa a ocupaciones específicas.

<div class="annotation-correct" markdown="1">
~~~ ann
...El paciente mencionó que trabaja como enfermero en el hospital local.
T1 Occupation 41 50 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
...Edad: 43. W: operario en bodega. FA: 19/03/2019 se encontraba...
T1 Occupation 41 50 
~~~
</div>


<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE informa que es profesor de educación física en colegio público.
T1 Occupation 24 52 
~~~
</div>

## Reglas negativas

* No incluir la institución o empresa en la que trabaja.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Ocupacion: auxiliar de colegio. Acude debido a que hoy siente malestar...
T1 Occupation 15 34 
~~~
</div>
