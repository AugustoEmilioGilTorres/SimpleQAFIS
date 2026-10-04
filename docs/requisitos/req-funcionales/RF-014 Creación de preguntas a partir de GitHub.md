# RF-014 Creación de preguntas a partir de GitHub
## Objetivo
Crear preguntas automáticamente con la información de las pruebas proporcionadas en GitHub, sin que el usuario DEV tenga que hacerlas manualmente. <br>
## Alcance
Apartado de administración para cuentas DEV e integración con GitHub. <br>
## Actores
## Actor principal
•	Usuario DEV
## Disparador
El usuario DEV solicita generar preguntas a partir de las pruebas de GitHub. <br>
## Precondiciones
•	RF-000: la cuenta es de tipo DEV y tiene la sesión iniciada.<br>
•	Existen pruebas con información en el GitHub del proyecto.
## Postcondiciones
## En éxito
Las preguntas se crean automáticamente y quedan disponibles en el sistema. <br>
## En fallo
Las preguntas no se crean y el DEV puede crearlas de forma manual (RF-014b). <br>
## Flujo principal
1.	El sistema obtiene la información de las pruebas desde GitHub.
2.	El sistema crea las preguntas a partir de dicha información.
3.	El sistema deja las preguntas disponibles para su uso.
## Flujos alternos
## RF-014b Creación y modificación manual de preguntas
1.	El usuario DEV decide crear o modificar preguntas de forma manual.
2.	El DEV captura o edita los datos de la pregunta.
3.	El sistema guarda la pregunta.
## Flujos de excepción
•	Falla la conexión con GitHub: el sistema muestra un mensaje de error y permite reintentar o crear las preguntas manualmente.
## Datos relevantes
## Entradas
•	Información de las pruebas en GitHub<br>
•	Datos de preguntas capturados manualmente (RF-014b)
## Salidas
•	Preguntas creadas o modificadas
