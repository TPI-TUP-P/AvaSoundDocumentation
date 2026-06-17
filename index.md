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

Interactive documentation is available at:

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

- ASP.NET 10
- Entity Framework
- JWT Authentication
- Swagger / OpenAPI
- Docker
- Render

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

## Autenticación

La API utiliza JWT Bearer Authentication.

```http
Authorization: Bearer {token}
```

---
