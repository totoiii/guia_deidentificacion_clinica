---
layout: entry
title: Guía de Anotación de Información Personal en Textos Médicos.
---

Luis Miranda (1),  Jocelyn Dunstan (1) 

1. Departamento de Ciencia de la Computación de la Escuela de Ingeniería. Pontificia Universidad Católica de Chile.


## Introducción
En un mundo cada vez más digitalizado, donde la información fluye constantemente a través de diversos canales y plataformas, la protección de la privacidad y la seguridad de los datos sensibles se ha vuelto una prioridad ineludible. La correcta anotación y etiquetado de información sensible es esencial para garantizar que se cumplan los más altos estándares de confidencialidad y se respeten las normativas legales establecidas para preservar la integridad de los datos personales y médicos. Esta guía tiene como objetivo proporcionar una instrucción sólida de la anotación manual de las entidades clave relacionadas con información personal clínica y cómo llevar a cabo este proceso de manera eficiente y precisa.

Este proyecto busca crear un cuerpo de texto (corpus) etiquetado con información persona clínica. Esta guía de etiquetado busca apoyar la labor de los(as) etiquetadores(as) y se utilizará el software [INCEpTION](https://inception-project.github.io/), en donde la interfaz es de la siguiente forma:

<img src="https://github.com/totoiii/clinical_deidentification_guideline/raw/master/static/img/image.png" width="100%"/>


### Ley N° [19.628](https://www.bcn.cl/leychile/navegar?idNorma=141599) sobre Protección de la Vida Privada

La privacidad de los datos de pacientes es una preocupación central en el ámbito de la salud en Chile. La ley chilena establece normativas específicas para proteger la confidencialidad de la información médica y personal de los pacientes. La Ley N° 19.628 sobre Protección de la Vida Privada regula la recopilación, en donde se definen los conceptos de :

* Información personal:
  
 La información personal se refiere a cualquier dato o conjunto de datos que puede identificar directa o indirectamente a una persona natural. Esto incluye datos como nombres, apellidos, números de identificación, direcciones, números de teléfono, direcciones de correo electrónico, fechas de nacimiento, entre otros. En esencia, es cualquier información que permita identificar o relacionar a una persona específica.el almacenamiento y el uso de datos personales en el país.
 
* Información sensible:
  
La información sensible es un subconjunto de información personal que abarca datos particularmente delicados o que pueden tener un impacto más significativo en la privacidad de una persona. Esta categoría puede incluir información relacionada con la salud, la orientación sexual, las creencias religiosas o filosóficas, antecedentes penales, afiliaciones sindicales y otros datos que, si se divulgaran o utilizaran incorrectamente, podrían causar perjuicio, discriminación o afectar negativamente la vida de una persona.

### Ley N° [20.584](https://www.bcn.cl/leychile/navegar?idNorma=1039348) sobre Derechos y Deberes de los Pacientes

En el ámbito médico, la Ley N° 20.584 sobre Derechos y Deberes de los Pacientes, junto con su Reglamento, establece directrices claras para el manejo de información sensible de pacientes, asegurando que se respeten sus derechos y su privacidad:

* Derechos de los Pacientes:
La ley garantiza a los pacientes una serie de derechos fundamentales en relación a su atención médica y a la privacidad de sus datos clínicos. Estos derechos incluyen el acceso a la información de su historia clínica, la obtención de una copia de sus registros médicos, el consentimiento informado antes de cualquier procedimiento o tratamiento, y el derecho a la confidencialidad y seguridad de sus datos médicos.

* Consentimiento Informado:
La ley enfatiza la importancia del consentimiento informado. Los pacientes tienen el derecho a recibir información completa y comprensible sobre su diagnóstico, opciones de tratamiento, riesgos y beneficios antes de someterse a cualquier procedimiento médico. El consentimiento debe ser otorgado voluntariamente por el paciente, después de haber recibido la información adecuada.

* Privacidad y Confidencialidad:
Se establecen normas estrictas para la confidencialidad de los datos clínicos de los pacientes. Los profesionales de la salud y las instituciones médicas deben garantizar que la información médica sea manejada de manera segura y solo sea compartida con aquellos que tengan la autorización correspondiente. Citando al artículo 3:

  *"Para los efectos del tratamiento de datos personales,
se entenderá que el prestador es el responsable de llevar
los registros o bases de datos de los pacientes que se
generen con ocasión de la gestión de los sistemas de apoyo
a la salud, y los proveedores tendrán las responsabilidades
propias de un mandatario, en los términos previstos en la
ley N° 19.628 sobre protección de la vida privada."*


### Ley de Portabilidad y Responsabilidad de Seguros de Salud  [HIPAA](https://www.hhs.gov/hipaa/index.html) en USA:
Dentro del ámbito médico, la Protected Health Information (PHI), o Información de Salud Protegida, se refiere a la información médica, de salud mental o historias clínicas que está protegida por la Ley de Portabilidad y Responsabilidad de Seguros de Salud (HIPAA) en los Estados Unidos. Esta ley establece normas rigurosas para la protección de la privacidad y la seguridad de los datos médicos y personales de los pacientes.
La HIPAA identifica un conjunto específico de 18 categorías de datos, conocidas como los "18 PHI Identifiers," que son considerados especialmente sensibles y deben recibir una protección adicional. Estos identificadores abarcan información que podría utilizarse para identificar a un individuo en particular. Algunos de los identificadores incluyen:

 * 1.-Nombre
 * 2.-Dirección (todas las subdivisiones geográficas más pequeñas que el estado, incluyendo dirección de calle, ciudad, condado y código postal)
 * 3.-Todos los elementos (excepto años) de fechas relacionadas con un individuo (incluyendo fecha de nacimiento, fecha de admisión, fecha de alta, fecha de fallecimiento y edad exacta si es mayor de 89 años)
 * 4.-Números de teléfono
 * 5.-Número de fax
 * 6.-Dirección de correo electrónico
 * 7.-Número de Seguro Social
 * 8.-Número de expediente médico
 * 9.-Número de beneficiario de plan de salud
 * 10.-Número de cuenta
 * 11.-Número de certificado o licencia
 * 12.-Identificadores y números de serie de vehículos, incluyendo números de matrícula
 * 13.-Identificadores y números de serie de dispositivos
 * 14.-URL web
 * 15.-Dirección de Protocolo de Internet (IP)
 * 16.-Impresión dactilar o de voz
 * 17.-Imagen fotográfica: Las imágenes fotográficas no se limitan a imágenes del rostro.
 * 18.-Cualquier otra característica que pueda identificar de manera única al individuo.

La HIPAA establece rigurosas pautas para la protección de estos identificadores y la información de salud protegida en general. Esto incluye medidas de seguridad física, administrativa y técnica para prevenir el acceso no autorizado, el uso indebido y la divulgación de datos médicos y personales. El cumplimiento de estas regulaciones es esencial para salvaguardar la privacidad y la confidencialidad de los pacientes y su información médica en los Estados Unidos.

En un contexto chileno, estos 18 identificadores PHI se han intentado adaptar para su aplicabilidad en la realidad nacional, especialmente en el ámbito de los textos médicos asociados a la Asociación Chilena de Seguridad (ACHS), que incluyen relatos de admisión y anamnesis de accidentes de trabajo o trayecto. Estos textos, que son vitales para la evaluación y el seguimiento de casos médicos, deben ser tratados con la misma rigurosidad en cuanto a la protección de datos personales/sensibles. La adopción de medidas de seguridad adecuadas, tanto físicas como tecnológicas, es fundamental para preservar la privacidad y la confidencialidad de los pacientes, garantizando que su información médica esté protegida en línea con los más altos estándares de seguridad y privacidad.

### Textos Médicos, Anamnesis y Relato de Admisión:
En la [Asociación Chilena de Seguridad](https://www.achs.cl/) (ACHS), los textos médicos adquieren un significado vital en situaciones de accidentes de trabajo y trayecto. La anamnesis se refiere al conjunto de preguntas dirigidas al paciente para obtener información médica relevante sobre su historial de salud, síntomas y condiciones preexistentes, en donde un ejemplo típico es:

* AM:- RAM:- HOY APROX 9:30 PISA SUELO RESBALADIZO RESBALANDO HACIA ADELANTE, DESPLAZANDOSE UN PAR DE METROS PERO RECUPERANDO EL EQUILIBRIO SIN CAER A SUELO, INICIANDO DOLOR SUBITO CARATER PROGRESIVO EN ASPECTO POSTERIOR DE MUSLO DERECHO.
PLAN: POR CLINICA Y DOLOR REFRACTARIO SOLICITO ECO DOPPLER URGENTE. TVP VS DESGARRO SEMIMEMBRANOSO REEV AP -ECODOPPLER (-) PARA TVP. (+) PARA DESGARRO CON COLECCION HEMATICA
-PERSISTE CON DOLOR E IMPOTENCIA FUNCIONAL. PLAN 2: -DERIVACION PARCIAL. MECANISMO INSUFICIENTE-CONTROL POR SUS SISTEMA DE PREVISION. REEV AP 15:43 DR JARA.

Por otro lado, el relato de admisión en la ACHS se centra en el registro detallado de los eventos que llevaron al accidente, proporcionando un contexto claro para el análisis y seguimiento. Un ejemplo típico corresponde a:

* AL MOMENTO DEL ACCIDENTE ESTABA CAMINO A SU TRABAJO . LO QUE OCURRIO FUE QUE BAJANDO ESCALERAS DE ESTACION DE METRO SE RESBALA CAYENDO AL PISO. EL ACCIDENTE OCURRIO CON OTROS. NO TIENE TESTIGOS DE SU ACCIDENTE, AVISO A LA EMPRESA, EL NOMBRE Y CARGO  DE LA PERSONA ES ANDREA CARRASCO, SUPERVISORA , FECHA Y HORA EN QUE AVISO A SU EMPRESA SOBRE EL ACCIDENTE: 02.10.2018 A LAS 09:40:00


## Reglas de anotación manual de entidades

Las premisas fundamentales que rigen todas las reglas de anotación en este protocolo son:

  *  **Anotar la expresión más corta y general posible**, considerando que aún así se debe describir completamente la entidad. En este sentido, las palabras modificadoras deben ser excluidas. Esto ayuda a preservar la coherencia y la fluidez del texto después de la anonimización.

  *  **Mantener el contexto clínico**.  Asegurarse de que las anotaciones de entidades nombradas en los textos clínicos conserven la información médica y contextual que rodea a esas entidades, ya que estos textos a menudo contienen información médica detallada que puede ser crucial para la comprensión y el tratamiento adecuado de los pacientes. 

  *  **Consultas para Casos Dudosos**. En caso de encontrarse en casos ambiguos, se invita a consultar en internet el nombre de empresas, apellidos, nombres, etc. En caso de que la duda persista o tenga que ver con la regla de anotación, escribir a [Luis Miranda](mailto:lmirandn@uc.cl).

Las reglas de anotación se pueden clasificar en 4 tipos:
* Reglas generales (Reglas-G): reglas positivas y negativas que se aplican a todas las etiquetas de menciones, incluyen reglas ortográficas generales.
* Reglas positivas (Reglas-P): reglas que especifican las entidades que se deben anotar.
* Reglas negativas (Reglas-N): reglas que especifican las entidades que NO hay que anotar.
* Reglas multipalabra (Regla-M): reglas que especifican si un grupo de palabras debe anotarse bajo una única etiqueta o no.

## Reglas generales
    
* No incluir en la etiqueta los espacios ni signos de puntuación que aparezcan antes o después de cada mención.

  * Correcto:

<div class="annotation-correct" markdown="1">
~~~ ann
FECHA Y HORA EN QUE AVISO A SU EMPRESA SOBRE EL ACCIDENTE: 09.03.2023 A LAS 08:30:00. ACCIDENTE OCURRIO EN...
T1 Time 76 84 
~~~
</div>.

  * Incorrecto:

<div class="annotation-correct" markdown="1">
~~~ ann
FECHA Y HORA EN QUE AVISO A SU EMPRESA SOBRE EL ACCIDENTE: 09.03.2023 A LAS 08:30:00. ACCIDENTE OCURRIO EN...
T1 Time 75 85 
~~~
</div>

  
## Reglas específicas

Las reglas asociadas a cada una de las entidades a anotar se encuentran definidas y explicadas en:

* **Entidades**
  {% for e in site.entity %}
  * [{{ e.title }}]({{ e.url | remove_first:'/' }}): {{ e.shortdef }}
  {% endfor %}

