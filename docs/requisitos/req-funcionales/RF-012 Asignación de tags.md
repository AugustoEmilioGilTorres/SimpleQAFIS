# RF-012 Asignación de tags
## Objetivo
Permitir al usuario DEV asignar tags a las preguntas y a los usuarios TESTER. <br>
## Alcance
Apartado de administración para cuentas DEV. <br>
## Actores
## Actor principal
•	Usuario DEV
## Disparador
El usuario DEV entra a la gestión de tags de una pregunta o de un usuario TESTER. <br>
## Precondiciones
•	RF-000: la cuenta es de tipo DEV y tiene la sesión iniciada.<br>
•	Existe la pregunta o el usuario TESTER al que se le asignará el tag.
## Postcondiciones
## En éxito
El tag queda asignado y guardado en la pregunta o en el usuario TESTER. <br>
## En fallo
El tag no se asigna y la pregunta o el usuario conservan sus tags anteriores. <br>
## Flujo principal
1.	El DEV accede al apartado de gestión de tags.
2.	El DEV selecciona una pregunta o un usuario TESTER.
3.	El DEV asigna el tag.
4.	El sistema guarda la asignación.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	Falla el guardado de la asignación: el sistema muestra un mensaje de error, conserva la selección y permite reintentar.
## Datos relevantes
## Entradas
•	Pregunta o usuario TESTER seleccionado<br>
•	Tag a asignar
## Salidas
•	Tag asignado y guardado<br>
•	Confirmación al usuario
