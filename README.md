# 🚀 **ForoHub Challenge**
¡Bienvenido al ForoHub Challenge! Este proyecto es una API RESTful desarrollada con Spring Boot, que proporciona funcionalidades para gestionar tópicos en un foro.

## 📑 Tabla de Contenidos
Características
Instalación
Uso
Endpoints
Tecnologías Utilizadas
Estructura del Proyecto

## 🌟 Características
🔒 Autenticación de usuarios con JWT
📝 Operaciones CRUD para tópicos
🛡️ Control de acceso basado en roles

## 🛠️ Instalación
Clona el repositorio:

Copiar código
git clone https://github.com/desiperezp/forohub_challenge

cd forohub-challenge

## Configura la base de datos:

Asegúrate de tener una base de datos MySQL en funcionamiento.

Crea una base de datos llamada forohub.

Actualiza la configuración de la base de datos en src/main/resources/application.properties:
spring.datasource.url=jdbc:mysql://localhost:3306/forohub
spring.datasource.username=tuusuario
spring.datasource.password=tupassword

## 🚀 Uso
Para interactuar con la API, puedes usar herramientas como Insomnia o Postman.

## 🛠️ Tecnologías Utilizadas
- Java 17
- Spring Boot 3.3.1
- Spring Security
- JWT para Autenticación
- MySQL
- Flyway para Migraciones de Base de Datos
- Maven

## 🔄 Endpoints

🔐 Autenticación
- Registra un nuevo usuario:
POST /auth/register
```http
{
    "nombre": "Juan Perez",
    "correo_electronico": "juan.perez@example.com",
    "contrasena": "password123"
} 

- Tópicos
POST /topicos
{
    "titulo": "Nuevo Tópico",
    "mensaje": "Este es un nuevo mensaje de tópico.",
    "autor": "Juan Perez",
    "curso": "Spring Boot"
}

- Obtener Todos los Tópicos
PUT /topicos/{id}
{
    "titulo": "Tópico Actualizado",
    "mensaje": "Este es un mensaje de tópico actualizado.",
    "autor": "Juan Perez",
    "curso": "Spring Boot"
}

- Actualizar Tópico
PUT /topicos/{id}
{
    "titulo": "Tópico Actualizado",
    "mensaje": "Este es un mensaje de tópico actualizado.",
    "autor": "Juan Perez",
    "curso": "Spring Boot"
}

- Eliminar Tópico
DELETE /topicos/{id}
