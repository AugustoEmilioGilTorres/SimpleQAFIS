# RF-007 Sector de pruebas realizadas
## Objetivo
Mostrar al usuario un historial de las pruebas realizadas con su resultado. <br>
## Alcance
Pantalla de sectores y sector "Pruebas realizadas". <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario termina al menos una prueba. <br>
## Precondiciones
•	RF-006, RF-006b o RF-006c: el usuario terminó una prueba, ya sea completándola, completándola con issue o terminándola prematuramente.
## Postcondiciones
## En éxito
Existe el sector de pruebas realizadas con la prueba y un color que indica su resultado. <br>
## En fallo
La prueba realizada no aparece en el historial. <br>
## Flujo principal
1.	El usuario completa al menos una prueba.
2.	El sistema crea un nuevo sector de pruebas realizadas.
3.	El sistema muestra en él la prueba realizada con un color que indica si fue completada exitosamente, completada con issue o no se pudo completar.
## Flujos alternos
## RF-007b El sector de pruebas realizadas ya existe
1.	El sistema detecta que el sector ya existe.
2.	El sistema añade la prueba realizada a dicho sector.
## Flujos de excepción
•	Falla el registro de la prueba: el sistema muestra un mensaje de error y conserva el resultado para reintentar.
## Datos relevantes
## Entradas
•	Resultado de la prueba (exitosa, con issue, no completada)
## Salidas
•	Sector de pruebas realizadas actualizado, con la prueba y su color de estado
