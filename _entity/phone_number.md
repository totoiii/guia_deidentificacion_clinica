---
layout: entry
title: "Phone_Number"
shortdef: "Etiqueta para el número de telefónico"
---

En Chile, un número telefónico fijo tiene 8 dígitos, mientras que un número de teléfono móvil tiene 9 dígitos. Por lo tanto, el largo de un número telefónico en Chile puede ser de 8 o 9 dígitos, dependiendo de si es fijo o móvil, respectivamente.

## Reglas positivas

* Etiquetar todas menciones a un número telefónico

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE tras recibir golpa llamo al doctor medina al 970042791...
T1 Phone_Number 54 63 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE tiene testigos,  +56993374194 colega de trabajo...
T1 Phone_Number 26 38 
~~~
</div>

## Reglas Negativas

* NO Etiquetar todas menciones a números telefónicos de emergencia

<div class="annotation-correct" markdown="1">
~~~ ann
... PCTE tras recibir robo llamo inmediatamente a 133 ...
T1 Phone_Number 50 53 
~~~
</div>

<div class="annotation-correct" markdown="1">
~~~ ann
... llama a 131 tras sentir dolor en brazo izquierdo y ...
T1 Phone_Number 12 15 
~~~
</div>
