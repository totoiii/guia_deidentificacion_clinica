---
layout: entry
title: "Full_Date"
shortdef: "Etiqueta para una fecha exacta."
---


Una fecha se define como representación específica de un punto en el tiempo, compuesta por el día, mes y año.

## Reglas positivas

* Etiquetar cualquier fecha específica.

<div class="annotation-correct" markdown="1">
~~~ ann
... El tratamiento comenzará el 23 de agosto de 2020 para abordar los síntomas...
T1 Full_Date 32 52 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... O: guardia de seguridad. FA: 14/05/2018 a las 18:30hrs...
T1 Full_Date 33 43 
~~~
</div>

<div class="annotation-correct" markdown="1">
Caso típico: dividir en dos etiquetas (revisar [Date_Part](../_entity/Date_part))
~~~ ann
...Fecha Accidente: martes 20/05/2021...
T1 Full_Date 27 37  
T2 Date_Part 20 26 
~~~
</div>

