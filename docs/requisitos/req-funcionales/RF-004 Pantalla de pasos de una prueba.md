# RF-004 Pantalla de pasos de una prueba
## Objetivo
Mostrar los pasos de una prueba seleccionada, con las acciones de completar paso y reportar issue. <br>
## Alcance
Página de ejecución de la prueba. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario selecciona una prueba de un sector. <br>
## Precondiciones
•	RF-003: el usuario entró a un sector que cuenta con pruebas y ve su lista.
## Postcondiciones
## En éxito
El usuario ve la lista de pasos de la prueba, cada uno con sus dos botones. <br>
## En fallo
El usuario no puede iniciar la prueba y permanece en la lista de pruebas. <br>
## Flujo principal
1.	El usuario selecciona una prueba.
2.	El sistema lo envía a una página con la serie de pasos a realizar.
3.	El sistema muestra, a la derecha de cada paso, dos botones: uno para darlo por completado y otro para reportar una issue en ese paso.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	Falla la carga de los pasos: el sistema muestra un mensaje de error y regresa a la lista de pruebas.
## Datos relevantes
## Entradas
•	Prueba seleccionada
## Salidas
•	Lista de pasos con botones "completar" y "reportar issue"
