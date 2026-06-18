# Examen Final Arquitectura de Computadores

## Objetivo del proyecto

Implementar una solución de despliegue automatizado en AWS utilizando CloudFormation y GitHub Actions. El proyecto permite crear y eliminar una instancia EC2 de manera automática mediante workflows ejecutados desde GitHub.

---

## Tecnologías utilizadas

* AWS CloudFormation
* AWS EC2
* GitHub Actions
* GitHub
* NGINX
* Linux (Amazon Linux)
* YAML

---

## Funcionalidad de Deploy

El workflow **deploy.yaml** permite desplegar automáticamente la infraestructura definida en el template CloudFormation.

Acciones realizadas:

* Configuración de credenciales AWS.
* Ejecución del template CloudFormation.
* Creación de la instancia EC2.
* Creación del Security Group.
* Instalación automática de NGINX mediante UserData.
* Publicación de la página web de presentación.

---

## Funcionalidad de Destroy

El workflow **destroy.yml** permite eliminar automáticamente todos los recursos creados por CloudFormation.

Acciones realizadas:

* Configuración de credenciales AWS.
* Eliminación del stack de CloudFormation.
* Eliminación de la instancia EC2.
* Eliminación del Security Group asociado.

---

## Objetivo del Template EC2

El template CloudFormation tiene como objetivo automatizar la creación de una instancia EC2 Amazon Linux con acceso HTTP habilitado mediante un Security Group.

Además, mediante UserData se realiza:

* Actualización del sistema operativo.
* Instalación de NGINX.
* Instalación de herramientas adicionales.
* Creación automática de una página web personalizada.
* Configuración inicial del servidor.

---

## Autor

Yordy Pacheco

Universidad Francisco de Paula Santander Ocaña

Examen Final - Arquitectura de Computadores

## codigo
0192498
