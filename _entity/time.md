---
layout: entry
title: "Time"
shortdef: "Etiqueta para una hora o referencia a ella"
---

## Reglas positivas

* Etiquetar todas las menciones de horas en específico.

<div class="annotation-correct" markdown="1">
~~~ ann
... Fecha Accidente: 20/03/2019 a las 15:45 hrs...
T1 Time 38 43 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... A eso de las 2 PM sus compañeros de trabajo lo recogieron del suelo...
T1 Time 17 21 
~~~
</div>

* Etiquetar duraciones de tiempo que tengan referencia a otra.

<div class="annotation-correct" markdown="1">
~~~ ann
...HA: 8 AM. Tras el accidente, tuvo dolor durante 3hrs...
T1 Time 7 11 
T2 Time 51 55 
~~~
</div>

* Etiquetar referencias a rangos de horarios del día.
  
<div class="annotation-correct" markdown="1">
~~~ ann
...Acude a la consulta debido a que en la mañana se accidentó caminando...
T1 Time 42 48 
~~~
</div>  

<div class="annotation-correct" markdown="1">
~~~ ann
...Paciente relata que en la noche no logra dormir...
T1 Time 29 34 
~~~
</div>  

## Reglas negativas

* NO etiquetar la palabra hrs.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... PCTE quien el día de hoy a las 13 hrs mientras se encontraba trabajando...
T1 Time 35 41 
~~~
</div>
