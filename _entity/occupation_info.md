---
layout: entry
title: "Occupation Info"
shortdef: "Etiqueta que menciones que hagan referencia a la ocupación de la persona"
---

Corresponde a cualquier acción, objeto, espacio, persona o cualquier otra información con la que se logre concluir a lo que se dedica una persona.

## Reglas positivas

* Etiquetar cualquier acción que se relacione directamente con la ocupación de la persona.

<div class="annotation-correct" markdown="1">
~~~ ann
... Ocupación profesor. estaba haciendo clases cuando se desploma al suelo...
T1 Occupation_info 40 46 
~~~
</div>

* Etiquetar cualquier lugar u objeto que se pueda relacionar directamente con la ocupación de la perosna.

<div class="annotation-correct" markdown="1">
~~~ ann
... Paciente trabaja en construcción. se aplasta el dedo meñique izquierdo con un martillo...
T1 Occupation_info 82 90 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Profesor lo echan de la sala de clase de manera violenta...
T1 Occupation_info 28 41 
~~~
</div>

* Etiquetar cualquier estamento que se pueda relacionar directamente con la ocupación de la perosna.

<div class="annotation-correct" markdown="1">
~~~ ann
... O: Profesor. Alumnos le gritan insultándolo descaradamente...
T1 Occupation_info 17 24 
~~~
</div>


## Reglas negativas

* NO etiquetar los casos en los que se hable de acciones u objetos asociados a áreas de la salud.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Al paciente se le inyectó insulina durante 1 semana...
T1 Occupation_info 22 38 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Al paciente se le realiza tratamiento intensivo durante 3 semanas...
T1 Occupation_info 30 51 
~~~
</div>

* NO etiquetar acciones típicas en un trabajo:

<div class="annotation-incorrect" markdown="1">
~~~ ann
... fué a una reunion de trabajo cuando se golpea en la cabeza...
T1 Occupation_info 14 33 
~~~
</div>

* NO etiquetar objetos comunes o generales en el trabajo o vida cotidiana:

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Se accidentó bajando las escaleras con torsión en tobillo derecho ...
T1 Occupation_info 29 38 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... estaba trabajando cuando salta una tapa eyectando liquido (acido sulfúrico) el cual se salta dentro del ojo derecho.
T1 Occupation_info 63 78 
~~~
</div>
