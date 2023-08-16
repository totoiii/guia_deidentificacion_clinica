---
layout: entry
title: "Company"
shortdef: "Cualquier nombre de alguna institucióm o que nombre alguna institución general"
---

Una institución corresponde a una organización, estructura o entidad establecida dentro de una sociedad para cumplir con una función específica, mantener ciertos valores, normas o tradiciones, y satisfacer necesidades colectivas. Estas entidades pueden ser de naturaleza pública o privada y abarcan una amplia gama de campos, como la educación, la religión, la política, la economía y la cultura, entre otras.

A continuación se encuentran las reglas de anotación de Company.

## Reglas positivas

* Etiquetar todos nombres de instituciones.

<div class="annotation-correct" markdown="1">
~~~ ann
… Hombre de 26 años se accidenta yendo a su hogar … 
T1 Age 12 19 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
… PCTE trabaja en Scotiabank. se dirigía a su trabajo cuando …
T1 Company 17 27
~~~
</div>

* Etiquetar todas las menciones de instituciones generales.

<div class="annotation-correct" markdown="1">
~~~ ann
… Operario en constructora se accidenta mientras se dirigía a su hogar…
T1 Company 16 27
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
… Auxiliar de aseo en Hospital del Profesor …
T1 Company 27 46
~~~
</div>

## Reglas multipalabra

* Etiquetar como una sola entidad las menciones a una institución específica .

<div class="annotation-correct" markdown="1">
~~~ ann
… Profesor en Colegio Público b-72 en su jornada laboral sufrió un accidente…
T1 Company 17 33
~~~
</div>

* Etiquetar como una sola entidad las menciones a una institución general .

<div class="annotation-correct" markdown="1">
~~~ ann
… W: empresa constructora. O: Maestro. Mientras trabajaba le entró nube de polvo en el ojo…
T1 Company 5 24
~~~
</div>
