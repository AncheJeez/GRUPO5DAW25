# Despliegue-en-grupo

El objetivo fundamental de esta práctica es desplegar un proyecto ya programado, basado en el patrón de diseño modelo vista controlador (MVC).

Se trata de una aplicación web para elaborar y consultar un repositorio de alimentos con datos acerca de sus propiedades dietéticas.

Los archivos php del proyecto pueden descargarse del siguiente enlace en .zip:

Proyecto alimentos ale

Dispone de 2 carpetas:

- app (back-end donde se encuentra archivos del modelo (Model.php)  y un archivo de configuración de conexión a la base de datos, etc (Config.php) , controlador-acciones (Controller.php) y archivos de vista ( en carpeta templates))

- web (front-end donde se encuentra el controlador frontal (index.php) y archivos en carpetas js css y assets o recursos de front (images) )

Emplea una base de datos, para almacenar dichos datos que consistirá en una sola tabla con la siguiente información sobre alimentos:

    El nombre del alimento,
    la energía en kilocalorías ,
    la cantidad de proteínas,
    la cantidad hidratos de carbono en gramos
    la cantidad de fibra en gramos y
    la cantidad de grasa en gramos,

todo ello por cada 100 gramos de alimento.

La estructura de la tabla en SQL será:

CREATE TABLE `alimentos` (
  `id` int(11) NOT NULL AUTO_INCREMENT,
  `nombre` varchar(255) NOT NULL,
  `energia` decimal(10,0) NOT NULL,
  `proteina` decimal(10,0) NOT NULL,
  `hidratocarbono` decimal(10,0) NOT NULL,
  `fibra` decimal(10,0) NOT NULL,
  `grasatotal` decimal(10,0) NOT NULL,
  PRIMARY KEY (`id`)
) ENGINE=InnoDB  DEFAULT CHARSET=utf8;

Aunque se trata de una aplicación muy sencilla, cuenta con los elementos suficientes para mostrar las características básicas de un framework de PHP.

En este práctica se propone la puesta en marcha por grupos de 3  personas, de dicha aplicación ya desarrollada.

Para ello a modo de resumen se realizará:

- Crear la base de datos en el hosting de uno de los compañeros. Se empleará como hosting alwaysdata, the European Cloud

- Repartir las partes (archivos) del proyecto para que cada integrante controle localmente con git su parte solamente. El integrante responsable del archivo Config.php deberá modificarlo para indicarle los parámetros de la base de datos en el hosting.

- Subir a un repositorio GITHUB del grupo (que administra un integrante) las distintas partes.

- Publicar el contenido de GITHUB en un hosting CDMON de uno de los integrantes.

Cada integrante tendrá instalado GIT localmente y tendrá un usuario en GITHUB.
 
Cada integrante deberá realizar una serie de tareas:

- Integrante 1: Administrará el repo en GITHUB, creará el repositorio GRUPOXDAW25 público donde X será el número del grupo: 0,1,2,3,4,5,6,7,8,9 (1punto)

y asociará los otros 2 usuarios (de GITHUB) para que puedan subir y hacer aportaciones al repositorio.  (1punto)

Asumirá la subida de los archivos de la vista (carpeta /app/templates) y los de Fron-end (web/css + web/js + web/images).  (1 punto)

También recogerá las valoraciones de la experiencia del resto de integrantes (deben aparecer cada valoración de cada integrante diferenciada) y las indicará en un fichero de texto (valoraciones.txt) . (1 punto)

- Integrante 2: Asumirá el modelo y el archivo (app/Model.php ).

Creará una base de datos en el hosting denominada alimentosX2025 y ejecutará la creación de la tabla alimentos (anteriormente citada) mediante SQL.  (1 punto)

Realizará mediante SSH + comandos GIT el despliegue en su hosting en una carpeta específica para el proyecto. (1 punto)

En la cuenta de GITHUB subirá las indicaciones para la instalación y despliegue del proyecto con las acciones y comandos SSH, GIT realizados por este integrante (instalación.txt). (1 punto)

- Integrante 3: Asumirá el controlador frontal, archivo con la clase controlador, y el archivo de configuración (web/index.php + app/Controller.php + app/Config.php).  (1 punto)

Modificará el código del archivo Config.php para indicar los datos de conexión con la base de datos con los datos proporcionados por el integrante 2. (1 punto)

Explicará en un archivo de texto el histórico de tareas realizadas y al final indicará el enlace o URL en el hosting desplegado (histórico.txt). (1 punto)

 

La entrega se realizará mediante:

- el enlace o URL de la página de inicio de acceso al proyecto desplegado.

- URL del proyecto público a Github.

- se indicarán los integrantes del grupo.
