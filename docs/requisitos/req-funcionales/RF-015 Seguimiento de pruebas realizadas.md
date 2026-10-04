# RF-015 Seguimiento de pruebas realizadas
## Objetivo
Permitir al usuario DEV consultar cuántas pruebas se han realizado, cuáles fueron exitosas o tuvieron issues, y qué usuarios han realizado una prueba específica. <br>
## Alcance
Apartado de seguimiento para cuentas DEV. <br>
## Actores
## Actor principal
•	Usuario DEV
## Disparador
El usuario DEV entra al apartado de seguimiento de pruebas. <br>
## Precondiciones
•	RF-000: la cuenta es de tipo DEV y tiene la sesión iniciada.<br>
•	RF-007: existen pruebas realizadas por los usuarios.
## Postcondiciones
## En éxito
El DEV ve el resumen de pruebas realizadas y el estado de realización de cada prueba por usuario. <br>
## En fallo
No se muestra la información y el DEV no puede consultar el avance de las pruebas. <br>
## Flujo principal
1.	El DEV entra al apartado de seguimiento.
2.	El sistema muestra cuántas pruebas se han realizado, cuántas fueron exitosas y cuántas tuvieron issues.
3.	El DEV selecciona una prueba específica.
4.	El sistema muestra qué usuarios la han realizado y cuáles todavía no.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	Falla la carga de la información: el sistema muestra un mensaje de error y permite reintentar.
## Datos relevantes
## Entradas
•	Prueba específica a consultar
## Salidas
•	Conteo de pruebas realizadas, exitosas y con issues<br>
•	Lista de usuarios que han realizado o no una prueba
