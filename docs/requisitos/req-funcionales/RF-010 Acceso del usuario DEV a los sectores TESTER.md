# RF-010 Acceso del usuario DEV a los sectores TESTER
## Objetivo
Permitir que el usuario DEV acceda a todos los sectores del usuario TESTER y realice las pruebas de forma normal. <br>
## Alcance
Pantalla de sectores y páginas de pruebas. <br>
## Actores
## Actor principal
•	Usuario DEV
## Disparador
El usuario DEV inicia sesión en la plataforma. <br>
## Precondiciones
•	RF-000: la cuenta del usuario es de tipo DEV.<br>
•	RF-001: el usuario inició sesión con sus datos de acceso.
## Postcondiciones
## En éxito
El DEV ve todos los sectores, incluidos los del usuario TESTER, y realiza las pruebas igual que un TESTER. <br>
## En fallo
El DEV no ve algún sector o no puede realizar sus pruebas. <br>
## Flujo principal
1.	El sistema identifica la cuenta como de tipo DEV.
2.	El sistema muestra todos los sectores, incluyendo los del usuario TESTER (RF-002).
3.	El DEV selecciona un sector y una prueba.
4.	El DEV realiza la prueba de forma normal (RF-004 a RF-009).
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	Falla la carga de sectores: el sistema muestra un mensaje de error y permite reintentar.
## Datos relevantes
## Entradas
•	Sector y prueba seleccionados
## Salidas
•	Acceso a todos los sectores y pruebas
