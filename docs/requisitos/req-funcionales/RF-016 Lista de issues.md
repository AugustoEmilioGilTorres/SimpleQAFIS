# RF-016 Lista de issues
## Objetivo
Mostrar una lista de issues ordenadas de mayor a menor importancia, con su información, un link a GitHub y los datos de quién la levantó. <br>
## Alcance
Apartado de issues para cuentas DEV. <br>
## Actores
## Actor principal
•	Usuario DEV
## Disparador
El usuario DEV entra al apartado de issues. <br>
## Precondiciones
•	RF-009: existen issues levantadas en GitHub desde la plataforma.
## Postcondiciones
## En éxito
El DEV ve la lista de issues ordenada por importancia, con su información, el link a GitHub y el usuario TESTER, la hora y el navegador de cada una. <br>
## En fallo
No se muestra la lista y el DEV no puede consultar las issues. <br>
## Flujo principal
1.	El DEV entra al apartado de issues.
2.	El sistema muestra la lista de issues ordenada de mayor a menor importancia.
3.	El sistema muestra la información de cada issue y un link para verla en GitHub.
4.	El sistema muestra qué usuario TESTER levantó la issue, a qué hora y en qué navegador.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	Falla la carga de issues: el sistema muestra un mensaje de error y permite reintentar.
## Datos relevantes
## Entradas
•	Ninguna (se usa la sesión del usuario)
## Salidas
•	Lista de issues ordenada por importancia<br>
•	Link a la issue en GitHub<br>
•	Usuario TESTER, hora y navegador de cada issue
