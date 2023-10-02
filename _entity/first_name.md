---
layout: entry
title: "First_Name"
shortdef: "Etiqueta para cualquier nombre de paciente, doctor, o cualquier persona mencionada."
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
T1 First_Name 41 47 
T2 First_Name 48 55 
~~~
</div>

* Etiquetar cualquier apodo de una persona.

<div class="annotation-correct" markdown="1">
~~~ ann
... Pcte fue insultado por Pepito jefe de área...
T1 First_Name 27 33 
~~~
</div>

## Reglas negativas 

* No etiquetar los tratamientos, como Don, Doña, Sra., Srta., etc.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Pcte fue insultado por Don Pepito jefe de área...
T1 First_Name 27 37 
~~~
</div>
