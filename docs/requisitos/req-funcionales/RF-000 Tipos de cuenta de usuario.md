# RF-000 Tipos de cuenta de usuario
## Objetivo
Definir los dos tipos de cuenta del sistema (DEV y TESTER) y los permisos de acceso de cada uno. <br>
## Alcance
Control de acceso general de la plataforma. <br>
## Actores
## Actor principal
•	Usuario DEV
•	Usuario TESTER
## Disparador
El usuario inicia sesión en la plataforma. <br>
## Precondiciones
•	La cuenta del usuario existe y tiene un tipo asignado (DEV o TESTER).
•	A las cuentas TESTER se les asignaron "tags" de sectores y pruebas.
## Postcondiciones
## En éxito
El usuario ve únicamente lo que su tipo de cuenta permite: el DEV ve todos los sectores y pruebas, el TESTER solo los de sus tags. <br>
## En fallo
El usuario no obtiene acceso a ningún sector ni prueba. <br>
## Flujo principal
1.	El sistema identifica el tipo de cuenta del usuario autenticado.
2.	Si es DEV, habilita el acceso a todo el sistema, incluyendo todos los sectores y pruebas.
3.	Si es TESTER, consulta sus tags y habilita solo los sectores y pruebas asociados.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	La cuenta no tiene un tipo válido: el sistema niega el acceso y muestra un mensaje de error.
## Datos relevantes
## Entradas
•	Tipo de cuenta (DEV o TESTER)<br>
•	Tags asignados (solo TESTER)
## Salidas
•	Permisos de acceso aplicados a la sesión
