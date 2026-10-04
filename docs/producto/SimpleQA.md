# Información del producto
## 1. ¿Qué es SimpleQA y cuál es su objetivo?
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
## 2. Alcance del producto
El alcance define las principales funcionalidades y responsabilidades que SimpleQA
contempla para los usuarios DEV y TESTER.


2.1 Gestión y asignación de pruebas<br>
Control de acceso por roles: el sistema diferencia entre usuarios DEV y TESTER,
proporcionando diferentes niveles de acceso según el tipo de cuenta.
Segmentación mediante tags: los usuarios TESTER pueden visualizar únicamente
los sectores y pruebas asociados con los tags que tienen asignados.
Integración con GitHub: SimpleQA puede utilizar información de pruebas
proporcionada en GitHub para facilitar la creación de preguntas dentro de la
plataforma.


Administración por parte de DEV: los usuarios DEV pueden crear, modificar y
eliminar preguntas y sectores, así como asignar tags a usuarios y contenido.


2.2 Ejecución guiada de pruebas<br>
Visualización de sectores: los usuarios pueden consultar los sectores de pruebas
disponibles de acuerdo con sus permisos.


Flujo de ejecución secuencial: las pruebas presentan sus pasos en orden y el
usuario debe completar el paso actual antes de avanzar al siguiente.


Indicadores de estado: el sistema utiliza diferentes estados visuales para distinguir
los pasos y las pruebas que han sido completados, así como aquellas que
presentaron problemas o no pudieron finalizarse.


Registro de pruebas realizadas: después de realizar una prueba, el sistema registra
su resultado para permitir su consulta posterior.


2.3 Reporte de issues<br>
Reporte desde el paso donde ocurre el problema: el TESTER puede levantar una
issue directamente desde el paso de la prueba en el que detectó el problema.
Formulario de reporte: el usuario debe proporcionar la información requerida para
registrar la issue.


Evidencia visual: el formulario permite adjuntar una imagen como evidencia del
problema.


Integración con GitHub: una vez completada la información obligatoria, la issue
puede enviarse a GitHub mediante su API.


Información del reporte: las issues pueden incluir datos como el usuario que realizó
el reporte, la hora, el navegador utilizado y un enlace hacia la issue correspondiente
en GitHub.


Finalización anticipada: después de reportar una issue, el usuario puede finalizar la
prueba antes de completar todos sus pasos.


2.4 Administración y seguimiento para usuarios DEV<br>
Consulta de resultados: los usuarios DEV pueden consultar información sobre las
pruebas realizadas, incluyendo cuáles fueron exitosas y cuáles presentaron issues.
Seguimiento de usuarios: pueden consultar qué usuarios han realizado
determinadas pruebas.


Consulta de issues: el sistema proporciona una lista de las issues reportadas,
ordenadas según su nivel de importancia, junto con información relevante y el
enlace correspondiente en GitHub.
## 3. Limitaciones del producto
Las siguientes limitaciones delimitan las responsabilidades de SimpleQA dentro del
proceso de QA:


No sustituye el proceso de desarrollo: SimpleQA permite realizar pruebas y reportar
problemas, pero la plataforma no se encarga de corregir el código ni de solucionar
los errores encontrados. Estas actividades corresponden al equipo de desarrollo.


No elimina la utilización de GitHub: aunque SimpleQA busca reducir la necesidad de
que los usuarios TESTER interactúen directamente con GitHub, mantiene una
integración con esta plataforma para registrar las issues.


Depende de la configuración realizada por los usuarios DEV: los sectores,
preguntas, pruebas y tags disponibles dependen de la información configurada y
administrada dentro del sistema.


Está orientado a la ejecución de pruebas guiadas: el funcionamiento descrito para
SimpleQA se centra en que los usuarios TESTER realicen pruebas mediante pasos
previamente definidos dentro de la plataforma.


Por lo tanto, SimpleQA funciona como una herramienta de apoyo al proceso de QA
y no como un reemplazo de las actividades de desarrollo, corrección de errores o
administración general del proyecto.
## 4. Usuarios
SimpleQA está dirigido principalmente a dos tipos de usuarios: TESTER y DEV.
Cada uno cuenta con diferentes funciones y permisos de acuerdo con las
actividades que realiza dentro del proceso de QA.


4.1 TESTER<br>
Los usuarios TESTER son las personas encargadas de realizar las pruebas. Su
principal necesidad es contar con una plataforma que les indique qué pruebas
pueden realizar y cómo llevarlas a cabo sin tener que interactuar directamente con
herramientas técnicas utilizadas para gestionar los problemas encontrados.


Al ingresar a SimpleQA, el TESTER puede visualizar los sectores de pruebas que
tiene asignados. Esto depende de los tags asociados a su usuario, por lo que no
todos los TESTER necesariamente tendrán acceso a las mismas pruebas.


Una vez seleccionado un sector, el usuario puede consultar las pruebas disponibles
y elegir la que desea realizar. Cada prueba contiene diferentes pasos que deben
seguirse en orden. El TESTER puede marcar los pasos conforme los vaya
completando y, si encuentra algún problema, puede levantar una issue
proporcionando la información correspondiente y, si lo desea, una imagen como
evidencia.


Después de realizar una prueba, el sistema registra su resultado y permite consultar
las pruebas realizadas. Esto proporciona al TESTER una visión del trabajo que ha
completado y de los resultados obtenidos.


