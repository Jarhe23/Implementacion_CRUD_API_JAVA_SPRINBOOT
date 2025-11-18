# API de Clientes – Spring Boot
**Autor:** Jahel Hernández  
**Tecnologías:** Java 17 · Spring Boot 3 · MySQL · JPA · Maven · Postman  

Este proyecto implementa una **API REST** para la gestión de clientes utilizando Java Spring Boot.  
El objetivo es demostrar una arquitectura profesional basada en capas y realizar operaciones básicas de un backend moderno.

---
## Tabla de Contenido

1. [Descripción del Proyecto](#-descripción-del-proyecto)
2. [Características](#-características)
3. [Tecnologías Utilizadas](#-tecnologías-utilizadas)
4. [Arquitectura](#-arquitectura)
5. [Diagrama General del Flujo](#-diagrama-general-del-flujo)
6. [Requisitos Previos](#-requisitos-previos)
7. [Instalación y Ejecución](#-instalación-y-ejecución)
8. [Configuración](#-configuración)
9. [Endpoints](#-endpoints)
10. [Ejemplos JSON](#-ejemplos-json)
11. [Pruebas con Postman](#-pruebas-con-postman)
12. [Estructura del Proyecto](#-estructura-del-proyecto)
13. [Próximas Mejoras](#-próximas-mejoras)
14. [Créditos](#-créditos)

---

##  Descripción del Proyecto

Este proyecto implementa un sistema CRUD básico para administrar clientes.  
Permite:

- Registrar clientes  
- Obtener la lista completa  
- Consultar un cliente individual  
- (Opcional) Actualizar y eliminar registros  

Sirve como base educativa para comprender:

✔ APIs REST  
✔ Arquitectura por capas  
✔ Persistencia con JPA  
✔ Conexión a MySQL  
✔ Validación  
✔ Pruebas con Postman  

---

##  Características

- API REST completamente funcional  
- Conexión a MySQL  
- Uso de Spring Boot 3  
- Respuestas JSON limpias  
- Manejo básico de errores  
- Arquitectura profesional en capas  
- Código entendible y mantenible  

---

##  Tecnologías Utilizadas

- **Java 17**  
- **Spring Boot 3.4**  
- **Spring Web**  
- **Spring Data JPA**  
- **MySQL**  
- **Maven**  
- **Postman**  

---

##  Arquitectura

El proyecto sigue una arquitectura tradicional por capas:

### Descripción de cada capa:

- **Controller:** Recibe y responde peticiones HTTP.  
- **Service:** Contiene la lógica de negocio.  
- **Repository:** Accede a la base de datos usando JPA.  
- **Entity:** Estructura de datos que representa la tabla de BD.

---

##  Requisitos Previos

Instalar:

- Java 17  
- Maven  
- MySQL Server  
- IntelliJ IDEA  
- Postman  

---
##  Instalación y Ejecución

### 1. Clonar el repositorio

```bash
git clone https://github.com/TU-USUARIO/TU-REPO.git

## Crear la base de datos
CREATE DATABASE clientes_db;

Configurar application.properties
spring.datasource.url=jdbc:mysql://localhost:3306/clientes_db
spring.datasource.username=root
spring.datasource.password=TU_PASSWORD

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true


##Ejecutar la aplicación:
mvn spring-boot:run
 

