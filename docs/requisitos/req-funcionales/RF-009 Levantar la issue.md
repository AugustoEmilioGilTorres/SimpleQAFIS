# RF-009 Levantar la issue
## Objetivo
Permitir enviar la issue a GitHub cuando el formulario está completo. <br>
## Alcance
Página del formulario de issue. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario llena los campos obligatorios del formulario. <br>
## Precondiciones
•	RF-008: el usuario está en la página del formulario de issue, abierta desde un paso de la prueba.
## Postcondiciones
## En éxito
La issue se crea en GitHub mediante su API y el usuario continúa con la prueba (RF-006c). <br>
## En fallo
La issue no se crea y el usuario permanece en el formulario. <br>
## Flujo principal
1.	El usuario llena todos los campos obligatorios.
2.	El sistema habilita el botón para levantar la issue.
3.	El usuario presiona el botón.
4.	El sistema crea la issue usando la API de GitHub.
## Flujos alternos
## RF-009b Campos obligatorios incompletos
1.	El usuario no completa los campos obligatorios.
2.	El sistema no permite interactuar con el botón para levantar la issue.
## RF-009c El usuario cierra el formulario
1.	El usuario cierra la pestaña del formulario.
2.	El sistema NO activa el botón para completar la prueba.
3.	El usuario puede continuar con los pasos de manera normal.
## Flujos de excepción
•	Falla la API de GitHub: el sistema muestra un mensaje de error, conserva los datos capturados y permite reintentar.
## Datos relevantes
## Entradas
•	Campos obligatorios del formulario<br>
•	Foto (opcional)
## Salidas
•	Issue creada en GitHub<br>
•	Confirmación al usuario
