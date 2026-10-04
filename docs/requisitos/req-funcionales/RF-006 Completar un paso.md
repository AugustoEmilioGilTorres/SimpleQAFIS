# RF-006 Completar un paso
## Objetivo
Permitir al usuario marcar un paso como completado y avanzar al siguiente. <br>
## Alcance
Página de pasos de la prueba. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario presiona el botón de completar en el paso actual. <br>
## Precondiciones
•	RF-005: los pasos se muestran en orden y el paso que se va a completar es el actual (no está bloqueado).
## Postcondiciones
## En éxito
El paso queda completado y los botones del paso siguiente se habilitan. <br>
## En fallo
El paso permanece sin completar y el siguiente sigue bloqueado. <br>
## Flujo principal
1.	El usuario presiona el botón de completar en el paso actual.
2.	El sistema marca el paso como completado.
3.	El sistema habilita los botones del paso siguiente.
## Flujos alternos
## RF-006b Completar el último paso
1.	El usuario presiona el botón de completar en el último paso.
2.	El sistema marca el paso como completado.
3.	El sistema permite dar la prueba como completada.
## RF-006c Terminar prematuramente tras reportar una issue
1.	El usuario reporta una issue en un paso (RF-008 y RF-009).
2.	El sistema ofrece la opción de terminar prematuramente la prueba.
3.	Si el usuario acepta, la prueba se da por terminada y se registra como no completada.
4.	Si el usuario no acepta, continúa con los pasos de forma normal.
## Flujos de excepción
•	Falla el guardado del avance: el sistema muestra un mensaje de error y mantiene el paso sin completar.
## Datos relevantes
## Entradas
•	Acción de completar paso<br>
•	Decisión de terminar la prueba prematuramente (RF-006c)
## Salidas
•	Paso marcado como completado<br>
•	Siguiente paso habilitado<br>
•	Prueba completada o terminada prematuramente
