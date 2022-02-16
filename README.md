# Concepts-of-containers
class work about containers

Haz una copia de este documento. A continaución, investiga y contesta a las siguientes preguntas. Criterios de calificación:
* Se contesta de forma clara y concisa a lo que se pregunta.
* Se responde a todas las partes de la pregunta.
* Las respuestas concuerdan con las preguntas, están bien redactadas y no contienen faltas.
* Se incluye enlace a la fuente de la información.
* Se incluyen imágenes o diagramas que ilustran la respuesta.

1. ¿Qué es un contenedor?
Un contenedor es un formato de empaquetado que empaqueta todo el código y las dependencias de una aplicación en un formato estándar que permite su ejecución rápida y fiable en todos los entornos informáticos.
2. ¿En qué se diferencia un contenedor de una máquina virtual?
es que las maquinas virtuales virtualizan toda una máquina hasta las capas de hardware, y los contenedores solo virtualizan las capas de software por encima del nivel del sistema operativo.
3. ¿Qué ventajas e inconvenientes presenta un contenedor respecto a una máquina virtual?
Ventajas:Como los contenedores son ligeros y solo incluyen software de alto nivel, son muy rápidos de modificar e iterar.
Incombenientes:Todos los contenedores comparten el mismo sistema de hardware subyacente por debajo de la capa del sistema operativo; es posible que una vulnerabilidad de un contenedor pueda salir de este y afectar al hardware compartido. Los entornos en tiempo de ejecución de contenedores más populares tienen repositorios públicos de contenedores prefabricados. Existe un riesgo de seguridad al utilizar una de estas imágenes públicas, ya que pueden contener vulnerabilidades o pueden ser un suculento objetivo para los delincuentes.
4. Dadas las siguientes tecnologías indicar cuales son de hipervisores de virtualización, cuáles de contenedores e insertar la licencia de cada una



| Tecnología | Hipervisor | Contenedor    | Licencia |
| ---------- | ---------- | --- | ---------- |
| openvz     |     X      |     |     GNU    |
| VMware     |     X      |     |  vSphere   |
| Hyper-V    |     X      |     |  Microsft  |
| podman     |            |  X  |   GNU      |
| docker     |            |  X  |   Docker   |
| lxd        |     X      |     |   GNU      |
| VirtualBox |     X      |     |   GPLv2    |
| QEMU       |     X      |     |    GNU     |



