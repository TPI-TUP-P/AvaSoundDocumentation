---
title: Ava Sound Documentation
layout: home
nav_order: 1
---

# Ava Sound API

Welcome to the official Ava Sound documentation.

## Description

We created an API for a web platform focused on independent artists, allowing them to publish their music, receive feedback from the community, and gain visibility without depending on major record labels.

---

## Swagger

La documentación interactiva se encuentra disponible en:

```text
https://ava-sound.onrender.com/
```

## Architecture

The API follows a Clean Architecture-based architecture, separating responsibilities into:

- Domain
- Application
- Infrastructure
- Web

---

## Tecnologías utilizadas

- ASP.NET Core 9
- Entity Framework Core
- PostgreSQL
- JWT Authentication
- Firebase Storage
- Swagger / OpenAPI
- Docker
- Render

---

## Funcionalidades

### Gestión de usuarios

- Registro de usuarios
- Inicio de sesión
- Actualización de perfil
- Gestión de roles

### Gestión de canciones

- Subida de audio
- Obtención de canciones
- Eliminación de canciones
- Actualización de metadatos

### Reproducción

- Streaming de audio
- Listas de reproducción
- Favoritos

---

## Endpoints

### Authentication

| Método | Endpoint           |
| ------ | ------------------ |
| POST   | /api/auth/register |
| POST   | /api/auth/login    |

### Songs

| Método | Endpoint        |
| ------ | --------------- |
| GET    | /api/songs      |
| GET    | /api/songs/{id} |
| POST   | /api/songs      |
| PUT    | /api/songs/{id} |
| DELETE | /api/songs/{id} |

### Playlists

| Método | Endpoint            |
| ------ | ------------------- |
| GET    | /api/playlists      |
| POST   | /api/playlists      |
| DELETE | /api/playlists/{id} |

---

## Arquitectura

La API sigue una arquitectura basada en Clean Architecture, separando responsabilidades en:

- Domain
- Application
- Infrastructure
- Presentation

---

## Autenticación

La API utiliza JWT Bearer Authentication.

```http
Authorization: Bearer {token}
```

---
