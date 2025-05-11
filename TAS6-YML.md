
# TAS4-Red de Contenedores
## 1. Titulo
Despliegue de WordPress, MySQL y phpMyAdmin en Contenedores Docker Usando Docker Compose

## 2.Tiempo de duracion 
El tiempo fue de 160 minutos. 

## 3. Fundamentos:

## Docker Compose 

Docker Compose es una herramienta para definir y ejecutar aplicaciones multicontenedor. Es la clave para lograr una experiencia de desarrollo e implementación optimizada y eficiente. Compose simplifica el control de toda la pila de aplicaciones, facilitando la gestión de servicios, redes y volúmenes en un único archivo de configuración YAML. Con un solo comando, se crean e inician todos los servicios desde el archivo de configuración. Compose funciona en todos los entornos: producción, staging, desarrollo, pruebas y flujos de trabajo de integración continua (CI)  (Docker Compose | Documentación de Docker, n.d.). 

También incluye comandos para gestionar todo el ciclo de vida de la aplicación:

- Iniciar, detener y reconstruir servicios
- Ver el estado de los servicios en ejecución
- Transmitir la salida del registro de los servicios en ejecución
- Ejecutar un comando único en un servicio

<img src="./redes-container/redes.png" alt="drawing0" width="500"/>

## YAML

YAML es un lenguaje de serialización de datos que las personas pueden comprender y suele utilizarse en el diseño de archivos de configuración. Para algunas personas, la sigla YAML significa "otro lenguaje de marcado más"; para otras, es un acrónimo recursivo que quiere decir "YAML no es un lenguaje de marcado", lo que enfatiza la idea de que se utiliza para los datos, no para los documentos (YAML: Qué Es, Usos, Sintaxis y Ejemplos, n.d.). 

YAML tiene características que provienen de Perl, C, XML, HTML y otros lenguajes de programación. También se basa en JSON, por lo que los archivos JSON son compatibles con YAML. No hay símbolos de formato habituales, como llaves, corchetes, etiquetas de cierre o comillas. Además, los archivos de este lenguaje son más sencillos de leer, ya que utilizan sangría al estilo Python para determinar la estructura e indicar la incrustación de un elemento de código dentro de otro. Está diseñado para que no se admitan los caracteres de tabulación y así se mantenga la portabilidad en todos los sistemas, por lo que se usan los espacios en blanco, que son los caracteres de espacio. Los comentarios se identifican con una almohadilla o símbolo numeral (#), y su uso es una práctica recomendada, ya que describen la intención del código. YAML no es compatible con los comentarios que tienen varias líneas, por lo cual el carácter de almohadilla se debe utilizar como sufijo de cada una (YAML: Qué Es, Usos, Sintaxis y Ejemplos, n.d.).


<img src="./redes-container/sql.png" alt="drawing0" width="500"/>

## 4. Conocimientos previos.
   
Para realizar esta practica el estudiante necesita tener claro los siguientes temas:
- Comandos de Docker y Docker Compose.
- Conceptos de contenedores y volumenes.
- Conceptos básicos de bases de datos.
- Conocimientos de acceso web y puertos.
- Estructura de archivos YAML.

## 5. Objetivos a alcanzar

- Construir un archivo docker compose usando el formato YML.
- Estructurar 3 servicios: wordpress, mysql, phpmyadmin
- Definir una red.
- Definir un volumen

## 6. Equipo necesario:
  
- Computador.
- Docker y Docker Compose funcionando.
- Navegador web.

## 7. Material de apoyo.
   
- Documentación de Docker y Docker Compose.
- Guía de asignatura.
- Cheat Sheet de comandos Docker.
- Documentación oficial de MySQL, phpMyAdmin y Wordpress.
- Videos tutoriales de redes Docker.

## 8. Procedimiento

### Pasos 

1. Construir un archivo docker compose usando el formato YML.

Figura 8-1 Creación del archivo docker-compose.yml

<img src="./redes-container/r1.PNG" alt="drawing0" width="500"/>

2. Estructurar 3 servicios: wordpress, mysql, phpmyadmin

Figura 8-2 Estructura de los servicios.

<img src="./redes-container/r2.PNG" alt="drawing0" width="500"/>

3. Definir una red.

Figura 8-3 Definicion de la red personalizada.

<img src="./redes-container/r3.PNG" alt="drawing0" width="500"/>


4. Definir un volumen.

Figura 8-4 Definicion de un volumen

<img src="./redes-container/r4.PNG" alt="drawing0" width="500"/>


## 9. Resultados esperados:
    
Al finalizar la práctica, se logró cumplir exitosamente los objetivos planteados. Se desplegó correctamente un contenedor de base de datos MySQL, se desplegaron los servicios de phpMyAdmin y WordPress, cada uno conectado correctamente a la base de datos MySQL a través de una red personalizada definida en el archivo ``docker-compose.yml``. Desde phpMyAdmin, accesible mediante el puerto ``8083``, se pudo verificar la existencia de la base de datos generada automáticamente por WordPress, confirmando así la conexión entre los servicios. A través del navegador web, se accedió al instalador de WordPress en el puerto ``8084``, completando su configuración inicial y dejando operativa la plataforma para su uso. Durante el desarrollo de la práctica, se aplicaron conceptos clave como la creación de redes personalizadas, la definición de volúmenes para almacenamiento persistente y el uso de variables de entorno para conectar servicios. Todo el entorno fue desplegado utilizando únicamente el archivo ``docker-compose.yml``, lo cual simplificó la configuración, redujo errores y permitió una orquestación más eficiente de los contenedores.

Todo el desarrollo de la práctica fue documentado con capturas de pantalla que evidencian la creación de la red personalizada, la definición de volúmenes y la correcta estructuración del ``archivo docker-compose.yml`` para el despliegue de los contenedores de ``MySQL``, ``phpMyAdmin`` y ``WordPress``. A través de Docker Compose se logró desplegar los servicios de forma eficiente, especificando variables de entorno, puertos y dependencias. Se verificó la conectividad entre los contenedores, la configuración adecuada de las credenciales de acceso y la correcta visualización del sitio WordPress.
<img src="./redes-container/resultado.PNG" alt="drawing0" width="500"/>


## 10. Bibliografía
    
- Docker Compose | Documentación de Docker. (n.d.). Retrieved May 9, 2025, from https://docs.docker.com/compose/
- YAML: qué es, usos, sintaxis y ejemplos. (n.d.). Retrieved May 9, 2025, from https://www.redhat.com/es/topics/automation/what-is-yaml
 


