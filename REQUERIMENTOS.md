NADA DE AQUI VA A QUEDARSE TRASPASENLO AL NUEVO FORMATO

RF-000

Requisitos: El sistema tiene 2 tipos de cuentas de usuario llamadas  "DEV" y "TESTER", las cuentas TESTER son manejadas via "tags" que permiten acceder a diferentes tipos de sectores y pruebas, las cuentas DEV permiten acceso a todo el sistema incluyendo los sectores y pruebas

Lectores:  
Desarrolladores de Software  
Arquitectos de software

RF-001

Requisito: El sistema provee una interfaz de inicio de sesión dónde se solicita la información de acceso al usuario (DEV o TESTER)

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software

RF-001b

Requisito: El sistema niega el acceso a la plataforma tras haber ingresado datos erróneos y devuelve al usuario (DEV o TESTER) para volverlo a intentar

Lectores:  
Usuarios Finales del sistema  
Desarrolladores de software  
Arquitectos de software

RF-002  
Requisito: se muestra en pantalla una Interfaz sencilla y clara mostrando los diferentes sectores de pruebas disponibles para el usuario

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-002b

Requisito: Se muestra un texto al usuario indicando que aún no ha sido asignado a ningún sector

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software 

RF-003

Requisito: El usuario es capaz de interactuar con las diferentes opciones mostradas, cada una lo lleva a una lista de las pruebas existentes en dicho sector y muestra en diferente color las que ya hayan sido completadas

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Diseñadores del software  
Arquitectos de software

RF-003b

Requisito: El sistema no cuenta con pruebas en el sector seleccionado, un texto en pantalla informa al usuario y lo regresa a la página anterior

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software

RF-004

Requisitos: El usuario selecciona una prueba de un sector, se le envía a una página con una serie de pasos a realizar, cada paso cuenta de lado derecho con dos botones, uno para dar por completado el paso y otro para reportar una issue en ese paso

Lectores  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software

RF-005

Requisito: La lista muestra los pasos en orden y solo permite interactuar con el paso actual o pasos ya completados, los pasos siguientes se muestran de un color diferente y no se permite interactuar con sus botones

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-006

Requisito: Interactuar con el botón para marcar el paso como completado permite interactuar con los botones del paso siguiente

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-006b

Requisito: Interactuar con el botón para marcar el último paso como completado permite dar como completada la prueba

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-006c

Requisito: Después de reportar una issue se da la opción de terminar prematuramente la prueba

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-007

Requisito: después de haber completado al menos una prueba, se crea un nuevo sector dónde se muestra la prueba realizada y un color indicado si fue completada exitosamente, completada con issue o no se pudo completar

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-007b

Requisito: En caso de ya existir el sector de pruebas realizadas el sistema añade la prueba realizada a dicho sector

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software

RF-008

Requisito: Al interactuar con el botón para levantar una issue en un paso, el usuario es mandado a otra página donde llena los datos solicitados y se le permite subir una foto si así lo desea

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-009 Si todos los campos obligatorios del formulario para levantar una issue están llenos, se permite acceso al botón para levantar la issue usando la API de GitHub

Lectores:  
Usuarios finales del sistema  
Desarrolladores de software  
Arquitectos de software

RF-009b

Requisito: El usuario no completa los campos obligatorios en el formulario para levantar una issue por lo que no se le permite interactuar con el botón para levantar dicha issue

Lectores:  
Usuarios del sistema  
Desarrolladores de software  
Arquitectos de software

RF-009c

Requisito: El usuario cierra la pestaña del formulario para levantar un issue, el botón para completar la prueba NO se activa y el usuario puede continuar los pasos de manera normal

Lectores:  
Usuarios del sistema  
Desarrolladores de software  
Arquitectos de software

RF-010

Requisito: El usuario DEV puede acceder a todos los sectores del usuario TESTER y puede realizar las pruebas de forma normal.

Lectores:  
Usuarios del sistema  
Desarrolladores de software

RF-011

Requisito: El sistema usa “tags” para identificar y ordenar sectores y preguntas correspondientes a los usuarios TESTER, un usuario TESTER no puede ver o responder preguntas que no tengan la misma tag a la que el usuario pertenece

Lectores:  
Desarrolladores de software  
Arquitectos de software

RF-012

Requisito: El usuario DEV puede asignar tags a las preguntas y los usuarios TESTER

Lectores:  
Usuarios del sistema  
Desarrolladores de software  
Arquitectos de software

RF-013

Requisito: El Usuario DEV puede cambiar, crear o borrar preguntas y sectores

Lectores:  
Usuarios del sistema  
Desarrolladores de software  
Arquitectos de software

RF-014

Requisito: El sistema es capaz de utilizar la información de las pruebas proporcionadas en el GitHub para crear preguntas sin necesidad de que el usuario DEV las haga manualmente

Lectores:  
Desarrolladores de software  
Arquitectos de software

RF-014b

Requisito: El usuario DEV es capaz de modificar y crear nuevas preguntas de forma manual

Lectores:  
Usuarios del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-015

Requisito: El sistema cuenta con un apartado para las cuentas DEV que permite ver cuantas pruebas han sido realizadas e incluye información sobre cuales fueron realizadas exitosamente y cuantas tuvieron issues, de la misma forma puede ver que usuarios han realizado una prueba específica y cuáles todavía no la realizan

Lectores:  
Usuarios del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz

RF-016

Requisito: El sistema provee una lista de issues clasificadas en orden de mayor a menor importancia, de la misma forma provee información respecto a la issue y un link permitiendo ver el issue en GitHub, finalmente se permite ver que usuario TESTER levantó la issue, a que hora y en qué navegador

Lectores:  
Usuarios del sistema  
Desarrolladores de software  
Arquitectos de software  
Diseñadores de interfaz
