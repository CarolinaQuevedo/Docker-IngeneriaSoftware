# Proyecto: HTML Simple en Docker

## Descripción

La aplicación consiste en una página HTML muy simple que será servida desde un contenedor Docker, utilizando **Docker** y **Nginx**.

El objetivo es practicar:

- Subida de código a un repositorio Git.
- Uso de imágenes desde Docker Hub.
- Creación de contenedores Docker.
- Documentación de los pasos de ejecución.

---

## Tecnologías utilizadas

- **HTML5** — para el contenido web.
- **Docker** — para contenerizar la aplicación.
- **Nginx** — como servidor web dentro del contenedor.
- **Git** — para control de versiones y gestión del repositorio.

---

## Requisitos previos

Asegurarse de tener instalado en el equipo:

- [Git](https://git-scm.com/downloads)
- [Docker](https://www.docker.com/get-started)

---

## Estructura del proyecto
```
docker-practico/
│
├── index.html
├── Dockerfile
└── README.md
```

## Instrucciones

### Paso 1: Descargar y clonar el repositorio

1. Abrí la terminal (CMD, PowerShell, Terminal de Linux o Mac).
2. Escribí el siguiente comando para clonar el proyecto desde GitHub:

``` git clone https://github.com/CarolinaQuevedo/Docker-IngeneriaSoftware.git ```

### Paso 2: Ingresar a la carpeta del proyecto
``` cd docker-practico ```

### Paso 3: Verificar los archivos dentro de la carpeta
Dentro del directorio deberías ver los siguientes archivos:
``` ls ```

### Paso 4: Construir la imagen Docker
Una vez dentro de la carpeta del proyecto, ejecutá el siguiente comando para construir la imagen Docker:
``` docker build -t docker-practico .```

### Paso 5: Ejecutar el contenedor
Con la imagen creada, iniciamos el contenedor ejecutando:
```docker run -d -p 8080:80 docker-practico```

### Paso 6: Ver la aplicación funcionando en el navegador
Por último, abrí tu navegador web (Chrome, Firefox, Edge, etc.) y escribí:
```http://localhost:8080```

## Licencia

Este proyecto está bajo una licencia de uso libre.  
Puedes usarlo, modificarlo y distribuirlo sin restricciones.
