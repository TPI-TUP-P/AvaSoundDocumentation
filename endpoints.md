---
title: End Points
layout: default
nav_order: 4
---

# Endpoints

## Authentication

| Método | Endpoint           |
| ------ | ------------------ |
| POST   | /api/auth/register |
| POST   | /api/auth/login    |

## Songs

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

The API uses JWT Bearer Authentication.

```http
Authorization: Bearer {token}
```

---
