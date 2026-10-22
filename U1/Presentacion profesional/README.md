# Kevin Chalán | Portafolio Profesional

Portafolio web personal de Kevin Anthony Chalán Yamberla, estudiante de Ingeniería de Software en la Universidad de las Fuerzas Armadas ESPE.

---

## Objetivo del Proyecto

Desarrollar una presentación profesional en formato web que muestre información personal, formación académica, proyectos destacados y un formulario de contacto. El proyecto es desplegado mediante un contenedor Docker usando Nginx como servidor web, lo que permite ejecutarlo en cualquier entorno de forma rápida y reproducible.

---

## Tecnologías Utilizadas

| Tecnología | Uso |
|---|---|
| **HTML5** | Estructura y contenido del sitio |
| **CSS3** | Estilos, diseño responsivo y animaciones |
| **Nginx Alpine** | Servidor web dentro del contenedor |
| **Docker** | Contenerización y despliegue del proyecto |
| **Docker Hub** | Repositorio público de la imagen |

---

## Estructura del Proyecto

```
Presentacion profesional/
├── index.html          # Página principal del portafolio
├── foto-perfil.jpg     # Fotografía de perfil
├── videoplayback.mp4   # Video de presentación
├── Dockerfile          # Definición de la imagen Docker
├── .dockerignore       # Archivos excluidos de la imagen
├── README.md           # Documentación del proyecto
└── css/
    └── estilos.css     # Hoja de estilos del portafolio
```

---

## Instrucciones rápidas para descargar, construir y desplegar la aplicación en un contenedor local.

## Requisitos Previos

* Tener instalado [Docker Desktop](https://docker.com) y en ejecución.

---

## Desde Docker Hub

Sin Código fuente 

# 1. Descargar la imagen oficial
docker pull kachalan/portafolio-profesional:latest

# 2. Iniciar el contenedor
docker run -d -p 8080:80 --name mi_portafolio kachalan/portafolio-profesional:latest
```


##  Construcción Local (Desde Código Fuente) Con Git clone en Github

# 1. Construir la imagen (Ejecutar en la raíz donde está el Dockerfile)
docker build -t kachalan/portafolio-profesional:latest .

# 2. Iniciar el contenedor
docker run -d -p 8080:80 --name mi_portafolio kachalan/portafolio-profesional:latest
```

---
## Enlace a Docker Hub

 **[hub.docker.com/r/kachalan/portafolio-profesional] (https://hub.docker.com/r/kachalan/portafolio-profesional)**

---
