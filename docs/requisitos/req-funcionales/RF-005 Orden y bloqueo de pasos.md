# RF-005 Orden y bloqueo de pasos
## Objetivo
Garantizar que los pasos se realicen en orden, bloqueando los que aún no corresponden. <br>
## Alcance
Página de pasos de la prueba. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El sistema muestra la lista de pasos de la prueba (RF-004). <br>
## Precondiciones
•	RF-004: el usuario seleccionó una prueba y la página de pasos ya se muestra con sus botones.
## Postcondiciones
## En éxito
Solo el paso actual y los pasos ya completados son interactivos. <br>
## En fallo
Los pasos se muestran sin distinción y se permite saltarse el orden (no aceptable). <br>
## Flujo principal
1.	El sistema muestra los pasos en orden.
2.	El sistema habilita los botones del paso actual y de los pasos ya completados.
3.	El sistema muestra en un color diferente los pasos siguientes y no permite interactuar con sus botones.
## Flujos alternos
Ninguno. <br>
## Flujos de excepción
•	El usuario intenta interactuar con un paso bloqueado: el sistema ignora la acción.
## Datos relevantes
## Entradas
•	Estado de avance de la prueba
## Salidas
•	Pasos habilitados y pasos bloqueados (con color diferenciado)
