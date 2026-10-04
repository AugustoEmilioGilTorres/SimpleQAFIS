# RF-011 Uso de tags para sectores y preguntas
## Objetivo
Identificar y ordenar con tags los sectores y preguntas de los usuarios TESTER, de modo que cada TESTER solo vea y responda lo que corresponde a su tag. <br>
## Alcance
Todas las pantallas donde se muestran sectores y preguntas a los usuarios TESTER. <br>
## Actores
## Actor principal
•	Usuario TESTER
## Disparador
El usuario TESTER accede a los sectores o a las pruebas. <br>
## Precondiciones
•	RF-000: la cuenta es de tipo TESTER y tiene tags asignados.<br>
•	RF-012: los sectores y las preguntas tienen tags asignados.
## Postcondiciones
## En éxito
El TESTER ve y responde únicamente los sectores y preguntas que tienen su misma tag. <br>
## En fallo
El TESTER no ve sectores ni preguntas, o ve contenido de una tag que no le corresponde. <br>
## Flujo principal
1.	El sistema obtiene los tags del usuario TESTER.
2.	El sistema filtra y ordena los sectores y preguntas que tienen la misma tag.
3.	El sistema muestra al TESTER únicamente ese contenido.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	El TESTER intenta ver o responder una pregunta con una tag distinta a la suya: el sistema no la muestra ni permite responderla.<br>
•	Falla la consulta de tags: el sistema muestra un mensaje de error y no muestra contenido.
## Datos relevantes
## Entradas
•	Tags del usuario TESTER<br>
•	Tags de sectores y preguntas
## Salidas
•	Sectores y preguntas filtrados y ordenados por tag
