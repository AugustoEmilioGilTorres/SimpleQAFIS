# RF-003 Selección de sector y lista de pruebas
## Objetivo
Permitir que el usuario entre a un sector y vea sus pruebas, distinguiendo las ya completadas. <br>
## Alcance
Pantalla de sectores y pantalla de lista de pruebas del sector. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario selecciona un sector. <br>
## Precondiciones
•	RF-002: el usuario está en la pantalla de sectores y tiene al menos un sector asignado.
## Postcondiciones
## En éxito
El usuario ve la lista de pruebas del sector, con las completadas en un color diferente. <br>
## En fallo
El usuario regresa a la pantalla anterior. <br>
## Flujo principal
1.	El usuario selecciona un sector.
2.	El sistema muestra la lista de pruebas existentes en ese sector.
3.	El sistema muestra en un color diferente las pruebas ya completadas.
## Flujos alternos
## RF-003b Sector sin pruebas
1.	El sistema detecta que el sector seleccionado no tiene pruebas.
2.	El sistema muestra un texto informando al usuario.
3.	El sistema regresa al usuario a la página anterior.
## Flujos de excepción
•	Falla la carga de pruebas: el sistema muestra un mensaje de error y regresa a la página anterior.
## Datos relevantes
## Entradas
•	Sector seleccionado
## Salidas
•	Lista de pruebas con su estado (completada o no)
•	Texto de "sin pruebas"
