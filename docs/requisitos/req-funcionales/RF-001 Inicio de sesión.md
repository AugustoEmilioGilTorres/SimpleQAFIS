# RF-001 Inicio de sesión
## Objetivo
Permitir que el usuario (DEV o TESTER) ingrese sus datos de acceso para entrar a la plataforma. <br>
## Alcance
Pantalla de inicio de sesión. <br>
## Actores
## Actor principal
•	Usuario DEV<br>
•	Usuario TESTER
## Disparador
El usuario abre la plataforma. <br>
## Precondiciones
•	El usuario tiene una cuenta registrada.
## Postcondiciones
## En éxito
El usuario accede a la plataforma y ve la pantalla de sectores (RF-002). <br>
## En fallo
El usuario permanece en la pantalla de inicio de sesión sin acceso. <br>
## Flujo principal
1.	El sistema muestra la interfaz de inicio de sesión solicitando los datos de acceso.
2.	El usuario captura sus datos.
3.	El usuario confirma el inicio de sesión.
4.	El sistema valida los datos y concede el acceso.
## Flujos alternos
## RF-001b Datos de acceso erróneos
1.	El sistema detecta que los datos ingresados son incorrectos.
2.	El sistema niega el acceso a la plataforma.
3.	El sistema informa al usuario del error.
4.	El sistema regresa al usuario a la pantalla de inicio de sesión para que lo intente de nuevo.
## Flujos de excepción
•	No hay conexión con el servidor: el sistema muestra un mensaje de error y permite reintentar.
## Datos relevantes
## Entradas
•	Datos de acceso (usuario y contraseña)
## Salidas
•	Acceso concedido o negado<br>
•	Mensaje de error en caso de datos incorrectos
