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
| VMware     |     x      |     |  vSphere   |
| Hyper-V    |     X      |     |  Microsft  |
| podman     |            |  X  |   GNU      |
| docker     |            |  X  |   Docker   |
| lxd        |     X      |     |   GNU      |
| VirtualBox |     X      |     |   GPLv2    |
| QEMU       |     X      |     |    GNU     |



5. Microservicios. ¿Qué son?¿Qué ventajas ofrecen?

6. En la aplicación desarrollada en la práctica anterior ¿Qué microservicios la comopone?

7. ¿En qué consiste la orquestación de microservicios?

8. Nombra 5 tecnologías de orquestación de contenedores/microservicios

## Conceptos docker

9. Según la licencia ¿Qué versiones de docker existen?¿En qué se direfencian?

10. ¿Qué es Docker Hub?

11. ¿Qué es un Dockerfile? 

12. ¿Qué relación hay entre un Dockerfile, una imagen de docker y un contenedor de docker?

13. ¿Qué ventajas ofrece Docker para el **desarrollo** local de aplicaciones?

###### tags: `dpl` `ut5` `contenedores` `docker` `conceptos`
