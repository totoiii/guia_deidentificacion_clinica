---
layout: entry
title: "First_Name"
shortdef: "Etiqueta para cualquier nombre de paciente, doctor, o cualquier persona mencionada"
---


## Reglas positivas

* Etiquetar cualquier nombre de persona

<div class="annotation-correct" markdown="1">
~~~ ann
... Nombre PCTE: Edgardo Molina…
T1 First_Name 17 24 
~~~
</div>

<div class="annotation-correct" markdown="1">
Correcto: cada nombre corresponde a una etiqueta
~~~ ann
... Fué acogido por compañero de trabajo Felipe Eduardo Saez ...
T1 Date_Part 41 47 
T2 First_Name 48 55 
~~~
</div>

* Etiquetar cualquier apodo de una persona.

<div class="annotation-correct" markdown="1">
~~~ ann
... Pcte fue insultado por Don Manuel jefe de área...
T1 First_Name 27 37 
~~~
</div>
