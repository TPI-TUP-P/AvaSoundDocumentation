---
title: Entities
layout: default
nav_order: 2
---

# Entities

### User

It represents a system user.

| Field        | Type        |
| ------------ | ----------- |
| Id           | Guid        |
| Name         | string      |
| Surname      | string      |
| Email        | string      |
| Password     | string      |
| IsArtist     | boolean     |
| IsActive     | boolean     |
| DateRegister | datetime    |
| Role         | string      |
| Song         | IColecction |

## Song

This represents a song uploaded by a user who has the variable IsArtist set to TRUE.

| Field      | Type     |
| ---------- | -------- |
| Id         | Guid     |
| IdArtist   | Guid     |
| IdAlbum    | Guid     |
| Title      | string   |
| Gender     | string   |
| Duration   | string   |
| AudioBig   | string   |
| DateUpload | datetime |
| Views      | int      |

## Statics

It keeps user statistics

| Field  | Type |
| ------ | ---- |
| Id     | Guid |
| IdUser | Guid |

## Review

This class handles user comments on artists' songs.

| Field       | Type     |
| ----------- | -------- |
| Id          | Guid     |
| IdUser      | Guid     |
| IdSong      | Guid     |
| Comment     | string   |
| DateCreated | datetime |

## ReproductionList

It manages playlists created by users.

| Field       | Type     |
| ----------- | -------- |
| Id          | Guid     |
| IdUser      | Guid     |
| Name        | string   |
| Description | string   |
| ItPublic    | boolean  |
| Creation    | datetime |

## InfoUser

This class handles non-sensitive user information.

| Field          | Type   |
| -------------- | ------ |
| Id             | Guid   |
| IdUser         | Guid   |
| ProfilePicture | string |
| Biography      | string |
| Country        | string |

## Album

Creates a set of songs belonging to a single artist and can only be created by that artist.

| Field       | Type     |
| ----------- | -------- |
| Id          | Guid     |
| IdUser      | Guid     |
| Title       | string   |
| ReleaseDate | datetime |
| FrontPage   | string   |
| Description | string   |