Necesidades principales del TESTER:<br>
Acceder únicamente a las pruebas que le corresponden.<br>
Contar con instrucciones claras para realizar cada prueba.<br>
Poder identificar fácilmente qué pasos ha completado.<br>
Reportar problemas sin tener que realizar directamente el proceso técnico de
creación de una issue en GitHub.<br>
Proporcionar evidencia del problema encontrado.


4.2 DEV<br>
Los usuarios DEV son las personas encargadas del desarrollo y administración del
sistema y de dar seguimiento a la información obtenida durante el proceso de QA.


Debido a sus funciones, cuentan con mayores permisos dentro de SimpleQA.
Un DEV puede acceder a los sectores disponibles para los TESTER y realizar las
pruebas de manera normal. Además, puede administrar diferentes elementos de la
plataforma, como sectores, preguntas y tags, así como crear y modificar preguntas.
Otra de sus funciones principales es consultar la información generada durante el
proceso de QA. Los DEV pueden conocer cuántas pruebas se han realizado, cuáles
fueron completadas exitosamente, cuáles presentaron issues y qué usuarios han
realizado determinadas pruebas.


También pueden consultar las issues reportadas por los TESTER, incluyendo
información que ayude a identificar el problema, como el usuario que lo reportó, la
hora, el navegador utilizado y el enlace correspondiente a la issue en GitHub.


Necesidades principales del DEV:<br>
Administrar las pruebas y el contenido de la plataforma.<br>
Organizar el acceso mediante tags.<br>
Consultar los resultados obtenidos durante las pruebas.<br>
Revisar las issues reportadas por los TESTER.<br>
Contar con información suficiente para dar seguimiento a los problemas
encontrados.<br>


4.3 Relación entre los usuarios<br>
Los dos perfiles utilizan SimpleQA con objetivos diferentes pero complementarios:<br>
Usuario Función principal.<br>
TESTER Ejecutar pruebas y reportar problemas.<br>
encontrados durante su realización.<br>
DEV Administrar las pruebas y consultar los
resultados e issues generados por los
TESTER.


De esta manera, SimpleQA permite que ambos perfiles trabajen sobre un mismo
proceso, pero con funciones y permisos acordes con sus responsabilidades.
## 5. Propuesta de valor
“Facilitar el aseguramiento de la calidad mediante pruebas guiadas y reducir la
necesidad de interacción directa con herramientas técnicas.”


5.1 Problema que resuelve<br>
El proceso de QA puede requerir que las personas encargadas de realizar las
pruebas interactúen con herramientas y procesos técnicos para registrar los
problemas encontrados. Esto puede dificultar la participación de usuarios que no
están familiarizados con estas herramientas y puede provocar que los reportes de
problemas sean incompletos o poco uniformes.


Además, el equipo de desarrollo necesita recibir información suficiente para
comprender y dar seguimiento a los problemas detectados durante las pruebas.


5.2 Solución que propone SimpleQA<br>
SimpleQA funciona como un punto intermedio entre las personas que realizan las
pruebas y el equipo de desarrollo.


Para los TESTER, proporciona un flujo guiado en el que pueden:<br>
- acceder a las pruebas que les corresponden;<br>
- seguir los pasos en orden;<br>
- identificar visualmente su progreso;<br>
- reportar una issue desde el mismo lugar donde detectaron el problema;<br>
- proporcionar información y evidencia sobre el error.<br>


Para los DEV, proporciona información organizada sobre las pruebas realizadas y
los problemas encontrados. Además, permite administrar el contenido de las
pruebas y enviar las issues a GitHub mediante su API.


De esta forma, SimpleQA busca simplificar la experiencia del TESTER sin eliminar
la información necesaria para que el equipo de desarrollo pueda dar seguimiento a
los problemas.


5.3 Valor para los usuarios<br>
Para los TESTER:<br>
- Reduce la necesidad de interactuar directamente con herramientas técnicas.<br>
- Proporciona instrucciones y pasos claros para realizar las pruebas.<br>
- Permite reportar problemas desde la misma plataforma.<br>
- Facilita la incorporación de evidencia al reporte.<br>
- Permite visualizar el estado de las pruebas realizadas.<br>


Para los DEV:<br>
- Centraliza la información obtenida durante el proceso de QA.<br>
- Facilita la administración de pruebas, sectores, preguntas y tags.<br>
- Permite consultar los resultados de las pruebas.<br>
- Proporciona información estructurada sobre las issues.<br>
- Mantiene la integración con GitHub para el seguimiento de los problemas.


5.4 Diferenciador de la propuesta<br>
La principal propuesta de valor de SimpleQA es servir como una capa intermedia
entre la ejecución de pruebas y las herramientas utilizadas por el equipo de
desarrollo.


En lugar de requerir que el TESTER interactúe directamente con GitHub para
registrar un problema, SimpleQA proporciona un flujo diseñado específicamente
para realizar la prueba y recopilar la información necesaria para el reporte.


Posteriormente, esa información puede enviarse a GitHub para que el equipo de
desarrollo continúe con el seguimiento correspondiente.


Por lo tanto, el valor de SimpleQA se encuentra en hacer más accesible y ordenado
el proceso de QA para los TESTER, mientras mantiene la información necesaria
para el trabajo del equipo DEV.
