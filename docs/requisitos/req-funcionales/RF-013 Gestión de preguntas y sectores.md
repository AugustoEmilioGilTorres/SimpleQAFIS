# RF-013 Gestión de preguntas y sectores
## Objetivo
Permitir al usuario DEV cambiar, crear o borrar preguntas y sectores. <br>
## Alcance
Apartado de administración para cuentas DEV. <br>
## Actores
## Actor principal
•	Usuario DEV
## Disparador
El usuario DEV entra a la gestión de preguntas y sectores. <br>
## Precondiciones
•	RF-000: la cuenta es de tipo DEV y tiene la sesión iniciada.
## Postcondiciones
## En éxito
La pregunta o el sector queda creado, modificado o eliminado según lo solicitado. <br>
## En fallo
La pregunta o el sector permanece sin cambios. <br>
## Flujo principal
1.	El DEV accede al apartado de gestión de preguntas y sectores.
2.	El DEV elige crear, cambiar o borrar una pregunta o un sector.
3.	El DEV captura o confirma la información.
4.	El sistema guarda el cambio.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	Falla el guardado del cambio: el sistema muestra un mensaje de error, conserva los datos capturados y permite reintentar.
## Datos relevantes
## Entradas
•	Datos de la pregunta o del sector<br>
•	Acción a realizar (crear, cambiar o borrar)
## Salidas
•	Preguntas y sectores actualizados
