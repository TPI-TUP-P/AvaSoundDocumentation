---
title: Ava Sound Documentation
layout: home
nav_order: 1
---

# Ava Sound API

Bienvenido a la documentación oficial de Ava Sound.

## Descripción

Ava Sound es una plataforma para la gestión y reproducción de contenido musical, permitiendo a los usuarios almacenar, buscar y reproducir canciones mediante una API REST desarrollada en ASP.NET Core.

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

## Entidades principales

### User

Representa un usuario del sistema.

| Campo | Tipo |
|---------|---------|
| Id | Guid |
| Username | string |
| Email | string |
| Role | string |

### Song

Representa una canción almacenada.

| Campo | Tipo |
|---------|---------|
| Id | Guid |
| Title | string |
| Artist | string |
| Duration | int |
| Url | string |

### Playlist

Representa una lista de reproducción.

| Campo | Tipo |
|---------|---------|
| Id | Guid |
| Name | string |
| UserId | Guid |

---

## Endpoints

### Authentication

| Método | Endpoint |
|----------|----------|
| POST | /api/auth/register |
| POST | /api/auth/login |

### Songs

| Método | Endpoint |
|----------|----------|
| GET | /api/songs |
| GET | /api/songs/{id} |
| POST | /api/songs |
| PUT | /api/songs/{id} |
| DELETE | /api/songs/{id} |

### Playlists

| Método | Endpoint |
|----------|----------|
| GET | /api/playlists |
| POST | /api/playlists |
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

## Swagger

La documentación interactiva se encuentra disponible en:

```text
https://tu-api.com/swagger
```
