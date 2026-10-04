# RF-008 Formulario para levantar una issue
## Objetivo
Permitir al usuario reportar una issue de un paso mediante un formulario con opción de adjuntar una foto. <br>
## Alcance
Página del formulario de issue, accesible desde la página de pasos. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario presiona el botón de reportar issue en un paso. <br>
## Precondiciones
•	RF-005: el paso donde se reporta la issue es el actual o ya fue completado, por lo que su botón de reportar issue está habilitado.
## Postcondiciones
## En éxito
El usuario llega al formulario y puede llenarlo y adjuntar una foto opcional. <br>
## En fallo
El usuario permanece en la página de pasos. <br>
## Flujo principal
1.	El usuario presiona el botón de reportar issue en un paso.
2.	El sistema lo envía a otra página con el formulario.
3.	El usuario llena los datos solicitados.
4.	El usuario, si lo desea, sube una foto.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	Falla la carga de la foto: el sistema muestra un mensaje de error y permite reintentar o continuar sin foto.
## Datos relevantes
## Entradas
•	Datos solicitados por el formulario
•	Foto (opcional)<br>
## Salidas
•	Formulario mostrado y datos capturados
