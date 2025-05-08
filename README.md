# Introducción a Docker 🐳

Docker es una plataforma que permite desarrollar, enviar y ejecutar aplicaciones dentro de contenedores. Un contenedor es una unidad estándar de software que empaqueta el código y todas sus dependencias para que la aplicación se ejecute de manera rápida y confiable en cualquier entorno.

Este repositorio contiene ejemplos básicos para comenzar a usar Docker.

## ¿Por qué Docker?

- **Portabilidad**: Funciona igual en desarrollo, pruebas y producción.
- **Consistencia**: Elimina problemas de "en mi máquina funciona".
- **Aislamiento**: Cada contenedor se ejecuta en su propio entorno.
- **Escalabilidad**: Fácil de escalar usando herramientas como Docker Compose o Kubernetes.

## Requisitos

- Tener instalado [Docker](https://www.docker.com/get-started)
- (Opcional) Tener instalado [Docker Compose](https://docs.docker.com/compose/)

## Comandos básicos

```bash
# Verificar instalación de Docker
docker --version

# Ejecutar un contenedor interactivo de Ubuntu
docker run -it ubuntu bash

# Listar contenedores en ejecución
docker ps

# Listar todos los contenedores (incluidos los detenidos)
docker ps -a

# Construir una imagen desde un Dockerfile
docker build -t nombre-de-tu-imagen .

# Ejecutar un contenedor desde una imagen
docker run -d -p 8080:80 nombre-de-tu-imagen
