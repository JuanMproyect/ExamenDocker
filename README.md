# ExamenDocker
# 🐳 Examen Práctico de Docker

![Docker](https://img.shields.io/badge/Docker-Compose-2496ED?logo=docker)

Evaluación práctica de Docker: CLI, Dockerfiles y Docker Compose.

---

## 📋 Información

- **Duración:** 80 minutos
- **Puntuación:** 20 puntos

---

## 🗂️ Estructura
```
[tu-nombre]-examen/
├── parte1/
│   └── comandos.txt
├── parte2/
│   ├── Dockerfile
│   ├── app.py
│   ├── requirements.txt
│   └── .dockerignore
└── parte3/
    ├── docker-compose.yml
    ├── api/
    │   ├── Dockerfile
    │   └── server.js
    └── web/
        └── index.html
```

---

## 📦 Parte 1: Docker CLI (6 puntos)

**Ejercicio 1.1:** Gestión de Contenedores (3 pts)
- Descargar `nginx:alpine`
- Crear contenedor `web-examen` (puerto 8080:80)
- Verificar, logs, IP, detener y eliminar

**Ejercicio 1.2:** Volúmenes (3 pts)
- Crear volumen `datos-examen`
- PostgreSQL con persistencia
- Verificar datos persisten

---

## 🐍 Parte 2: Dockerfile Python (7 puntos)

**App Flask (2 pts):**
- `GET /` → JSON con mensaje y nombre
- `GET /salud` → status ok

**Dockerfile (5 pts):**
- `python:3.11-slim`
- Usuario no-root
- `.dockerignore`

---

## 🏗️ Parte 3: Docker Compose (7 puntos)

**Stack con 3 servicios:**
- `api` (Node.js) - Puerto 3000
- `web` (Nginx) - Puerto 8080
- `db` (MongoDB) - Volumen persistente

**Redes:** frontend, backend
---

## ✅ Entrega

- Todos los archivos funcionales
- `comandos.txt` documentados
- Contenedores probados
