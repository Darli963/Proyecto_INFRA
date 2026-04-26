# Sistema de Compras - Proyecto Infraestructura

## Descripción
Este proyecto consiste en la migración y refactorización de un sistema legacy hacia una arquitectura moderna basada en contenedores utilizando Docker.

El sistema está compuesto por:
- Backend (Node.js + Express)
- Frontend (HTML, JS servido con Nginx)
- Base de datos (MySQL)

El objetivo es preparar el sistema para despliegue en la nube (AWS) usando herramientas de Infraestructura como Código (IaC).

---

## Arquitectura

El sistema está dividido en tres servicios principales:

- **backend**: API REST desarrollada en Node.js
- **frontend**: Aplicación estática servida por Nginx
- **mysql**: Base de datos relacional

Todos los servicios se comunican a través de una red interna definida en Docker.

---

## Tecnologías utilizadas

- Node.js
- Express
- MySQL
- Docker
- Docker Compose
- Nginx

---

## Estructura del proyecto
tree -L 3


---

## Levantar el proyecto

### Requisitos
- Docker
- Docker Compose

### Pasos

1. Clonar el repositorio:
```bash
git clone <URL_DEL_REPO>
cd Proyecto_INFRA

### Levantar los servicios:
docker-compose up --build


### Variables de entorno. -> .env


