# RF-002 Pantalla de sectores de pruebas
## Objetivo
Mostrar al usuario, con una interfaz sencilla y clara, los sectores de pruebas disponibles para él. <br>
## Alcance
Pantalla principal posterior al inicio de sesión. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario inicia sesión correctamente. <br>
## Precondiciones
•	RF-001: el usuario (DEV o TESTER) inició sesión con datos de acceso válidos.
## Postcondiciones
## En éxito
El usuario ve los sectores que le corresponden. <br>
## En fallo
El usuario no ve sectores y recibe un aviso. <br>
## Flujo principal
1.	El sistema consulta los sectores disponibles según el tipo de cuenta (y tags, si es TESTER).
2.	El sistema muestra los sectores en pantalla de forma clara y sencilla.
## Flujos alternos
## RF-002b Usuario sin sectores asignados
1.	El sistema detecta que el usuario no tiene ningún sector asignado.
2.	El sistema muestra un texto indicando que aún no ha sido asignado a ningún sector.
## Flujos de excepción
•	Falla la carga de sectores: el sistema muestra un mensaje de error y permite reintentar.
## Datos relevantes
## Entradas
•	Ninguna (se usa la sesión del usuario)
## Salidas
•	Lista de sectores disponibles<br>
•	Texto de "sin sectores asignados"
