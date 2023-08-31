---
layout: entry
title: "RUT"
shortdef: "Etiqueta para RUT: rol único unitario"
---

El RUT (Rol Único Tributario) en Chile es un número único de identificación que se asigna a las personas naturales y jurídicas que realicen actividades económicas en el país. Este número se utiliza para fines tributarios y administrativos, y es emitido por el Servicio de Impuestos Internos (SII) de Chile. El RUT es esencial en diversas transacciones y trámites, como la presentación de declaraciones de impuestos, la apertura de cuentas bancarias, la facturación de servicios y la participación en contratos y transacciones comerciales. Además, cada RUT lleva consigo información sobre la situación tributaria y legal de la persona o entidad. 

## Reglas positivas

* Etiquetar todas menciones al RUT


<div class="annotation-correct" markdown="1">
~~~ ann
... RUN PCTE: 10755042...
T1 RUT 19 23 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... paciente 17784042-2 se presenta hoy ...
T1 RUT 19 23 
~~~
</div>


## Reglas negativas

* NO anotar numeros que no tengan sentido con un RUT.

<div class="annotation-incorrect" markdown="1">
~~~ ann
... Se anoto 
T1 Date_Part 31 37 
~~~
</div>

