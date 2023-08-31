---
layout: entry
title: "Age"
shortdef: "Etiqueta para la edad de una persona o una referencia al rango etario de ella."
---

## Reglas positivas

* Etiquetar edades específicas e incluir la palabra "años".

<div class="annotation-correct" markdown="1">
~~~ ann
… Hombre de 26 años se accidenta yendo a su hogar … 
T1 Age 12 19 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
… PCTE EDAD: 32. SE ENCONTRABA EN OFICINA CUANDO SE ACCIDENTA … 
T1 Age 13 15 
~~~
</div>

* Etiquetar referencias a edad o rangos etarios.

<div class="annotation-correct" markdown="1">
~~~ ann
… PCTE Adulto mayor. Ocupacion:carpintero … 
T1 Age 7 19 
~~~
</div>


<div class="annotation-correct" markdown="1">
~~~ ann
... Paciente joven de 24 acude al consultorio...
T1 Age 13 18 
T2 Age 22 24 
~~~
</div>


## Reglas negativas

* NO etiquetar años que no tengan que ver con edad de personas
<div class="annotation-incorrect" markdown="1">
~~~ ann
... Adminisrativo en empresa financiera con 25 años de antiguedad...
T1 Age 44 51 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Persona con operación de vesicula hace 9 años...
T1 Age 13 18 
~~~
</div>
