# Información del producto
## ¿Qué es SimpleQA y cuál es su objetivo?
SimpleQA es una plataforma web creada para facilitar y organizar el proceso de
aseguramiento de la calidad (QA). Su propósito es proporcionar un espacio donde
las personas encargadas de realizar las pruebas puedan llevarlas a cabo de una
manera sencilla, ordenada y fácil de seguir, mientras que el equipo de desarrollo
puede consultar y dar seguimiento a los resultados obtenidos.<br>


La plataforma cuenta con dos tipos principales de usuarios: DEV y TESTER, cada
uno con diferentes funciones y permisos de acuerdo con sus responsabilidades
dentro del proceso de QA.<br>


Los usuarios TESTER pueden iniciar sesión y visualizar los sectores de pruebas
que tienen disponibles. El acceso a estos sectores se determina mediante tags
asignados a cada usuario, por lo que cada TESTER puede acceder únicamente al
contenido que le corresponde.<br>


Dentro de cada sector se encuentran las pruebas disponibles. Cada prueba cuenta
con una serie de pasos que el TESTER debe seguir en orden para comprobar que
el funcionamiento de la aplicación sea el esperado. Conforme avanza, puede marcar
los pasos como completados y consultar visualmente cuáles ya fueron realizados y
cuáles se encuentran pendientes.<br>


En caso de encontrar un problema durante una prueba, el usuario puede reportarlo
como una issue desde la misma plataforma. Para ello, SimpleQA proporciona un
formulario donde se solicita la información necesaria para registrar el problema y
permite adjuntar una imagen como evidencia. Una vez completada la información
requerida, la issue puede enviarse a GitHub mediante su API para que el equipo de
desarrollo pueda darle seguimiento.<br>


SimpleQA también registra información sobre las pruebas realizadas. Esto permite
identificar cuáles fueron completadas exitosamente, cuáles presentaron algún
problema y cuáles no pudieron ser terminadas. Los usuarios DEV pueden consultar
esta información para conocer el estado del proceso de QA y revisar las issues
reportadas.<br>


Además, los usuarios DEV pueden administrar diferentes elementos del sistema,
como sectores, preguntas y tags, así como crear o modificar preguntas
manualmente. La plataforma también contempla utilizar información de pruebas
proporcionadas en GitHub para facilitar la creación de preguntas.<br>


En general, el objetivo de SimpleQA es facilitar la ejecución y seguimiento del
proceso de QA, reduciendo la necesidad de que los usuarios TESTER interactúen
directamente con herramientas técnicas como GitHub y proporcionando al equipo
DEV información organizada sobre las pruebas y problemas encontrados.
## Alcance del producto
El alcance define a los usuarios DEV y TESTER de la FILEY APP pues ellos son quienes usarán el sistema, SimpleQA funciona como una herramienta de apoyo al proceso de QA y no como un reemplazo de las actividades de desarrollo, corrección de errores o
administración general del proyecto. 
## Propuesta de valor
El proceso de QA puede requerir que las personas encargadas de realizar las
pruebas interactúen con herramientas y procesos técnicos para registrar los
problemas encontrados. Esto puede dificultar la participación de usuarios que no
están familiarizados con estas herramientas y puede provocar que los reportes de
problemas sean incompletos o poco uniformes. 

Además, el equipo de desarrollo necesita recibir información suficiente para
comprender y dar seguimiento a los problemas detectados durante las pruebas.


SimpleQA funciona como un punto intermedio entre las personas que realizan las
pruebas y el equipo de desarrollo, se busca simplificar la experiencia del TESTER sin eliminar
la información necesaria para que el equipo de desarrollo pueda dar seguimiento a
los problemas.