5. Microservicios. ¿Qué son?¿Qué ventajas ofrecen?
Los microservicios son un enfoque arquitectónico y organizativo para el desarrollo de software donde el software está compuesto por pequeños servicios independientes que se comunican a través de API bien definidas.
ventajas:
Modularidad: al tratarse de servicios autónomos, se pueden desarrollar y desplegar de forma independiente. Además un error en un servicio no debería afectar la capacidad de otros servicios para seguir trabajando según lo previsto.
Escalabilidad: como es una aplicación modular, se puede escalar horizontalmente cada parte según sea necesario, aumentando el escalado de los módulos que tengan un procesamiento más intensivo.
Versatilidad: se pueden usar diferentes tecnologías y lenguajes de programación. Lo que permite adaptar cada funcionalidad a la tecnología más adecuada y rentable.
Rapidez de actuación: el reducido tamaño de los microservicios permite un desarrollo menos costoso, así como el uso de “contenedores de software” permite que el despliegue de la aplicación se pueda llevar a cabo rápidamente.
Mantenimiento simple y barato: al poder hacerse mejoras de un solo módulo y no tener que intervenir en toda la estructura, el mantenimiento es más sencillo y barato que en otras arquitecturas.
Agilidad: se pueden utilizar funcionalidades típicas (autenticación, trazabilidad, etc.) que ya han sido desarrolladas por terceros, no hace falta que el desarrollador las cree de nuevo.
desventajas:
Alto consumo de memoria: al tener cada microservicio sus propios recursos y bases de datos, consumen más memoria y CPU.
Inversión de tiempo inicial: al crear la arquitectura, se necesita más tiempo para poder fragmentar los distintos microservicios e implementar la comunicación entre ellos.
Complejidad en la gestión: si contamos con un gran número de microservicios, será más complicado controlar la gestión e integración de los mismos. Es necesario disponer de una centralización de trazas y herramientas avanzadas de procesamiento de información que permitan tener una visión general de todos los microservicios y orquesten el sistema.
Perfil de desarrollador: los microservicios requieren desarrolladores experimentados con un nivel muy alto de experiencia y un control exhaustivo de las versiones. Además de conocimiento sobre solución de problemas como latencia en la red o balanceo de cargas.
No uniformidad: aunque disponer de un equipo tecnológico diferente para cada uno de los servicios tiene sus ventajas, si no se gestiona correctamente, conducirá a un diseño y arquitectura de aplicación poco uniforme.
Dificultad en la realización de pruebas: debido a que los componentes de la aplicación están distribuidos, las pruebas y test globales son más complicados de realizar.
Coste de implantación alto: una arquitectura de microservicios puede suponer un alto coste de implantación debido a costes de infraestructura y pruebas distribuidas.
6. En la aplicación desarrollada en la práctica anterior ¿Qué microservicios la comopone?
Docker-compose:php-mysql-ngix
7. ¿En qué consiste la orquestación de microservicios?
Utiliza la "Orquestación de procesos" para gestionar todas las interacciones en espera de una respuesta antes de solicitar el siguiente servicio. La orquestación sigue un paradigma de solicitud/respuesta.
8. Nombra 5 tecnologías de orquestación de contenedores/microservicios
-Kubernetes
-OpenShift
-Nomad
-Docker Swarm
-Docker Compose
## Conceptos docker

9. Según la licencia ¿Qué versiones de docker existen?¿En qué se direfencian?
    Docker Personal:uso basico del Docker Desktop, subir 200 imagenes por dia, ilimitados repositorios publicos, foros de la comunidad
    Docker Pro:Ilimitado repositorios privados, 5 compilaciones simultáneas, 50000 imagenes por dia, 5 tokens de acceso con alcance.
    Docker Team:Equipos ilimitados, 15 compilaciones simultáneas,Escaneos ilimitados y tokens de alcance
    Docker Business:Gestion centralizada,Gestión de acceso a imágenes, inicio de session unico, compra mediante factura

10. ¿Qué es Docker Hub?
es un servicio de registro de repositorios proporcionado por estibador inc. Nos permite extraer y enviar imágenes de la ventana acoplable hacia y desde Docker Hub
11. ¿Qué es un Dockerfile? 
Un DockerFile es un documento de texto que contiene todos los comandos que queramos ejecutar en la linea de comandos para armar una imágen. Esta imágen se creará mediante el comando docker build que irá siguiendo las instrucciones.
12. ¿Qué relación hay entre un Dockerfile, una imagen de docker y un contenedor de docker?
una imagen es una captura del contenedor en un momento dado y el dockerfile es un archivo de configuración que se utiliza para crear imágenes.
13. ¿Qué ventajas ofrece Docker para el **desarrollo** local de aplicaciones
muy evidente: es posible encapsular todo el entorno de trabajo, de manera que los desarrolladores pueden estar trabajando en su servidor local con la seguridad de que, al llegar el momento de poner la aplicación en producción, se va a ejecutar con la misma configuración sobre la que se han hecho todas las pruebas.
Su ligereza: al no virtualizar un sistema completo el consumo de recursos es mínimo, ahorrando alrededor de un 80% de dichos recursos—, la portabilidad y su autosuficiencia, pues Docker se encarga de la gestión del contenedor y de las aplicaciones que contenga.

###### tags: `dpl` `ut5` `contenedores` `docker` `conceptos`
