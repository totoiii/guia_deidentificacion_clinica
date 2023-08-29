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

<div class="annotation-correct" markdown="1">
~~~ ann
...TRAS ROBO DE CAMIONETA MIENTRAS SE TRASLADABA LLAMO A CARABINEROS ...
T1 Company 22 36 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Se accidentó a las afueras del Colegio Público b-72 en su jornada laboral...
T1 Company 35 56 
~~~
</div>

## Reglas negativas

* NO etiquetar todas las menciones de instituciones generales.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Operario en constructora se accidenta mientras se dirigía a su hogar ...
T1 Company 16 28 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
...MIENTRAS TRABAJABA EN COLEGIO SIENTE MAREOS REPENTINOS ...
T1 Company 16 28 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... W: empresa constructora. O: Maestro. Mientras trabajaba le entró nube de polvo en el ojo...
T1 Company 7 27 
~~~
</div>

* NO etiquetar instituciones de salud, ya que tienen su propia etiqueta [Health_Care_Unit](../entity/health_care_unit).

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Auxiliar de aseo en Hospital del Profesor ...
T1 Company 24 45 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... A LAS 17:45 ES LLEVADO A LA ACHS ...
T1 Company 24 45 
~~~
</div>




