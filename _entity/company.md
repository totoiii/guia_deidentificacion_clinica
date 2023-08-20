---
layout: entry
title: "Company"
shortdef: "Nombre o mención de alguna institución específica o general."
---

Una institución corresponde a una organización, estructura o entidad establecida dentro de una sociedad para cumplir con una función específica. Estas entidades pueden ser de naturaleza pública o privada y abarcan una amplia gama de campos, como la educación, la religión, la política, la economía y la cultura, entre otras. Exceptuando las instituciones de salud (ver Reglas negativas)

A continuación se encuentran las reglas de anotación de Company.

## Reglas positivas

* Etiquetar todos nombres de instituciones, empresas, etc.

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE trabaja en Scotiabank. se dirigía a su trabajo cuando ...
T1 Company 20 30 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... FA: 19.03.2018 W: Registro Civil Se dirigía en micro a su casa y  ...
T1 Company 22 36 
~~~
</div>

* Etiquetar todas las menciones de instituciones generales.

<div class="annotation-correct" markdown="1">
~~~ ann
... Operario en constructora se accidenta mientras se dirigía a su hogar ...
T1 Company 16 28 
~~~
</div>

<!---
Esto debería ir en otra categoría dentro de finding llamada Factores de riesgo
* Etiquetar dentro de esta categoría las frases que describen hábitos de consumo.

<div class="annotation-correct" markdown="1">
~~~ ann
Consumo de alcohol: +, conusmo de cigarro: - ....
T1 Clinical_Finding 11 21 
T2 Clinical_Finding 34 44 
~~~
</div>
-->

## Reglas negativas

* NO etiquetar instituciones de salud, ya que tienen su propia etiqueta.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Auxiliar de aseo en Hospital del Profesor ...
T1 Company 24 45 
~~~
</div>

## Reglas multipalabra

* Etiquetar como una sola entidad las menciones a una institución específica .

<div class="annotation-correct" markdown="1">
~~~ ann
... Se accidentó a las afueras del Colegio Público b-72 en su jornada laboral...
T1 Company 35 56 
~~~
</div>

* Etiquetar como una sola entidad las menciones a una institución general .

<div class="annotation-correct" markdown="1">
~~~ ann
... W: empresa constructora. O: Maestro. Mientras trabajaba le entró nube de polvo en el ojo...
T1 Company 7 27 
~~~
</div>
