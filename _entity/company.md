---
layout: entry
title: "Company"
shortdef: "Etiqueta para nombres de instituciones."
---

Una institución corresponde a una organización, estructura o entidad establecida dentro de una sociedad para cumplir con una función específica. Estas entidades pueden ser de naturaleza pública o privada y abarcan una amplia gama de campos, como la educación, la religión, la política, la economía y la cultura, entre otras.

A continuación se encuentran las reglas de anotación de Company.

## Reglas positivas

* Etiquetar todos nombres de instituciones, empresas, organizaciones, etc.

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE trabaja en Scotiabank. se dirigía a su trabajo cuando ...
T1 Company 20 30 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
...TRAS ROBO DE CAMIONETA MIENTRAS SE TRASLADABA LLAMO A CARABINEROS ...
T1 Company 57 68 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... Trabaja como DOCENTE en Colegio Público b-42. En su jornada laboral se encontraba...
T1 Company 28 48 
~~~
</div>


## Reglas negativas

* NO etiquetar nombres de instituciones cuando se estén refiriendo a ellas como lugar:

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Se accidentó a las afueras del Colegio Público b-42. En su jornada laboral se encontraba...
T1 Company 35 55 
~~~
</div>


* NO etiquetar todas las menciones de instituciones generales.

<div class="annotation-incorrect" markdown="1">
~~~ ann
...MIENTRAS TRABAJABA EN COLEGIO SIENTE MAREOS REPENTINOS ...
T1 Company 25 32 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
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
.... A LAS 17:45 ES LLEVADO A LA ACHS ...
T1 Company 33 37 
~~~
</div>


## Caso típico.

* En general las instituciones vienen mencionadas junto al lugar de uno de sus establecimientos. En este caso anotar sólo el nombre de la insitución:

  * Incorrecto:
  
<div class="annotation-incorrect" markdown="1">
~~~ ann
.... Vendedor de productos en JUMBO Providencia.  ...
T1 Company 30 47 
~~~
</div>

<div class="annotation-incorrect" markdown="1">
~~~ ann
... FA: 19.03.2018 E: Registro Civil de La Florida. Se dirigía en micro a su casa y  ...
T1 Company 22 50 
~~~
</div>

   * Correcto:
  
<div class="annotation-correct" markdown="1">
~~~ ann
.... Vendedor de productos en JUMBO de Providencia.  ...
T1 Company 30 35 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... FA: 19.03.2018 E: Registro Civil de La Florida. Se dirigía en micro a su casa y  ...
T1 Company 22 36 
~~~
</div>

* En caso de no saber si es que el lugar es parte o no del nombre de la institución. Anotar la entidad completa.

<div class="annotation-correct" markdown="1">
~~~ ann
.... TRABAJA EN AGRICOLA SANTA ROSA.  ...
T1 Company 16 35 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
.... SERVICIO LOCAL DE EDUCACIÓN DE LA JUNTA. Profesora diferencial.  ...
T1 Company 5 44 
~~~
</div>
