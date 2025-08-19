# 📌 Foro API REST
<img width="1536" height="1024" alt="ChatGPT Image Aug 18, 2025, 07_08_19 PM" src="https://github.com/user-attachments/assets/3e96eea2-f49a-46b8-93c4-a88fa9134d4b" />


[![Java](https://img.shields.io/badge/Java-17-red?logo=java)](https://www.oracle.com/java/)  
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen?logo=springboot)](https://spring.io/projects/spring-boot)  
[![MySQL](https://img.shields.io/badge/MySQL-8-blue?logo=mysql)](https://www.mysql.com/)  
[![Flyway](https://img.shields.io/badge/Flyway-Migrations-orange?logo=flyway)](https://flywaydb.org/)  
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)

API REST desarrollada con **Java + Spring Boot**, que implementa un sistema de foro donde los usuarios pueden crear, consultar, actualizar y eliminar **tópicos**.  

Incluye autenticación con **Spring Security + JWT**, migraciones con **Flyway** y validaciones con **Spring Validation**.  

---

## ⚙️ Tecnologías utilizadas

- ☕ **Java 17**  
- 🌱 **Spring Boot**  
  - Spring Web  
  - Spring Data JPA  
  - Spring Security (JWT)  
  - Validation  
- 🐬 **MySQL**  
- 🛫 **Flyway** (migraciones de base de datos)  
- 📝 **Lombok**  

---

## 🗂️ Entidades principales

### 🔑 Usuario
- Autenticación con **JWT**.  
- Un usuario debe iniciar sesión para obtener un token y poder interactuar con el CRUD de tópicos.  

### 📝 Tópico
Representa una "tarjeta" del foro con la siguiente información:  

| Campo          | Descripción |
|----------------|-------------|
| `titulo`       | Título del tópico |
| `mensaje`      | Contenido del mensaje |
| `autor`        | Autor del tópico |
| `curso`        | Curso al que pertenece |
| `fechaCreacion`| Fecha en la que se creó |

---

## 🚀 Funcionalidades

- ✅ Registro e inicio de sesión de usuario  
- ✅ Generación de **JWT Token** para autenticación  
- ✅ CRUD de tópicos:
  - Crear  
  - Consultar  
  - Actualizar  
  - Eliminar  

---

## 📖 Endpoints principales

### 🔑 Autenticación

| Método | Endpoint       | Descripción |
|--------|---------------|-------------|
| POST   | `/login` | Autenticación y generación de token JWT |

### 📝 Tópicos

| Método | Endpoint         | Descripción |
|--------|-----------------|-------------|
| GET    | `/topicos`      | Listar todos los tópicos |
| GET    | `/topicos/{id}` | Consultar un tópico por ID |
| POST   | `/topicos`      | Crear un nuevo tópico |
| PUT    | `/topicos/{id}` | Actualizar un tópico existente |
| DELETE | `/topicos/{id}` | Eliminar un tópico |

---

